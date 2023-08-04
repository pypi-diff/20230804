# Comparing `tmp/types-aiobotocore-cloudfront-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudfront-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudfront-2.5.2.post1.tar` & `types-aiobotocore-cloudfront-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34119 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32589 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.029637 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83226 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83104 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174495 2023-08-02 14:34:39.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   174134 2023-08-02 14:34:36.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34119 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.791432 types-aiobotocore-cloudfront-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-04 12:00:33.791432 types-aiobotocore-cloudfront-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.791432 types-aiobotocore-cloudfront-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.787432 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83071 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82949 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   138333 2023-08-04 11:41:53.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138070 2023-08-04 11:41:51.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:48.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-04 11:41:49.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.791432 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:33.000000 types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudfront-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/setup.py` & `types-aiobotocore-cloudfront-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudFront 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__main__.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
-    CachePolicyConfigUnionTypeDef,
+    CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,20 +53,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigUnionTypeDef,
+    DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigUnionTypeDef,
-    FieldLevelEncryptionProfileConfigUnionTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -88,16 +88,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchUnionTypeDef,
-    KeyGroupConfigUnionTypeDef,
+    InvalidationBatchTypeDef,
+    KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -115,22 +115,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigUnionTypeDef,
+    OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigUnionTypeDef,
-    StreamingDistributionConfigUnionTypeDef,
+    ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsUnionTypeDef,
+    TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -372,15 +372,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
         """
 
     async def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cache_policy)
         """
@@ -392,26 +392,26 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     async def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     async def create_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef
+        self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution)
         """
@@ -423,25 +423,25 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution_with_tags)
         """
 
     async def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_config)
         """
 
     async def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_profile)
         """
@@ -453,25 +453,25 @@
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_function)
         """
 
     async def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_invalidation)
         """
 
     async def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_key_group)
@@ -494,15 +494,15 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_access_control)
         """
 
     async def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_request_policy)
         """
@@ -533,25 +533,25 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
 
     async def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_response_headers_policy)
         """
 
     async def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_streaming_distribution)
         """
@@ -1251,15 +1251,15 @@
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#publish_function)
         """
 
     async def tag_resource(
-        self, *, Resource: str, Tags: TagsUnionTypeDef
+        self, *, Resource: str, Tags: TagsTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#tag_resource)
         """
@@ -1281,15 +1281,15 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#untag_resource)
         """
 
     async def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cache_policy)
         """
@@ -1307,27 +1307,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     async def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     async def update_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution)
         """
@@ -1342,29 +1342,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     async def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
 
     async def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1383,15 +1383,15 @@
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
 
     async def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_key_group)
         """
@@ -1409,15 +1409,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
 
     async def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1449,29 +1449,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
 
     async def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
 
     async def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
-    CachePolicyConfigUnionTypeDef,
+    CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,20 +53,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigUnionTypeDef,
+    DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigUnionTypeDef,
-    FieldLevelEncryptionProfileConfigUnionTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -88,16 +88,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchUnionTypeDef,
-    KeyGroupConfigUnionTypeDef,
+    InvalidationBatchTypeDef,
+    KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -115,22 +115,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigUnionTypeDef,
+    OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigUnionTypeDef,
-    StreamingDistributionConfigUnionTypeDef,
+    ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsUnionTypeDef,
+    TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -363,15 +363,15 @@
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
         """
     async def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cache_policy)
         """
@@ -381,25 +381,25 @@
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
     async def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_continuous_deployment_policy)
         """
     async def create_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef
+        self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution)
         """
@@ -409,24 +409,24 @@
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution_with_tags)
         """
     async def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_config)
         """
     async def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_profile)
         """
@@ -436,24 +436,24 @@
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_function)
         """
     async def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_invalidation)
         """
     async def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_key_group)
@@ -473,15 +473,15 @@
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_access_control)
         """
     async def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_request_policy)
         """
@@ -509,24 +509,24 @@
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
     async def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_response_headers_policy)
         """
     async def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_streaming_distribution)
         """
@@ -1155,15 +1155,15 @@
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#publish_function)
         """
     async def tag_resource(
-        self, *, Resource: str, Tags: TagsUnionTypeDef
+        self, *, Resource: str, Tags: TagsTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#tag_resource)
         """
@@ -1182,15 +1182,15 @@
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#untag_resource)
         """
     async def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cache_policy)
         """
@@ -1206,26 +1206,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
     async def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
     async def update_distribution(
-        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution)
         """
@@ -1238,28 +1238,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution_with_staging_config)
         """
     async def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
     async def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1276,15 +1276,15 @@
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
     async def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_key_group)
         """
@@ -1300,15 +1300,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
     async def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1337,28 +1337,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
     async def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
     async def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -55,50 +55,40 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasICPRecordalTypeDef",
-    "AliasesOutputTypeDef",
     "AliasesTypeDef",
-    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
-    "TrustedKeyGroupsOutputTypeDef",
-    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
-    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
-    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
-    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -111,22 +101,19 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
-    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
-    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -136,29 +123,27 @@
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
-    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
-    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
@@ -181,29 +166,24 @@
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
-    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
@@ -211,255 +191,201 @@
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
-    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "TestFunctionRequestRequestTypeDef",
-    "CachePolicyCookiesConfigOutputTypeDef",
-    "CookiePreferenceOutputTypeDef",
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
-    "CachePolicyHeadersConfigOutputTypeDef",
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
-    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
-    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
-    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
-    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
-    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
-    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
-    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupConfigUnionTypeDef",
-    "KeyGroupTypeDef",
-    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
-    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
-    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
-    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
-    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
-    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "TagsOutputTypeDef",
     "TagsTypeDef",
-    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
-    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
-    "OriginOutputTypeDef",
     "OriginTypeDef",
-    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
-    "InvalidationBatchUnionTypeDef",
+    "InvalidationTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
-    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
-    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
-    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
-    "StreamingDistributionConfigUnionTypeDef",
+    "GetStreamingDistributionConfigResultTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagsUnionTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigOutputTypeDef",
-    "GetOriginRequestPolicyConfigResultTypeDef",
-    "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
-    "OriginRequestPolicyConfigUnionTypeDef",
+    "GetOriginRequestPolicyConfigResultTypeDef",
+    "OriginRequestPolicyTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "OriginsOutputTypeDef",
+    "KeyGroupListTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
-    "FieldLevelEncryptionProfileSummaryTypeDef",
     "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileSummaryTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
-    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
-    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigOutputTypeDef",
-    "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionSummaryTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
-    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
-    "CachePolicyConfigUnionTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
-    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "ListKeyGroupsResultTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "FieldLevelEncryptionProfileListTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileListTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
-    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "FieldLevelEncryptionListTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionListTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigOutputTypeDef",
-    "DistributionSummaryTypeDef",
     "DistributionConfigTypeDef",
+    "DistributionSummaryTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -470,313 +396,168 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "DistributionTypeDef",
-    "GetDistributionConfigResultTypeDef",
-    "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
+    "DistributionTypeDef",
+    "GetDistributionConfigResultTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
+    "DistributionListTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
-_RequiredAliasesOutputTypeDef = TypedDict(
-    "_RequiredAliasesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalAliasesOutputTypeDef = TypedDict(
-    "_OptionalAliasesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
-    pass
-
-
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
-
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
-
-CachedMethodsOutputTypeDef = TypedDict(
-    "CachedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-    },
-)
-
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
-    "_RequiredTrustedKeyGroupsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-    },
-)
-_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
-    "_OptionalTrustedKeyGroupsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class TrustedKeyGroupsOutputTypeDef(
-    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
-):
-    pass
-
-
-_RequiredTrustedSignersOutputTypeDef = TypedDict(
-    "_RequiredTrustedSignersOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-    },
-)
-_OptionalTrustedSignersOutputTypeDef = TypedDict(
-    "_OptionalTrustedSignersOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class TrustedSignersOutputTypeDef(
-    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
-):
-    pass
-
-
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
-
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
 
-
 _RequiredTrustedSignersTypeDef = TypedDict(
     "_RequiredTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": Sequence[str],
-    },
-    total=False,
-)
-
-
-class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
-    pass
-
-
-_RequiredCookieNamesOutputTypeDef = TypedDict(
-    "_RequiredCookieNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCookieNamesOutputTypeDef = TypedDict(
-    "_OptionalCookieNamesOutputTypeDef",
-    {
         "Items": List[str],
     },
     total=False,
 )
 
-
-class CookieNamesOutputTypeDef(
-    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
-):
+class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
-
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": Sequence[str],
-    },
-    total=False,
-)
-
-
-class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
-    pass
-
-
-_RequiredHeadersOutputTypeDef = TypedDict(
-    "_RequiredHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalHeadersOutputTypeDef = TypedDict(
-    "_OptionalHeadersOutputTypeDef",
-    {
         "Items": List[str],
     },
     total=False,
 )
 
-
-class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
+class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
-
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": Sequence[str],
-    },
-    total=False,
-)
-
-
-class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
-    pass
-
-
-_RequiredQueryStringNamesOutputTypeDef = TypedDict(
-    "_RequiredQueryStringNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryStringNamesOutputTypeDef = TypedDict(
-    "_OptionalQueryStringNamesOutputTypeDef",
-    {
         "Items": List[str],
     },
     total=False,
 )
 
-
-class QueryStringNamesOutputTypeDef(
-    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
-):
+class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
-
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringNamesTypeDef = TypedDict(
     "_OptionalQueryStringNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
-
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -811,64 +592,38 @@
     "_OptionalContentTypeProfileTypeDef",
     {
         "ProfileId": str,
     },
     total=False,
 )
 
-
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
-
-_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class StagingDistributionDnsNamesOutputTypeDef(
-    _RequiredStagingDistributionDnsNamesOutputTypeDef,
-    _OptionalStagingDistributionDnsNamesOutputTypeDef,
-):
-    pass
-
-
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalStagingDistributionDnsNamesTypeDef = TypedDict(
     "_OptionalStagingDistributionDnsNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
-
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
@@ -893,21 +648,19 @@
     {
         "Staging": bool,
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -934,19 +687,17 @@
     "_OptionalKeyGroupConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class KeyGroupConfigTypeDef(_RequiredKeyGroupConfigTypeDef, _OptionalKeyGroupConfigTypeDef):
     pass
 
-
 _RequiredOriginAccessControlConfigTypeDef = TypedDict(
     "_RequiredOriginAccessControlConfigTypeDef",
     {
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
@@ -956,21 +707,19 @@
     "_OptionalOriginAccessControlConfigTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class OriginAccessControlConfigTypeDef(
     _RequiredOriginAccessControlConfigTypeDef, _OptionalOriginAccessControlConfigTypeDef
 ):
     pass
 
-
 _RequiredPublicKeyConfigTypeDef = TypedDict(
     "_RequiredPublicKeyConfigTypeDef",
     {
         "CallerReference": str,
         "Name": str,
         "EncodedKey": str,
     },
@@ -979,19 +728,17 @@
     "_OptionalPublicKeyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
-
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -1000,42 +747,32 @@
         "ResponsePagePath": str,
         "ResponseCode": str,
         "ErrorCachingMinTTL": int,
     },
     total=False,
 )
 
-
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
-
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
-OriginSslProtocolsOutputTypeDef = TypedDict(
-    "OriginSslProtocolsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[SslProtocolType],
-    },
-)
-
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[SslProtocolType],
+        "Items": List[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -1045,131 +782,119 @@
     "_OptionalDeleteCachePolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteCachePolicyRequestRequestTypeDef(
     _RequiredDeleteCachePolicyRequestRequestTypeDef, _OptionalDeleteCachePolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteDistributionRequestRequestTypeDef(
     _RequiredDeleteDistributionRequestRequestTypeDef,
     _OptionalDeleteDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteFieldLevelEncryptionConfigRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteFunctionRequestRequestTypeDef = TypedDict(
     "DeleteFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -1184,21 +909,19 @@
     "_OptionalDeleteKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteKeyGroupRequestRequestTypeDef(
     _RequiredDeleteKeyGroupRequestRequestTypeDef, _OptionalDeleteKeyGroupRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 
@@ -1212,65 +935,59 @@
     "_OptionalDeleteOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteOriginAccessControlRequestRequestTypeDef(
     _RequiredDeleteOriginAccessControlRequestRequestTypeDef,
     _OptionalDeleteOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteOriginRequestPolicyRequestRequestTypeDef(
     _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef,
     _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeletePublicKeyRequestRequestTypeDef(
     _RequiredDeletePublicKeyRequestRequestTypeDef, _OptionalDeletePublicKeyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "ARN": str,
     },
     total=False,
@@ -1286,65 +1003,59 @@
     "_OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredDeleteResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingDistributionRequestRequestTypeDef(
     _RequiredDeleteStreamingDistributionRequestRequestTypeDef,
     _OptionalDeleteStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFunctionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1379,111 +1090,63 @@
     {
         "NextMarker": str,
         "Items": List[str],
     },
     total=False,
 )
 
-
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
-
-_RequiredFieldPatternsOutputTypeDef = TypedDict(
-    "_RequiredFieldPatternsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalFieldPatternsOutputTypeDef = TypedDict(
-    "_OptionalFieldPatternsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class FieldPatternsOutputTypeDef(
-    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
-):
-    pass
-
-
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsTypeDef = TypedDict(
     "_OptionalFieldPatternsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
-
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
-_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
-    "_RequiredQueryStringCacheKeysOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
-    "_OptionalQueryStringCacheKeysOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class QueryStringCacheKeysOutputTypeDef(
-    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
-):
-    pass
-
-
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
-
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
-
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1500,61 +1163,35 @@
     {
         "Stage": FunctionStageType,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
-
-_RequiredGeoRestrictionOutputTypeDef = TypedDict(
-    "_RequiredGeoRestrictionOutputTypeDef",
-    {
-        "RestrictionType": GeoRestrictionTypeType,
-        "Quantity": int,
-    },
-)
-_OptionalGeoRestrictionOutputTypeDef = TypedDict(
-    "_OptionalGeoRestrictionOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class GeoRestrictionOutputTypeDef(
-    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
-):
-    pass
-
-
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
-
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
 
-
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1654,21 +1291,19 @@
     "_OptionalGetFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
-
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1676,36 +1311,14 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredKeyGroupConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Items": List[str],
-    },
-)
-_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalKeyGroupConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-
-class KeyGroupConfigOutputTypeDef(
-    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
-):
-    pass
-
-
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1791,52 +1404,31 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredPathsOutputTypeDef = TypedDict(
-    "_RequiredPathsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalPathsOutputTypeDef = TypedDict(
-    "_OptionalPathsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
-    pass
-
-
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
     "_OptionalPathsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class PathsTypeDef(_RequiredPathsTypeDef, _OptionalPathsTypeDef):
     pass
 
-
 InvalidationSummaryTypeDef = TypedDict(
     "InvalidationSummaryTypeDef",
     {
         "Id": str,
         "CreateTime": datetime,
         "Status": str,
     },
@@ -1852,19 +1444,17 @@
     "_OptionalKeyPairIdsTypeDef",
     {
         "Items": List[str],
     },
     total=False,
 )
 
-
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
-
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1872,21 +1462,19 @@
     "_OptionalLambdaFunctionAssociationTypeDef",
     {
         "IncludeBody": bool,
     },
     total=False,
 )
 
-
 class LambdaFunctionAssociationTypeDef(
     _RequiredLambdaFunctionAssociationTypeDef, _OptionalLambdaFunctionAssociationTypeDef
 ):
     pass
 
-
 ListCachePoliciesRequestRequestTypeDef = TypedDict(
     "ListCachePoliciesRequestRequestTypeDef",
     {
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
@@ -1924,22 +1512,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListConflictingAliasesRequestRequestTypeDef(
     _RequiredListConflictingAliasesRequestRequestTypeDef,
     _OptionalListConflictingAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 ListContinuousDeploymentPoliciesRequestRequestTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1956,22 +1542,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByCachePolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByCachePolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByCachePolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupId": str,
     },
 )
 _OptionalListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
@@ -1979,22 +1563,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByKeyGroupRequestRequestTypeDef(
     _RequiredListDistributionsByKeyGroupRequestRequestTypeDef,
     _OptionalListDistributionsByKeyGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     {
         "OriginRequestPolicyId": str,
     },
 )
 _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
@@ -2002,22 +1584,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 ListDistributionsByRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "RealtimeLogConfigName": str,
         "RealtimeLogConfigArn": str,
@@ -2036,22 +1616,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByWebACLIdRequestRequestTypeDef",
     {
         "WebACLId": str,
     },
 )
 _OptionalListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
@@ -2059,22 +1637,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
-
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2119,21 +1695,19 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListInvalidationsRequestRequestTypeDef(
     _RequiredListInvalidationsRequestRequestTypeDef, _OptionalListInvalidationsRequestRequestTypeDef
 ):
     pass
 
-
 ListKeyGroupsRequestRequestTypeDef = TypedDict(
     "ListKeyGroupsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2217,27 +1791,19 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
-StatusCodesOutputTypeDef = TypedDict(
-    "StatusCodesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[int],
-    },
-)
-
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[int],
+        "Items": List[int],
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
@@ -2254,19 +1820,17 @@
     "_OptionalOriginShieldTypeDef",
     {
         "OriginShieldRegion": str,
     },
     total=False,
 )
 
-
 class OriginShieldTypeDef(_RequiredOriginShieldTypeDef, _OptionalOriginShieldTypeDef):
     pass
 
-
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
 )
 
@@ -2283,19 +1847,17 @@
     "_OptionalPublicKeySummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class PublicKeySummaryTypeDef(_RequiredPublicKeySummaryTypeDef, _OptionalPublicKeySummaryTypeDef):
     pass
 
-
 PublishFunctionRequestRequestTypeDef = TypedDict(
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -2304,128 +1866,78 @@
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
-_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
-    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
-
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "SamplingRate": float,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
-
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
@@ -2481,22 +1993,20 @@
     {
         "IncludeSubdomains": bool,
         "Preload": bool,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyStrictTransportSecurityTypeDef(
     _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef,
     _OptionalResponseHeadersPolicyStrictTransportSecurityTypeDef,
 ):
     pass
 
-
 _RequiredResponseHeadersPolicyXSSProtectionTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyXSSProtectionTypeDef",
     {
         "Override": bool,
         "Protection": bool,
     },
 )
@@ -2505,22 +2015,20 @@
     {
         "ModeBlock": bool,
         "ReportUri": str,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
 ):
     pass
 
-
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
@@ -2552,19 +2060,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
@@ -2572,64 +2078,38 @@
     {
         "StagingDistributionId": str,
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
     _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
     _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredAllowedMethodsOutputTypeDef = TypedDict(
-    "_RequiredAllowedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-    },
-)
-_OptionalAllowedMethodsOutputTypeDef = TypedDict(
-    "_OptionalAllowedMethodsOutputTypeDef",
-    {
-        "CachedMethods": CachedMethodsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AllowedMethodsOutputTypeDef(
-    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
-):
-    pass
-
-
 _RequiredAllowedMethodsTypeDef = TypedDict(
     "_RequiredAllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 _OptionalAllowedMethodsTypeDef = TypedDict(
     "_OptionalAllowedMethodsTypeDef",
     {
         "CachedMethods": CachedMethodsTypeDef,
     },
     total=False,
 )
 
-
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
-
 _RequiredTestFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredTestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "EventObject": BlobTypeDef,
     },
@@ -2638,320 +2118,153 @@
     "_OptionalTestFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class TestFunctionRequestRequestTypeDef(
     _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": CachePolicyCookieBehaviorType,
-    },
-)
-_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
-    {
-        "Cookies": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CachePolicyCookiesConfigOutputTypeDef(
-    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredCookiePreferenceOutputTypeDef = TypedDict(
-    "_RequiredCookiePreferenceOutputTypeDef",
-    {
-        "Forward": ItemSelectionType,
-    },
-)
-_OptionalCookiePreferenceOutputTypeDef = TypedDict(
-    "_OptionalCookiePreferenceOutputTypeDef",
-    {
-        "WhitelistedNames": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CookiePreferenceOutputTypeDef(
-    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
-):
-    pass
-
-
-_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "Cookies": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class OriginRequestPolicyCookiesConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalCachePolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyCookiesConfigTypeDef(
     _RequiredCachePolicyCookiesConfigTypeDef, _OptionalCachePolicyCookiesConfigTypeDef
 ):
     pass
 
-
 _RequiredCookiePreferenceTypeDef = TypedDict(
     "_RequiredCookiePreferenceTypeDef",
     {
         "Forward": ItemSelectionType,
     },
 )
 _OptionalCookiePreferenceTypeDef = TypedDict(
     "_OptionalCookiePreferenceTypeDef",
     {
         "WhitelistedNames": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class CookiePreferenceTypeDef(_RequiredCookiePreferenceTypeDef, _OptionalCookiePreferenceTypeDef):
     pass
 
-
 _RequiredOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
-
-_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": CachePolicyHeaderBehaviorType,
-    },
-)
-_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CachePolicyHeadersConfigOutputTypeDef(
-    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class OriginRequestPolicyHeadersConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
 _OptionalCachePolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalCachePolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyHeadersConfigTypeDef(
     _RequiredCachePolicyHeadersConfigTypeDef, _OptionalCachePolicyHeadersConfigTypeDef
 ):
     pass
 
-
 _RequiredOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
-
-_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
-    },
-)
-_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStrings": QueryStringNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CachePolicyQueryStringsConfigOutputTypeDef(
-    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
-    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
-):
-    pass
-
-
-_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStrings": QueryStringNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
 _OptionalCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyQueryStringsConfigTypeDef(
     _RequiredCachePolicyQueryStringsConfigTypeDef, _OptionalCachePolicyQueryStringsConfigTypeDef
 ):
     pass
 
-
 _RequiredOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyQueryStringsConfigTypeDef(
     _RequiredOriginRequestPolicyQueryStringsConfigTypeDef,
     _OptionalOriginRequestPolicyQueryStringsConfigTypeDef,
 ):
     pass
 
-
 _RequiredCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityTypeDef",
     {
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
@@ -2959,21 +2272,19 @@
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
-
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
-
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
@@ -2988,22 +2299,20 @@
     "_OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCloudFrontOriginAccessIdentityListTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -3014,97 +2323,70 @@
     {
         "NextMarker": str,
         "Items": List[CloudFrontOriginAccessIdentitySummaryTypeDef],
     },
     total=False,
 )
 
-
 class CloudFrontOriginAccessIdentityListTypeDef(
     _RequiredCloudFrontOriginAccessIdentityListTypeDef,
     _OptionalCloudFrontOriginAccessIdentityListTypeDef,
 ):
     pass
 
-
 ConflictingAliasesListTypeDef = TypedDict(
     "ConflictingAliasesListTypeDef",
     {
         "NextMarker": str,
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
-_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfilesOutputTypeDef",
-    {
-        "Items": List[ContentTypeProfileTypeDef],
-    },
-    total=False,
-)
-
-
-class ContentTypeProfilesOutputTypeDef(
-    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
-):
-    pass
-
-
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
     "_OptionalContentTypeProfilesTypeDef",
     {
         "Items": Sequence[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
-
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
-
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_OptionalContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "SessionStickinessConfig": SessionStickinessConfigTypeDef,
     },
     total=False,
 )
 
-
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3149,14 +2431,32 @@
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+    },
+)
+
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -3164,21 +2464,19 @@
     "_OptionalUpdateKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateKeyGroupRequestRequestTypeDef(
     _RequiredUpdateKeyGroupRequestRequestTypeDef, _OptionalUpdateKeyGroupRequestRequestTypeDef
 ):
     pass
 
-
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
@@ -3201,21 +2499,19 @@
     "_OptionalOriginAccessControlTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
     total=False,
 )
 
-
 class OriginAccessControlTypeDef(
     _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
 ):
     pass
 
-
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -3223,22 +2519,20 @@
     "_OptionalUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateOriginAccessControlRequestRequestTypeDef(
     _RequiredUpdateOriginAccessControlRequestRequestTypeDef,
     _OptionalUpdateOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
@@ -3271,128 +2565,55 @@
     "_OptionalUpdatePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
-    "_RequiredCustomErrorResponsesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
-    "_OptionalCustomErrorResponsesOutputTypeDef",
-    {
-        "Items": List[CustomErrorResponseTypeDef],
-    },
-    total=False,
-)
-
-
-class CustomErrorResponsesOutputTypeDef(
-    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": Sequence[CustomErrorResponseTypeDef],
+        "Items": List[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
-
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
-
-_RequiredCustomHeadersOutputTypeDef = TypedDict(
-    "_RequiredCustomHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCustomHeadersOutputTypeDef = TypedDict(
-    "_OptionalCustomHeadersOutputTypeDef",
-    {
-        "Items": List[OriginCustomHeaderTypeDef],
-    },
-    total=False,
-)
-
-
-class CustomHeadersOutputTypeDef(
-    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": Sequence[OriginCustomHeaderTypeDef],
+        "Items": List[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
-
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
-
-_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
-    "_RequiredCustomOriginConfigOutputTypeDef",
-    {
-        "HTTPPort": int,
-        "HTTPSPort": int,
-        "OriginProtocolPolicy": OriginProtocolPolicyType,
-    },
-)
-_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
-    "_OptionalCustomOriginConfigOutputTypeDef",
-    {
-        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
-        "OriginReadTimeout": int,
-        "OriginKeepaliveTimeout": int,
-    },
-    total=False,
-)
-
-
-class CustomOriginConfigOutputTypeDef(
-    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
     },
@@ -3403,21 +2624,19 @@
         "OriginSslProtocols": OriginSslProtocolsTypeDef,
         "OriginReadTimeout": int,
         "OriginKeepaliveTimeout": int,
     },
     total=False,
 )
 
-
 class CustomOriginConfigTypeDef(
     _RequiredCustomOriginConfigTypeDef, _OptionalCustomOriginConfigTypeDef
 ):
     pass
 
-
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3442,23 +2661,14 @@
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EncryptionEntityOutputTypeDef = TypedDict(
-    "EncryptionEntityOutputTypeDef",
-    {
-        "PublicKeyId": str,
-        "ProviderId": str,
-        "FieldPatterns": FieldPatternsOutputTypeDef,
-    },
-)
-
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
@@ -3474,61 +2684,36 @@
     "_OptionalEndPointTypeDef",
     {
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
     },
     total=False,
 )
 
-
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
-
-_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
-    "_RequiredFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
-    "_OptionalFunctionAssociationsOutputTypeDef",
-    {
-        "Items": List[FunctionAssociationTypeDef],
-    },
-    total=False,
-)
-
-
-class FunctionAssociationsOutputTypeDef(
-    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
-):
-    pass
-
-
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": Sequence[FunctionAssociationTypeDef],
+        "Items": List[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
-
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
 ):
     pass
 
-
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
@@ -3537,26 +2722,17 @@
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
-
-RestrictionsOutputTypeDef = TypedDict(
-    "RestrictionsOutputTypeDef",
-    {
-        "GeoRestriction": GeoRestrictionOutputTypeDef,
-    },
-)
-
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
 
@@ -3570,22 +2746,20 @@
     "_OptionalGetDistributionRequestDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetDistributionRequestDistributionDeployedWaitTypeDef(
     _RequiredGetDistributionRequestDistributionDeployedWaitTypeDef,
     _OptionalGetDistributionRequestDistributionDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef = TypedDict(
     "_RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -3593,71 +2767,40 @@
     "_OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetInvalidationRequestInvalidationCompletedWaitTypeDef(
     _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef,
     _OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
-
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-    },
-)
-
-InvalidationBatchOutputTypeDef = TypedDict(
-    "InvalidationBatchOutputTypeDef",
-    {
-        "Paths": PathsOutputTypeDef,
-        "CallerReference": str,
-    },
-)
-
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -3676,19 +2819,17 @@
     {
         "NextMarker": str,
         "Items": List[InvalidationSummaryTypeDef],
     },
     total=False,
 )
 
-
 class InvalidationListTypeDef(_RequiredInvalidationListTypeDef, _OptionalInvalidationListTypeDef):
     pass
 
-
 KGKeyPairIdsTypeDef = TypedDict(
     "KGKeyPairIdsTypeDef",
     {
         "KeyGroupId": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
@@ -3699,57 +2840,33 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
-_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Items": List[LambdaFunctionAssociationTypeDef],
-    },
-    total=False,
-)
-
-
-class LambdaFunctionAssociationsOutputTypeDef(
-    _RequiredLambdaFunctionAssociationsOutputTypeDef,
-    _OptionalLambdaFunctionAssociationsOutputTypeDef,
-):
-    pass
-
-
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": Sequence[LambdaFunctionAssociationTypeDef],
+        "Items": List[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
-
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
-
 ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -3772,22 +2889,20 @@
     "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
     _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
     _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
 ):
     pass
 
-
 ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -3814,48 +2929,31 @@
     {
         "NextMarker": str,
         "Items": List[OriginAccessControlSummaryTypeDef],
     },
     total=False,
 )
 
-
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
-
-OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
-    "OriginGroupFailoverCriteriaOutputTypeDef",
-    {
-        "StatusCodes": StatusCodesOutputTypeDef,
-    },
-)
-
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
-OriginGroupMembersOutputTypeDef = TypedDict(
-    "OriginGroupMembersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
-    },
-)
-
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginGroupMemberTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -3867,86 +2965,34 @@
     {
         "NextMarker": str,
         "Items": List[PublicKeySummaryTypeDef],
     },
     total=False,
 )
 
-
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
-
-_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
-    "_RequiredQueryArgProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
-    "_OptionalQueryArgProfilesOutputTypeDef",
-    {
-        "Items": List[QueryArgProfileTypeDef],
-    },
-    total=False,
-)
-
-
-class QueryArgProfilesOutputTypeDef(
-    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
-):
-    pass
-
-
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesTypeDef = TypedDict(
     "_OptionalQueryArgProfilesTypeDef",
     {
         "Items": Sequence[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
-
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
-
-_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
-        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
-        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
-        "AccessControlAllowCredentials": bool,
-        "OriginOverride": bool,
-    },
-)
-_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-        "AccessControlMaxAgeSec": int,
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyCorsConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
@@ -3958,109 +3004,59 @@
     {
         "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
         "AccessControlMaxAgeSec": int,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
-
-_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
-
-_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
-
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -4075,50 +3071,22 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesOutputTypeDef,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "TrustedSigners": TrustedSignersTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
-_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
-    "_RequiredStreamingDistributionConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "S3Origin": S3OriginTypeDef,
-        "Comment": str,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "Enabled": bool,
-    },
-)
-_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
-    "_OptionalStreamingDistributionConfigOutputTypeDef",
-    {
-        "Aliases": AliasesOutputTypeDef,
-        "Logging": StreamingLoggingConfigTypeDef,
-        "PriceClass": PriceClassType,
-    },
-    total=False,
-)
-
-
-class StreamingDistributionConfigOutputTypeDef(
-    _RequiredStreamingDistributionConfigOutputTypeDef,
-    _OptionalStreamingDistributionConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -4131,68 +3099,35 @@
         "Aliases": AliasesTypeDef,
         "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
-
 class StreamingDistributionConfigTypeDef(
     _RequiredStreamingDistributionConfigTypeDef, _OptionalStreamingDistributionConfigTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
-TagsOutputTypeDef = TypedDict(
-    "TagsOutputTypeDef",
-    {
-        "Items": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredForwardedValuesOutputTypeDef = TypedDict(
-    "_RequiredForwardedValuesOutputTypeDef",
-    {
-        "QueryString": bool,
-        "Cookies": CookiePreferenceOutputTypeDef,
-    },
-)
-_OptionalForwardedValuesOutputTypeDef = TypedDict(
-    "_OptionalForwardedValuesOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ForwardedValuesOutputTypeDef(
-    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
-):
-    pass
-
-
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -4201,68 +3136,17 @@
     {
         "Headers": HeadersTypeDef,
         "QueryStringCacheKeys": QueryStringCacheKeysTypeDef,
     },
     total=False,
 )
 
-
 class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
-
-_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingGzip": bool,
-        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
-    },
-)
-_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingBrotli": bool,
-    },
-    total=False,
-)
-
-
-class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
-    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
-    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
-):
-    pass
-
-
-_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
-    },
-)
-_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-
-class OriginRequestPolicyConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -4272,22 +3156,20 @@
     "_OptionalParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingBrotli": bool,
     },
     total=False,
 )
 
-
 class ParametersInCacheKeyAndForwardedToOriginTypeDef(
     _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef,
     _OptionalParametersInCacheKeyAndForwardedToOriginTypeDef,
 ):
     pass
 
-
 _RequiredOriginRequestPolicyConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyConfigTypeDef",
     {
         "Name": str,
         "HeadersConfig": OriginRequestPolicyHeadersConfigTypeDef,
         "CookiesConfig": OriginRequestPolicyCookiesConfigTypeDef,
         "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigTypeDef,
@@ -4297,21 +3179,19 @@
     "_OptionalOriginRequestPolicyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyConfigTypeDef(
     _RequiredOriginRequestPolicyConfigTypeDef, _OptionalOriginRequestPolicyConfigTypeDef
 ):
     pass
 
-
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4348,56 +3228,33 @@
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenContentTypeIsUnknown": bool,
-    },
-)
-_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfileConfigOutputTypeDef",
-    {
-        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ContentTypeProfileConfigOutputTypeDef(
-    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
 _OptionalContentTypeProfileConfigTypeDef = TypedDict(
     "_OptionalContentTypeProfileConfigTypeDef",
     {
         "ContentTypeProfiles": ContentTypeProfilesTypeDef,
     },
     total=False,
 )
 
-
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
-
 _RequiredTrafficConfigTypeDef = TypedDict(
     "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
 _OptionalTrafficConfigTypeDef = TypedDict(
@@ -4405,18 +3262,51 @@
     {
         "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
         "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
@@ -4466,41 +3356,14 @@
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredOriginOutputTypeDef = TypedDict(
-    "_RequiredOriginOutputTypeDef",
-    {
-        "Id": str,
-        "DomainName": str,
-    },
-)
-_OptionalOriginOutputTypeDef = TypedDict(
-    "_OptionalOriginOutputTypeDef",
-    {
-        "OriginPath": str,
-        "CustomHeaders": CustomHeadersOutputTypeDef,
-        "S3OriginConfig": S3OriginConfigTypeDef,
-        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
-        "ConnectionAttempts": int,
-        "ConnectionTimeout": int,
-        "OriginShield": OriginShieldTypeDef,
-        "OriginAccessControlId": str,
-    },
-    total=False,
-)
-
-
-class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
-    pass
-
-
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
@@ -4515,61 +3378,36 @@
         "ConnectionTimeout": int,
         "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
-
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
-
-_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
-    "_RequiredEncryptionEntitiesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
-    "_OptionalEncryptionEntitiesOutputTypeDef",
-    {
-        "Items": List[EncryptionEntityOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class EncryptionEntitiesOutputTypeDef(
-    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
-):
-    pass
-
-
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalEncryptionEntitiesTypeDef = TypedDict(
     "_OptionalEncryptionEntitiesTypeDef",
     {
         "Items": Sequence[EncryptionEntityTypeDef],
     },
     total=False,
 )
 
-
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
-
 CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
         "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
@@ -4630,19 +3468,17 @@
     {
         "NextMarker": str,
         "Items": List[FunctionSummaryTypeDef],
     },
     total=False,
 )
 
-
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
-
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4664,68 +3500,32 @@
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DistributionId": str,
+        "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
-        "InvalidationBatch": InvalidationBatchOutputTypeDef,
-    },
-)
-
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
-    {
-        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
-InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4741,21 +3541,19 @@
     "_OptionalActiveTrustedKeyGroupsTypeDef",
     {
         "Items": List[KGKeyPairIdsTypeDef],
     },
     total=False,
 )
 
-
 class ActiveTrustedKeyGroupsTypeDef(
     _RequiredActiveTrustedKeyGroupsTypeDef, _OptionalActiveTrustedKeyGroupsTypeDef
 ):
     pass
 
-
 _RequiredActiveTrustedSignersTypeDef = TypedDict(
     "_RequiredActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -4763,21 +3561,19 @@
     "_OptionalActiveTrustedSignersTypeDef",
     {
         "Items": List[SignerTypeDef],
     },
     total=False,
 )
 
-
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
-
 CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
@@ -4802,23 +3598,14 @@
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OriginGroupOutputTypeDef = TypedDict(
-    "OriginGroupOutputTypeDef",
-    {
-        "Id": str,
-        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
-        "Members": OriginGroupMembersOutputTypeDef,
-    },
-)
-
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -4828,83 +3615,33 @@
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredQueryArgProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenQueryArgProfileIsUnknown": bool,
-    },
-)
-_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalQueryArgProfileConfigOutputTypeDef",
-    {
-        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryArgProfileConfigOutputTypeDef(
-    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
 _OptionalQueryArgProfileConfigTypeDef = TypedDict(
     "_OptionalQueryArgProfileConfigTypeDef",
     {
         "QueryArgProfiles": QueryArgProfilesTypeDef,
     },
     total=False,
 )
 
-
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
-
-_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
-        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
-        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
-        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ResponseHeadersPolicyConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalResponseHeadersPolicyConfigTypeDef = TypedDict(
@@ -4916,21 +3653,19 @@
         "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyConfigTypeDef(
     _RequiredResponseHeadersPolicyConfigTypeDef, _OptionalResponseHeadersPolicyConfigTypeDef
 ):
     pass
 
-
 _RequiredStreamingDistributionListTypeDef = TypedDict(
     "_RequiredStreamingDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -4941,40 +3676,35 @@
     {
         "NextMarker": str,
         "Items": List[StreamingDistributionSummaryTypeDef],
     },
     total=False,
 )
 
-
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
-
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamingDistributionConfigUnionTypeDef = Union[
-    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -4982,26 +3712,24 @@
     "_OptionalUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateStreamingDistributionRequestRequestTypeDef(
     _RequiredUpdateStreamingDistributionRequestRequestTypeDef,
     _OptionalUpdateStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsOutputTypeDef,
+        "Tags": TagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
@@ -5014,90 +3742,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
-TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
-_RequiredCacheBehaviorOutputTypeDef = TypedDict(
-    "_RequiredCacheBehaviorOutputTypeDef",
-    {
-        "PathPattern": str,
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-    },
-)
-_OptionalCacheBehaviorOutputTypeDef = TypedDict(
-    "_OptionalCacheBehaviorOutputTypeDef",
-    {
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
-        "AllowedMethods": AllowedMethodsOutputTypeDef,
-        "SmoothStreaming": bool,
-        "Compress": bool,
-        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
-        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
-        "FieldLevelEncryptionId": str,
-        "RealtimeLogConfigArn": str,
-        "CachePolicyId": str,
-        "OriginRequestPolicyId": str,
-        "ResponseHeadersPolicyId": str,
-        "ForwardedValues": ForwardedValuesOutputTypeDef,
-        "MinTTL": int,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-    },
-    total=False,
-)
-
-
-class CacheBehaviorOutputTypeDef(
-    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
-):
-    pass
-
-
-_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "_RequiredDefaultCacheBehaviorOutputTypeDef",
-    {
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-    },
-)
-_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "_OptionalDefaultCacheBehaviorOutputTypeDef",
-    {
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
-        "AllowedMethods": AllowedMethodsOutputTypeDef,
-        "SmoothStreaming": bool,
-        "Compress": bool,
-        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
-        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
-        "FieldLevelEncryptionId": str,
-        "RealtimeLogConfigArn": str,
-        "CachePolicyId": str,
-        "OriginRequestPolicyId": str,
-        "ResponseHeadersPolicyId": str,
-        "ForwardedValues": ForwardedValuesOutputTypeDef,
-        "MinTTL": int,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-    },
-    total=False,
-)
-
-
-class DefaultCacheBehaviorOutputTypeDef(
-    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
-):
-    pass
-
-
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -5121,19 +3773,17 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
-
 class CacheBehaviorTypeDef(_RequiredCacheBehaviorTypeDef, _OptionalCacheBehaviorTypeDef):
     pass
 
-
 _RequiredDefaultCacheBehaviorTypeDef = TypedDict(
     "_RequiredDefaultCacheBehaviorTypeDef",
     {
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
 )
@@ -5156,101 +3806,67 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
-
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
-
-_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigOutputTypeDef",
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigOutputTypeDef",
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": (
-            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
-        ),
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
     },
     total=False,
 )
 
-
-class CachePolicyConfigOutputTypeDef(
-    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
 ):
     pass
 
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+    },
+)
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
-    },
-)
-
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
-    {
-        "Name": str,
-        "MinTTL": int,
-    },
-)
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
-    {
-        "Comment": str,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
-    },
-    total=False,
-)
-
-
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
-):
-    pass
-
-
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
-OriginRequestPolicyConfigUnionTypeDef = Union[
-    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5258,45 +3874,20 @@
     "_OptionalUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
-        "Enabled": bool,
-    },
-)
-_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "TrafficConfig": TrafficConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ContinuousDeploymentPolicyConfigOutputTypeDef(
-    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
-    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
 )
@@ -5304,111 +3895,92 @@
     "_OptionalContinuousDeploymentPolicyConfigTypeDef",
     {
         "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
-
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
-
-OriginsOutputTypeDef = TypedDict(
-    "OriginsOutputTypeDef",
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
     {
+        "MaxItems": int,
         "Quantity": int,
-        "Items": List[OriginOutputTypeDef],
     },
 )
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginTypeDef],
+        "Items": List[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
-class FieldLevelEncryptionProfileConfigOutputTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
 ):
     pass
 
-
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
-
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Name": str,
-        "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
-    },
-)
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
-):
-    pass
-
-
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5434,21 +4006,19 @@
     {
         "Items": List[RealtimeLogConfigTypeDef],
         "NextMarker": str,
     },
     total=False,
 )
 
-
 class RealtimeLogConfigsTypeDef(
     _RequiredRealtimeLogConfigsTypeDef, _OptionalRealtimeLogConfigsTypeDef
 ):
     pass
 
-
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5465,35 +4035,14 @@
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
-
-
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5511,171 +4060,115 @@
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
-
-_RequiredOriginGroupsOutputTypeDef = TypedDict(
-    "_RequiredOriginGroupsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalOriginGroupsOutputTypeDef = TypedDict(
-    "_OptionalOriginGroupsOutputTypeDef",
-    {
-        "Items": List[OriginGroupOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class OriginGroupsOutputTypeDef(
-    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
-):
-    pass
-
-
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": Sequence[OriginGroupTypeDef],
+        "Items": List[OriginGroupTypeDef],
     },
     total=False,
 )
 
-
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
-
-_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
     total=False,
 )
 
-
-class FieldLevelEncryptionConfigOutputTypeDef(
-    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
-    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
 ):
     pass
 
-
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
     total=False,
 )
 
-
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
-
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
-    {
-        "CallerReference": str,
-    },
-)
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
-        "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
-    total=False,
 )
 
-
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
-):
-    pass
-
-
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
-    },
-)
-
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
-ResponseHeadersPolicyConfigUnionTypeDef = Union[
-    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5683,22 +4176,20 @@
     "_OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5706,72 +4197,76 @@
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
-_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
-    "_RequiredCacheBehaviorsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
-    "_OptionalCacheBehaviorsOutputTypeDef",
-    {
-        "Items": List[CacheBehaviorOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class CacheBehaviorsOutputTypeDef(
-    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
-):
-    pass
-
-
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": Sequence[CacheBehaviorTypeDef],
+        "Items": List[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
-
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
-
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5800,69 +4295,36 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
-
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
-ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
-    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-]
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -5873,73 +4335,53 @@
     "_OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-FieldLevelEncryptionProfileTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
-    },
-)
-
-GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
-    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
-        "ETag": str,
+        "KeyGroupList": KeyGroupListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+
+FieldLevelEncryptionProfileTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
-    total=False,
 )
 
-
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
-):
-    pass
-
-
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
+    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
-    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -5947,34 +4389,45 @@
     "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-
-ListRealtimeLogConfigsResultTypeDef = TypedDict(
-    "ListRealtimeLogConfigsResultTypeDef",
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+    },
+    total=False,
+)
 
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+):
+    pass
+
+ListRealtimeLogConfigsResultTypeDef = TypedDict(
+    "ListRealtimeLogConfigsResultTypeDef",
     {
-        "KeyGroupList": KeyGroupListTypeDef,
+        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
@@ -6009,65 +4462,39 @@
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+    },
+)
+
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
-):
-    pass
-
-
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
-
-FieldLevelEncryptionConfigUnionTypeDef = Union[
-    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-]
 _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "Id": str,
     },
 )
@@ -6075,21 +4502,40 @@
     "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
+    {
+        "MaxItems": int,
+        "Quantity": int,
+    },
+)
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+    },
+    total=False,
+)
+
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+):
+    pass
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
@@ -6119,130 +4565,88 @@
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDistributionConfigOutputTypeDef = TypedDict(
-    "_RequiredDistributionConfigOutputTypeDef",
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigOutputTypeDef = TypedDict(
-    "_OptionalDistributionConfigOutputTypeDef",
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
     {
-        "Aliases": AliasesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
-
-class DistributionConfigOutputTypeDef(
-    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
 ):
     pass
 
-
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesOutputTypeDef,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsOutputTypeDef,
+        "OriginGroups": OriginGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
-
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
-
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
-    {
-        "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "Comment": str,
-        "Enabled": bool,
-    },
-)
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
-    {
-        "Aliases": AliasesTypeDef,
-        "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
-        "Logging": LoggingConfigTypeDef,
-        "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
-        "WebACLId": str,
-        "HttpVersion": HttpVersionType,
-        "IsIPV6Enabled": bool,
-        "ContinuousDeploymentPolicyId": str,
-        "Staging": bool,
-    },
-    total=False,
-)
-
-
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
-):
-    pass
-
-
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
 )
@@ -6287,21 +4691,19 @@
     {
         "NextMarker": str,
         "Items": List[OriginRequestPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class OriginRequestPolicyListTypeDef(
     _RequiredOriginRequestPolicyListTypeDef, _OptionalOriginRequestPolicyListTypeDef
 ):
     pass
 
-
 ContinuousDeploymentPolicySummaryTypeDef = TypedDict(
     "ContinuousDeploymentPolicySummaryTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
     },
 )
 
@@ -6417,96 +4819,68 @@
     {
         "NextMarker": str,
         "Items": List[ResponseHeadersPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
 
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
-
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
-
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDistributionListTypeDef = TypedDict(
-    "_RequiredDistributionListTypeDef",
-    {
-        "Marker": str,
-        "MaxItems": int,
-        "IsTruncated": bool,
-        "Quantity": int,
-    },
-)
-_OptionalDistributionListTypeDef = TypedDict(
-    "_OptionalDistributionListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[DistributionSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
-    pass
-
-
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -6514,21 +4888,40 @@
     "_OptionalUpdateDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateDistributionRequestRequestTypeDef(
     _RequiredUpdateDistributionRequestRequestTypeDef,
     _OptionalUpdateDistributionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDistributionListTypeDef = TypedDict(
+    "_RequiredDistributionListTypeDef",
+    {
+        "Marker": str,
+        "MaxItems": int,
+        "IsTruncated": bool,
+        "Quantity": int,
+    },
+)
+_OptionalDistributionListTypeDef = TypedDict(
+    "_OptionalDistributionListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[DistributionSummaryTypeDef],
+    },
+    total=False,
+)
+
+class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
+    pass
 
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
     },
@@ -6538,19 +4931,17 @@
     {
         "NextMarker": str,
         "Items": List[CachePolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
-
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6567,29 +4958,34 @@
     {
         "NextMarker": str,
         "Items": List[ContinuousDeploymentPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class ContinuousDeploymentPolicyListTypeDef(
     _RequiredContinuousDeploymentPolicyListTypeDef, _OptionalContinuousDeploymentPolicyListTypeDef
 ):
     pass
 
-
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
+
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6663,21 +5059,14 @@
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
-
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,49 +55,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasICPRecordalTypeDef",
-    "AliasesOutputTypeDef",
     "AliasesTypeDef",
-    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
-    "TrustedKeyGroupsOutputTypeDef",
-    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
-    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
-    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
-    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
-    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -110,22 +102,19 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
-    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
-    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -135,29 +124,27 @@
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
-    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
-    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
@@ -180,29 +167,24 @@
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
-    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
-    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
@@ -210,255 +192,201 @@
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
-    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
     "TestFunctionRequestRequestTypeDef",
-    "CachePolicyCookiesConfigOutputTypeDef",
-    "CookiePreferenceOutputTypeDef",
-    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
-    "CachePolicyHeadersConfigOutputTypeDef",
-    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
-    "CachePolicyQueryStringsConfigOutputTypeDef",
-    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
-    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
-    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
-    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
-    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
-    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
-    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
-    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupConfigUnionTypeDef",
-    "KeyGroupTypeDef",
-    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
-    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
-    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
-    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
-    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
-    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
-    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
-    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
-    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "TagsOutputTypeDef",
     "TagsTypeDef",
-    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
-    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
-    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
-    "OriginOutputTypeDef",
     "OriginTypeDef",
-    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
-    "InvalidationBatchUnionTypeDef",
+    "InvalidationTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
-    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
-    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
-    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
-    "StreamingDistributionConfigUnionTypeDef",
+    "GetStreamingDistributionConfigResultTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagsUnionTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigOutputTypeDef",
-    "GetOriginRequestPolicyConfigResultTypeDef",
-    "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
-    "OriginRequestPolicyConfigUnionTypeDef",
+    "GetOriginRequestPolicyConfigResultTypeDef",
+    "OriginRequestPolicyTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
-    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "OriginsOutputTypeDef",
+    "KeyGroupListTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigOutputTypeDef",
-    "FieldLevelEncryptionProfileSummaryTypeDef",
     "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileSummaryTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
-    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
-    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigOutputTypeDef",
-    "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionSummaryTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
-    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
-    "CachePolicyConfigUnionTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
-    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
+    "ListKeyGroupsResultTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "FieldLevelEncryptionProfileListTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileListTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
-    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "FieldLevelEncryptionListTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionListTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigOutputTypeDef",
-    "DistributionSummaryTypeDef",
     "DistributionConfigTypeDef",
+    "DistributionSummaryTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -469,271 +397,160 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "DistributionTypeDef",
-    "GetDistributionConfigResultTypeDef",
-    "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
+    "DistributionTypeDef",
+    "GetDistributionConfigResultTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
+    "DistributionListTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
-_RequiredAliasesOutputTypeDef = TypedDict(
-    "_RequiredAliasesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalAliasesOutputTypeDef = TypedDict(
-    "_OptionalAliasesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
-    pass
-
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
-CachedMethodsOutputTypeDef = TypedDict(
-    "CachedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-    },
-)
 
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
-    "_RequiredTrustedKeyGroupsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-    },
-)
-_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
-    "_OptionalTrustedKeyGroupsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class TrustedKeyGroupsOutputTypeDef(
-    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
-):
-    pass
-
-_RequiredTrustedSignersOutputTypeDef = TypedDict(
-    "_RequiredTrustedSignersOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Quantity": int,
-    },
-)
-_OptionalTrustedSignersOutputTypeDef = TypedDict(
-    "_OptionalTrustedSignersOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class TrustedSignersOutputTypeDef(
-    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
-):
-    pass
-
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
 
+
 _RequiredTrustedSignersTypeDef = TypedDict(
     "_RequiredTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
-_RequiredCookieNamesOutputTypeDef = TypedDict(
-    "_RequiredCookieNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCookieNamesOutputTypeDef = TypedDict(
-    "_OptionalCookieNamesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class CookieNamesOutputTypeDef(
-    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
-):
-    pass
 
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
-_RequiredHeadersOutputTypeDef = TypedDict(
-    "_RequiredHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalHeadersOutputTypeDef = TypedDict(
-    "_OptionalHeadersOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
-    pass
 
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
-_RequiredQueryStringNamesOutputTypeDef = TypedDict(
-    "_RequiredQueryStringNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryStringNamesOutputTypeDef = TypedDict(
-    "_OptionalQueryStringNamesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class QueryStringNamesOutputTypeDef(
-    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
-):
-    pass
 
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -741,17 +558,19 @@
     "_OptionalQueryStringNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
+
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -786,38 +605,20 @@
     "_OptionalContentTypeProfileTypeDef",
     {
         "ProfileId": str,
     },
     total=False,
 )
 
+
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
-_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
-    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class StagingDistributionDnsNamesOutputTypeDef(
-    _RequiredStagingDistributionDnsNamesOutputTypeDef,
-    _OptionalStagingDistributionDnsNamesOutputTypeDef,
-):
-    pass
 
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -825,19 +626,21 @@
     "_OptionalStagingDistributionDnsNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
+
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
@@ -862,19 +665,21 @@
     {
         "Staging": bool,
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -901,17 +706,19 @@
     "_OptionalKeyGroupConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class KeyGroupConfigTypeDef(_RequiredKeyGroupConfigTypeDef, _OptionalKeyGroupConfigTypeDef):
     pass
 
+
 _RequiredOriginAccessControlConfigTypeDef = TypedDict(
     "_RequiredOriginAccessControlConfigTypeDef",
     {
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
@@ -921,19 +728,21 @@
     "_OptionalOriginAccessControlConfigTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class OriginAccessControlConfigTypeDef(
     _RequiredOriginAccessControlConfigTypeDef, _OptionalOriginAccessControlConfigTypeDef
 ):
     pass
 
+
 _RequiredPublicKeyConfigTypeDef = TypedDict(
     "_RequiredPublicKeyConfigTypeDef",
     {
         "CallerReference": str,
         "Name": str,
         "EncodedKey": str,
     },
@@ -942,17 +751,19 @@
     "_OptionalPublicKeyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
+
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -961,40 +772,34 @@
         "ResponsePagePath": str,
         "ResponseCode": str,
         "ErrorCachingMinTTL": int,
     },
     total=False,
 )
 
+
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
+
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
-OriginSslProtocolsOutputTypeDef = TypedDict(
-    "OriginSslProtocolsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[SslProtocolType],
-    },
-)
-
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[SslProtocolType],
+        "Items": List[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -1004,119 +809,131 @@
     "_OptionalDeleteCachePolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteCachePolicyRequestRequestTypeDef(
     _RequiredDeleteCachePolicyRequestRequestTypeDef, _OptionalDeleteCachePolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteDistributionRequestRequestTypeDef(
     _RequiredDeleteDistributionRequestRequestTypeDef,
     _OptionalDeleteDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteFieldLevelEncryptionConfigRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteFunctionRequestRequestTypeDef = TypedDict(
     "DeleteFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -1131,19 +948,21 @@
     "_OptionalDeleteKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteKeyGroupRequestRequestTypeDef(
     _RequiredDeleteKeyGroupRequestRequestTypeDef, _OptionalDeleteKeyGroupRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 
@@ -1157,59 +976,65 @@
     "_OptionalDeleteOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteOriginAccessControlRequestRequestTypeDef(
     _RequiredDeleteOriginAccessControlRequestRequestTypeDef,
     _OptionalDeleteOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteOriginRequestPolicyRequestRequestTypeDef(
     _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef,
     _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeletePublicKeyRequestRequestTypeDef(
     _RequiredDeletePublicKeyRequestRequestTypeDef, _OptionalDeletePublicKeyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "ARN": str,
     },
     total=False,
@@ -1225,59 +1050,65 @@
     "_OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredDeleteResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingDistributionRequestRequestTypeDef(
     _RequiredDeleteStreamingDistributionRequestRequestTypeDef,
     _OptionalDeleteStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFunctionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1312,37 +1143,20 @@
     {
         "NextMarker": str,
         "Items": List[str],
     },
     total=False,
 )
 
+
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
-_RequiredFieldPatternsOutputTypeDef = TypedDict(
-    "_RequiredFieldPatternsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalFieldPatternsOutputTypeDef = TypedDict(
-    "_OptionalFieldPatternsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class FieldPatternsOutputTypeDef(
-    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
-):
-    pass
 
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -1350,63 +1164,48 @@
     "_OptionalFieldPatternsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
-_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
-    "_RequiredQueryStringCacheKeysOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
-    "_OptionalQueryStringCacheKeysOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class QueryStringCacheKeysOutputTypeDef(
-    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
-):
-    pass
-
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
+
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1423,55 +1222,39 @@
     {
         "Stage": FunctionStageType,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
+
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
-_RequiredGeoRestrictionOutputTypeDef = TypedDict(
-    "_RequiredGeoRestrictionOutputTypeDef",
-    {
-        "RestrictionType": GeoRestrictionTypeType,
-        "Quantity": int,
-    },
-)
-_OptionalGeoRestrictionOutputTypeDef = TypedDict(
-    "_OptionalGeoRestrictionOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class GeoRestrictionOutputTypeDef(
-    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
-):
-    pass
 
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": Sequence[str],
+        "Items": List[str],
     },
     total=False,
 )
 
+
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
 
+
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1571,19 +1354,21 @@
     "_OptionalGetFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
+
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1591,34 +1376,14 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredKeyGroupConfigOutputTypeDef",
-    {
-        "Name": str,
-        "Items": List[str],
-    },
-)
-_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalKeyGroupConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-class KeyGroupConfigOutputTypeDef(
-    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
-):
-    pass
-
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1704,48 +1469,33 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredPathsOutputTypeDef = TypedDict(
-    "_RequiredPathsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalPathsOutputTypeDef = TypedDict(
-    "_OptionalPathsOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
-    pass
-
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
     "_OptionalPathsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class PathsTypeDef(_RequiredPathsTypeDef, _OptionalPathsTypeDef):
     pass
 
+
 InvalidationSummaryTypeDef = TypedDict(
     "InvalidationSummaryTypeDef",
     {
         "Id": str,
         "CreateTime": datetime,
         "Status": str,
     },
@@ -1761,17 +1511,19 @@
     "_OptionalKeyPairIdsTypeDef",
     {
         "Items": List[str],
     },
     total=False,
 )
 
+
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
+
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1779,19 +1531,21 @@
     "_OptionalLambdaFunctionAssociationTypeDef",
     {
         "IncludeBody": bool,
     },
     total=False,
 )
 
+
 class LambdaFunctionAssociationTypeDef(
     _RequiredLambdaFunctionAssociationTypeDef, _OptionalLambdaFunctionAssociationTypeDef
 ):
     pass
 
+
 ListCachePoliciesRequestRequestTypeDef = TypedDict(
     "ListCachePoliciesRequestRequestTypeDef",
     {
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
@@ -1829,20 +1583,22 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListConflictingAliasesRequestRequestTypeDef(
     _RequiredListConflictingAliasesRequestRequestTypeDef,
     _OptionalListConflictingAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 ListContinuousDeploymentPoliciesRequestRequestTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1859,20 +1615,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByCachePolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByCachePolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByCachePolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupId": str,
     },
 )
 _OptionalListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
@@ -1880,20 +1638,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByKeyGroupRequestRequestTypeDef(
     _RequiredListDistributionsByKeyGroupRequestRequestTypeDef,
     _OptionalListDistributionsByKeyGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     {
         "OriginRequestPolicyId": str,
     },
 )
 _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
@@ -1901,20 +1661,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 ListDistributionsByRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "RealtimeLogConfigName": str,
         "RealtimeLogConfigArn": str,
@@ -1933,20 +1695,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByWebACLIdRequestRequestTypeDef",
     {
         "WebACLId": str,
     },
 )
 _OptionalListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
@@ -1954,20 +1718,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
+
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2012,19 +1778,21 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListInvalidationsRequestRequestTypeDef(
     _RequiredListInvalidationsRequestRequestTypeDef, _OptionalListInvalidationsRequestRequestTypeDef
 ):
     pass
 
+
 ListKeyGroupsRequestRequestTypeDef = TypedDict(
     "ListKeyGroupsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -2108,27 +1876,19 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
-StatusCodesOutputTypeDef = TypedDict(
-    "StatusCodesOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[int],
-    },
-)
-
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[int],
+        "Items": List[int],
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
@@ -2145,17 +1905,19 @@
     "_OptionalOriginShieldTypeDef",
     {
         "OriginShieldRegion": str,
     },
     total=False,
 )
 
+
 class OriginShieldTypeDef(_RequiredOriginShieldTypeDef, _OptionalOriginShieldTypeDef):
     pass
 
+
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
 )
 
@@ -2172,17 +1934,19 @@
     "_OptionalPublicKeySummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class PublicKeySummaryTypeDef(_RequiredPublicKeySummaryTypeDef, _OptionalPublicKeySummaryTypeDef):
     pass
 
+
 PublishFunctionRequestRequestTypeDef = TypedDict(
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -2191,122 +1955,82 @@
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
-ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
-    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[str],
-    },
-)
-
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
-_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
-    {
-        "Items": List[str],
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
-    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-):
-    pass
-
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
+
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "SamplingRate": float,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
+
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
@@ -2362,20 +2086,22 @@
     {
         "IncludeSubdomains": bool,
         "Preload": bool,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyStrictTransportSecurityTypeDef(
     _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef,
     _OptionalResponseHeadersPolicyStrictTransportSecurityTypeDef,
 ):
     pass
 
+
 _RequiredResponseHeadersPolicyXSSProtectionTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyXSSProtectionTypeDef",
     {
         "Override": bool,
         "Protection": bool,
     },
 )
@@ -2384,20 +2110,22 @@
     {
         "ModeBlock": bool,
         "ReportUri": str,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
 ):
     pass
 
+
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
@@ -2429,17 +2157,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
@@ -2447,58 +2177,42 @@
     {
         "StagingDistributionId": str,
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
     _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
     _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAllowedMethodsOutputTypeDef = TypedDict(
-    "_RequiredAllowedMethodsOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[MethodType],
-    },
-)
-_OptionalAllowedMethodsOutputTypeDef = TypedDict(
-    "_OptionalAllowedMethodsOutputTypeDef",
-    {
-        "CachedMethods": CachedMethodsOutputTypeDef,
-    },
-    total=False,
-)
-
-class AllowedMethodsOutputTypeDef(
-    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
-):
-    pass
 
 _RequiredAllowedMethodsTypeDef = TypedDict(
     "_RequiredAllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[MethodType],
+        "Items": List[MethodType],
     },
 )
 _OptionalAllowedMethodsTypeDef = TypedDict(
     "_OptionalAllowedMethodsTypeDef",
     {
         "CachedMethods": CachedMethodsTypeDef,
     },
     total=False,
 )
 
+
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
+
 _RequiredTestFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredTestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "EventObject": BlobTypeDef,
     },
@@ -2507,76 +2221,20 @@
     "_OptionalTestFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class TestFunctionRequestRequestTypeDef(
     _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
 ):
     pass
 
-_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": CachePolicyCookieBehaviorType,
-    },
-)
-_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
-    {
-        "Cookies": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class CachePolicyCookiesConfigOutputTypeDef(
-    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
-):
-    pass
-
-_RequiredCookiePreferenceOutputTypeDef = TypedDict(
-    "_RequiredCookiePreferenceOutputTypeDef",
-    {
-        "Forward": ItemSelectionType,
-    },
-)
-_OptionalCookiePreferenceOutputTypeDef = TypedDict(
-    "_OptionalCookiePreferenceOutputTypeDef",
-    {
-        "WhitelistedNames": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class CookiePreferenceOutputTypeDef(
-    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
-):
-    pass
-
-_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
-    {
-        "Cookies": CookieNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class OriginRequestPolicyCookiesConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
-):
-    pass
 
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
@@ -2584,94 +2242,61 @@
     "_OptionalCachePolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyCookiesConfigTypeDef(
     _RequiredCachePolicyCookiesConfigTypeDef, _OptionalCachePolicyCookiesConfigTypeDef
 ):
     pass
 
+
 _RequiredCookiePreferenceTypeDef = TypedDict(
     "_RequiredCookiePreferenceTypeDef",
     {
         "Forward": ItemSelectionType,
     },
 )
 _OptionalCookiePreferenceTypeDef = TypedDict(
     "_OptionalCookiePreferenceTypeDef",
     {
         "WhitelistedNames": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class CookiePreferenceTypeDef(_RequiredCookiePreferenceTypeDef, _OptionalCookiePreferenceTypeDef):
     pass
 
+
 _RequiredOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
-_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": CachePolicyHeaderBehaviorType,
-    },
-)
-_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-    },
-    total=False,
-)
-
-class CachePolicyHeadersConfigOutputTypeDef(
-    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
-):
-    pass
-
-_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-    },
-    total=False,
-)
-
-class OriginRequestPolicyHeadersConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
-):
-    pass
 
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
@@ -2679,78 +2304,42 @@
     "_OptionalCachePolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyHeadersConfigTypeDef(
     _RequiredCachePolicyHeadersConfigTypeDef, _OptionalCachePolicyHeadersConfigTypeDef
 ):
     pass
 
+
 _RequiredOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
-_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
-    },
-)
-_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStrings": QueryStringNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class CachePolicyQueryStringsConfigOutputTypeDef(
-    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
-    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
-):
-    pass
-
-_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
-    },
-)
-_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
-    {
-        "QueryStrings": QueryStringNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
-    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
-):
-    pass
 
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
@@ -2758,39 +2347,43 @@
     "_OptionalCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyQueryStringsConfigTypeDef(
     _RequiredCachePolicyQueryStringsConfigTypeDef, _OptionalCachePolicyQueryStringsConfigTypeDef
 ):
     pass
 
+
 _RequiredOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyQueryStringsConfigTypeDef(
     _RequiredOriginRequestPolicyQueryStringsConfigTypeDef,
     _OptionalOriginRequestPolicyQueryStringsConfigTypeDef,
 ):
     pass
 
+
 _RequiredCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityTypeDef",
     {
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
@@ -2798,19 +2391,21 @@
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
+
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
+
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
@@ -2825,20 +2420,22 @@
     "_OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCloudFrontOriginAccessIdentityListTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -2849,89 +2446,76 @@
     {
         "NextMarker": str,
         "Items": List[CloudFrontOriginAccessIdentitySummaryTypeDef],
     },
     total=False,
 )
 
+
 class CloudFrontOriginAccessIdentityListTypeDef(
     _RequiredCloudFrontOriginAccessIdentityListTypeDef,
     _OptionalCloudFrontOriginAccessIdentityListTypeDef,
 ):
     pass
 
+
 ConflictingAliasesListTypeDef = TypedDict(
     "ConflictingAliasesListTypeDef",
     {
         "NextMarker": str,
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
-_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfilesOutputTypeDef",
-    {
-        "Items": List[ContentTypeProfileTypeDef],
-    },
-    total=False,
-)
-
-class ContentTypeProfilesOutputTypeDef(
-    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
-):
-    pass
-
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
     "_OptionalContentTypeProfilesTypeDef",
     {
         "Items": Sequence[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
+
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
+
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_OptionalContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "SessionStickinessConfig": SessionStickinessConfigTypeDef,
     },
     total=False,
 )
 
+
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2976,14 +2560,32 @@
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigTypeDef,
+    },
+)
+
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -2991,19 +2593,21 @@
     "_OptionalUpdateKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateKeyGroupRequestRequestTypeDef(
     _RequiredUpdateKeyGroupRequestRequestTypeDef, _OptionalUpdateKeyGroupRequestRequestTypeDef
 ):
     pass
 
+
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
@@ -3026,19 +2630,21 @@
     "_OptionalOriginAccessControlTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
     total=False,
 )
 
+
 class OriginAccessControlTypeDef(
     _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
 ):
     pass
 
+
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -3046,20 +2652,22 @@
     "_OptionalUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateOriginAccessControlRequestRequestTypeDef(
     _RequiredUpdateOriginAccessControlRequestRequestTypeDef,
     _OptionalUpdateOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
@@ -3092,115 +2700,60 @@
     "_OptionalUpdatePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
-_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
-    "_RequiredCustomErrorResponsesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
-    "_OptionalCustomErrorResponsesOutputTypeDef",
-    {
-        "Items": List[CustomErrorResponseTypeDef],
-    },
-    total=False,
-)
-
-class CustomErrorResponsesOutputTypeDef(
-    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
-):
-    pass
 
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": Sequence[CustomErrorResponseTypeDef],
+        "Items": List[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
+
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
-_RequiredCustomHeadersOutputTypeDef = TypedDict(
-    "_RequiredCustomHeadersOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCustomHeadersOutputTypeDef = TypedDict(
-    "_OptionalCustomHeadersOutputTypeDef",
-    {
-        "Items": List[OriginCustomHeaderTypeDef],
-    },
-    total=False,
-)
-
-class CustomHeadersOutputTypeDef(
-    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
-):
-    pass
 
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": Sequence[OriginCustomHeaderTypeDef],
+        "Items": List[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
+
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
-_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
-    "_RequiredCustomOriginConfigOutputTypeDef",
-    {
-        "HTTPPort": int,
-        "HTTPSPort": int,
-        "OriginProtocolPolicy": OriginProtocolPolicyType,
-    },
-)
-_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
-    "_OptionalCustomOriginConfigOutputTypeDef",
-    {
-        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
-        "OriginReadTimeout": int,
-        "OriginKeepaliveTimeout": int,
-    },
-    total=False,
-)
-
-class CustomOriginConfigOutputTypeDef(
-    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
-):
-    pass
 
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
@@ -3212,19 +2765,21 @@
         "OriginSslProtocols": OriginSslProtocolsTypeDef,
         "OriginReadTimeout": int,
         "OriginKeepaliveTimeout": int,
     },
     total=False,
 )
 
+
 class CustomOriginConfigTypeDef(
     _RequiredCustomOriginConfigTypeDef, _OptionalCustomOriginConfigTypeDef
 ):
     pass
 
+
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3249,23 +2804,14 @@
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EncryptionEntityOutputTypeDef = TypedDict(
-    "EncryptionEntityOutputTypeDef",
-    {
-        "PublicKeyId": str,
-        "ProviderId": str,
-        "FieldPatterns": FieldPatternsOutputTypeDef,
-    },
-)
-
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
@@ -3281,55 +2827,40 @@
     "_OptionalEndPointTypeDef",
     {
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
     },
     total=False,
 )
 
+
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
-_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
-    "_RequiredFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
-    "_OptionalFunctionAssociationsOutputTypeDef",
-    {
-        "Items": List[FunctionAssociationTypeDef],
-    },
-    total=False,
-)
-
-class FunctionAssociationsOutputTypeDef(
-    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
-):
-    pass
 
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": Sequence[FunctionAssociationTypeDef],
+        "Items": List[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
+
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
 ):
     pass
 
+
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
@@ -3338,23 +2869,18 @@
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
+
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
-RestrictionsOutputTypeDef = TypedDict(
-    "RestrictionsOutputTypeDef",
-    {
-        "GeoRestriction": GeoRestrictionOutputTypeDef,
-    },
-)
 
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
@@ -3369,20 +2895,22 @@
     "_OptionalGetDistributionRequestDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetDistributionRequestDistributionDeployedWaitTypeDef(
     _RequiredGetDistributionRequestDistributionDeployedWaitTypeDef,
     _OptionalGetDistributionRequestDistributionDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef = TypedDict(
     "_RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -3390,66 +2918,43 @@
     "_OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetInvalidationRequestInvalidationCompletedWaitTypeDef(
     _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef,
     _OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
-    },
-)
-
-InvalidationBatchOutputTypeDef = TypedDict(
-    "InvalidationBatchOutputTypeDef",
-    {
-        "Paths": PathsOutputTypeDef,
-        "CallerReference": str,
-    },
-)
 
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
@@ -3469,17 +2974,19 @@
     {
         "NextMarker": str,
         "Items": List[InvalidationSummaryTypeDef],
     },
     total=False,
 )
 
+
 class InvalidationListTypeDef(_RequiredInvalidationListTypeDef, _OptionalInvalidationListTypeDef):
     pass
 
+
 KGKeyPairIdsTypeDef = TypedDict(
     "KGKeyPairIdsTypeDef",
     {
         "KeyGroupId": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
@@ -3490,53 +2997,35 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
-_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
-    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
-    {
-        "Items": List[LambdaFunctionAssociationTypeDef],
-    },
-    total=False,
-)
-
-class LambdaFunctionAssociationsOutputTypeDef(
-    _RequiredLambdaFunctionAssociationsOutputTypeDef,
-    _OptionalLambdaFunctionAssociationsOutputTypeDef,
-):
-    pass
-
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": Sequence[LambdaFunctionAssociationTypeDef],
+        "Items": List[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
+
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
+
 ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -3559,20 +3048,22 @@
     "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
     _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
     _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
 ):
     pass
 
+
 ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -3599,46 +3090,33 @@
     {
         "NextMarker": str,
         "Items": List[OriginAccessControlSummaryTypeDef],
     },
     total=False,
 )
 
+
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
-OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
-    "OriginGroupFailoverCriteriaOutputTypeDef",
-    {
-        "StatusCodes": StatusCodesOutputTypeDef,
-    },
-)
 
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
-OriginGroupMembersOutputTypeDef = TypedDict(
-    "OriginGroupMembersOutputTypeDef",
-    {
-        "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
-    },
-)
-
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginGroupMemberTypeDef],
+        "Items": List[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -3650,35 +3128,18 @@
     {
         "NextMarker": str,
         "Items": List[PublicKeySummaryTypeDef],
     },
     total=False,
 )
 
+
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
-_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
-    "_RequiredQueryArgProfilesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
-    "_OptionalQueryArgProfilesOutputTypeDef",
-    {
-        "Items": List[QueryArgProfileTypeDef],
-    },
-    total=False,
-)
-
-class QueryArgProfilesOutputTypeDef(
-    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
-):
-    pass
 
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3686,41 +3147,18 @@
     "_OptionalQueryArgProfilesTypeDef",
     {
         "Items": Sequence[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
+
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
-_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
-        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
-        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
-        "AccessControlAllowCredentials": bool,
-        "OriginOverride": bool,
-    },
-)
-_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
-    {
-        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
-        "AccessControlMaxAgeSec": int,
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyCorsConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
-):
-    pass
 
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
@@ -3733,38 +3171,20 @@
     {
         "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
         "AccessControlMaxAgeSec": int,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
-_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
-    {
-        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-):
-    pass
 
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3772,39 +3192,21 @@
     "_OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
-_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
-    {
-        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-):
-    pass
 
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3812,20 +3214,22 @@
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
+
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -3840,48 +3244,22 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesOutputTypeDef,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "TrustedSigners": TrustedSignersTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
-_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
-    "_RequiredStreamingDistributionConfigOutputTypeDef",
-    {
-        "CallerReference": str,
-        "S3Origin": S3OriginTypeDef,
-        "Comment": str,
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "Enabled": bool,
-    },
-)
-_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
-    "_OptionalStreamingDistributionConfigOutputTypeDef",
-    {
-        "Aliases": AliasesOutputTypeDef,
-        "Logging": StreamingLoggingConfigTypeDef,
-        "PriceClass": PriceClassType,
-    },
-    total=False,
-)
-
-class StreamingDistributionConfigOutputTypeDef(
-    _RequiredStreamingDistributionConfigOutputTypeDef,
-    _OptionalStreamingDistributionConfigOutputTypeDef,
-):
-    pass
-
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -3894,64 +3272,37 @@
         "Aliases": AliasesTypeDef,
         "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
+
 class StreamingDistributionConfigTypeDef(
     _RequiredStreamingDistributionConfigTypeDef, _OptionalStreamingDistributionConfigTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
-TagsOutputTypeDef = TypedDict(
-    "TagsOutputTypeDef",
-    {
-        "Items": List[TagTypeDef],
-    },
-    total=False,
-)
-
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredForwardedValuesOutputTypeDef = TypedDict(
-    "_RequiredForwardedValuesOutputTypeDef",
-    {
-        "QueryString": bool,
-        "Cookies": CookiePreferenceOutputTypeDef,
-    },
-)
-_OptionalForwardedValuesOutputTypeDef = TypedDict(
-    "_OptionalForwardedValuesOutputTypeDef",
-    {
-        "Headers": HeadersOutputTypeDef,
-        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
-    },
-    total=False,
-)
-
-class ForwardedValuesOutputTypeDef(
-    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
-):
-    pass
-
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -3960,61 +3311,18 @@
     {
         "Headers": HeadersTypeDef,
         "QueryStringCacheKeys": QueryStringCacheKeysTypeDef,
     },
     total=False,
 )
 
-class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
-    pass
-
-_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingGzip": bool,
-        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
-    },
-)
-_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
-    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
-    {
-        "EnableAcceptEncodingBrotli": bool,
-    },
-    total=False,
-)
 
-class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
-    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
-    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
-):
+class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
-_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
-        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
-        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
-    },
-)
-_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-class OriginRequestPolicyConfigOutputTypeDef(
-    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
-):
-    pass
 
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
@@ -4025,20 +3333,22 @@
     "_OptionalParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingBrotli": bool,
     },
     total=False,
 )
 
+
 class ParametersInCacheKeyAndForwardedToOriginTypeDef(
     _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef,
     _OptionalParametersInCacheKeyAndForwardedToOriginTypeDef,
 ):
     pass
 
+
 _RequiredOriginRequestPolicyConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyConfigTypeDef",
     {
         "Name": str,
         "HeadersConfig": OriginRequestPolicyHeadersConfigTypeDef,
         "CookiesConfig": OriginRequestPolicyCookiesConfigTypeDef,
         "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigTypeDef,
@@ -4048,19 +3358,21 @@
     "_OptionalOriginRequestPolicyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyConfigTypeDef(
     _RequiredOriginRequestPolicyConfigTypeDef, _OptionalOriginRequestPolicyConfigTypeDef
 ):
     pass
 
+
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4097,52 +3409,35 @@
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredContentTypeProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenContentTypeIsUnknown": bool,
-    },
-)
-_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalContentTypeProfileConfigOutputTypeDef",
-    {
-        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
-    },
-    total=False,
-)
-
-class ContentTypeProfileConfigOutputTypeDef(
-    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
-):
-    pass
-
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
 _OptionalContentTypeProfileConfigTypeDef = TypedDict(
     "_OptionalContentTypeProfileConfigTypeDef",
     {
         "ContentTypeProfiles": ContentTypeProfilesTypeDef,
     },
     total=False,
 )
 
+
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
+
 _RequiredTrafficConfigTypeDef = TypedDict(
     "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
 _OptionalTrafficConfigTypeDef = TypedDict(
@@ -4150,17 +3445,54 @@
     {
         "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
         "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
+
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4209,39 +3541,14 @@
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredOriginOutputTypeDef = TypedDict(
-    "_RequiredOriginOutputTypeDef",
-    {
-        "Id": str,
-        "DomainName": str,
-    },
-)
-_OptionalOriginOutputTypeDef = TypedDict(
-    "_OptionalOriginOutputTypeDef",
-    {
-        "OriginPath": str,
-        "CustomHeaders": CustomHeadersOutputTypeDef,
-        "S3OriginConfig": S3OriginConfigTypeDef,
-        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
-        "ConnectionAttempts": int,
-        "ConnectionTimeout": int,
-        "OriginShield": OriginShieldTypeDef,
-        "OriginAccessControlId": str,
-    },
-    total=False,
-)
-
-class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
-    pass
-
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
@@ -4256,35 +3563,18 @@
         "ConnectionTimeout": int,
         "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
+
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
-_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
-    "_RequiredEncryptionEntitiesOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
-    "_OptionalEncryptionEntitiesOutputTypeDef",
-    {
-        "Items": List[EncryptionEntityOutputTypeDef],
-    },
-    total=False,
-)
-
-class EncryptionEntitiesOutputTypeDef(
-    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
-):
-    pass
 
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -4292,19 +3582,21 @@
     "_OptionalEncryptionEntitiesTypeDef",
     {
         "Items": Sequence[EncryptionEntityTypeDef],
     },
     total=False,
 )
 
+
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
+
 CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
         "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
@@ -4365,17 +3657,19 @@
     {
         "NextMarker": str,
         "Items": List[FunctionSummaryTypeDef],
     },
     total=False,
 )
 
+
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
+
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4397,68 +3691,32 @@
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DistributionId": str,
+        "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
-        "InvalidationBatch": InvalidationBatchOutputTypeDef,
-    },
-)
-
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
-    {
-        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
-InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4474,19 +3732,21 @@
     "_OptionalActiveTrustedKeyGroupsTypeDef",
     {
         "Items": List[KGKeyPairIdsTypeDef],
     },
     total=False,
 )
 
+
 class ActiveTrustedKeyGroupsTypeDef(
     _RequiredActiveTrustedKeyGroupsTypeDef, _OptionalActiveTrustedKeyGroupsTypeDef
 ):
     pass
 
+
 _RequiredActiveTrustedSignersTypeDef = TypedDict(
     "_RequiredActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -4494,19 +3754,21 @@
     "_OptionalActiveTrustedSignersTypeDef",
     {
         "Items": List[SignerTypeDef],
     },
     total=False,
 )
 
+
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
+
 CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
@@ -4531,23 +3793,14 @@
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OriginGroupOutputTypeDef = TypedDict(
-    "OriginGroupOutputTypeDef",
-    {
-        "Id": str,
-        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
-        "Members": OriginGroupMembersOutputTypeDef,
-    },
-)
-
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -4557,76 +3810,34 @@
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredQueryArgProfileConfigOutputTypeDef",
-    {
-        "ForwardWhenQueryArgProfileIsUnknown": bool,
-    },
-)
-_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalQueryArgProfileConfigOutputTypeDef",
-    {
-        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
-    },
-    total=False,
-)
-
-class QueryArgProfileConfigOutputTypeDef(
-    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
-):
-    pass
-
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
 _OptionalQueryArgProfileConfigTypeDef = TypedDict(
     "_OptionalQueryArgProfileConfigTypeDef",
     {
         "QueryArgProfiles": QueryArgProfilesTypeDef,
     },
     total=False,
 )
 
+
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
-_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
-        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
-        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
-        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
-        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class ResponseHeadersPolicyConfigOutputTypeDef(
-    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
-    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
-):
-    pass
 
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
@@ -4639,19 +3850,21 @@
         "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyConfigTypeDef(
     _RequiredResponseHeadersPolicyConfigTypeDef, _OptionalResponseHeadersPolicyConfigTypeDef
 ):
     pass
 
+
 _RequiredStreamingDistributionListTypeDef = TypedDict(
     "_RequiredStreamingDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -4662,38 +3875,37 @@
     {
         "NextMarker": str,
         "Items": List[StreamingDistributionSummaryTypeDef],
     },
     total=False,
 )
 
+
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamingDistributionConfigUnionTypeDef = Union[
-    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -4701,24 +3913,26 @@
     "_OptionalUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateStreamingDistributionRequestRequestTypeDef(
     _RequiredUpdateStreamingDistributionRequestRequestTypeDef,
     _OptionalUpdateStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsOutputTypeDef,
+        "Tags": TagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
@@ -4731,86 +3945,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
-TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
-_RequiredCacheBehaviorOutputTypeDef = TypedDict(
-    "_RequiredCacheBehaviorOutputTypeDef",
-    {
-        "PathPattern": str,
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-    },
-)
-_OptionalCacheBehaviorOutputTypeDef = TypedDict(
-    "_OptionalCacheBehaviorOutputTypeDef",
-    {
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
-        "AllowedMethods": AllowedMethodsOutputTypeDef,
-        "SmoothStreaming": bool,
-        "Compress": bool,
-        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
-        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
-        "FieldLevelEncryptionId": str,
-        "RealtimeLogConfigArn": str,
-        "CachePolicyId": str,
-        "OriginRequestPolicyId": str,
-        "ResponseHeadersPolicyId": str,
-        "ForwardedValues": ForwardedValuesOutputTypeDef,
-        "MinTTL": int,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-    },
-    total=False,
-)
-
-class CacheBehaviorOutputTypeDef(
-    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
-):
-    pass
-
-_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "_RequiredDefaultCacheBehaviorOutputTypeDef",
-    {
-        "TargetOriginId": str,
-        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
-    },
-)
-_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "_OptionalDefaultCacheBehaviorOutputTypeDef",
-    {
-        "TrustedSigners": TrustedSignersOutputTypeDef,
-        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
-        "AllowedMethods": AllowedMethodsOutputTypeDef,
-        "SmoothStreaming": bool,
-        "Compress": bool,
-        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
-        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
-        "FieldLevelEncryptionId": str,
-        "RealtimeLogConfigArn": str,
-        "CachePolicyId": str,
-        "OriginRequestPolicyId": str,
-        "ResponseHeadersPolicyId": str,
-        "ForwardedValues": ForwardedValuesOutputTypeDef,
-        "MinTTL": int,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-    },
-    total=False,
-)
-
-class DefaultCacheBehaviorOutputTypeDef(
-    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
-):
-    pass
-
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -4834,17 +3976,19 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
+
 class CacheBehaviorTypeDef(_RequiredCacheBehaviorTypeDef, _OptionalCacheBehaviorTypeDef):
     pass
 
+
 _RequiredDefaultCacheBehaviorTypeDef = TypedDict(
     "_RequiredDefaultCacheBehaviorTypeDef",
     {
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
 )
@@ -4867,95 +4011,71 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
+
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
-_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigOutputTypeDef",
+
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigOutputTypeDef",
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": (
-            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
-        ),
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
     },
     total=False,
 )
 
-class CachePolicyConfigOutputTypeDef(
-    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
+
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
 ):
     pass
 
+
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+    },
+)
+
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
-    },
-)
-
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
-    {
-        "Name": str,
-        "MinTTL": int,
-    },
-)
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
-    {
-        "Comment": str,
-        "DefaultTTL": int,
-        "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
-    },
-    total=False,
-)
-
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
-):
-    pass
-
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
-OriginRequestPolicyConfigUnionTypeDef = Union[
-    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4963,40 +4083,21 @@
     "_OptionalUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
-        "Enabled": bool,
-    },
-)
-_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
-    {
-        "TrafficConfig": TrafficConfigTypeDef,
-    },
-    total=False,
-)
-
-class ContinuousDeploymentPolicyConfigOutputTypeDef(
-    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
-    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
-):
-    pass
 
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
@@ -5005,102 +4106,99 @@
     "_OptionalContinuousDeploymentPolicyConfigTypeDef",
     {
         "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
+
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
-OriginsOutputTypeDef = TypedDict(
-    "OriginsOutputTypeDef",
+
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
     {
+        "MaxItems": int,
         "Quantity": int,
-        "Items": List[OriginOutputTypeDef],
     },
 )
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
+
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": Sequence[OriginTypeDef],
+        "Items": List[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionProfileConfigOutputTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
+
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
 ):
     pass
 
+
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Name": str,
-        "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
-    },
-)
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
-    {
-        "Comment": str,
-    },
-    total=False,
-)
-
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
-):
-    pass
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5127,19 +4225,21 @@
     {
         "Items": List[RealtimeLogConfigTypeDef],
         "NextMarker": str,
     },
     total=False,
 )
 
+
 class RealtimeLogConfigsTypeDef(
     _RequiredRealtimeLogConfigsTypeDef, _OptionalRealtimeLogConfigsTypeDef
 ):
     pass
 
+
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5156,33 +4256,14 @@
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
-
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5200,159 +4281,123 @@
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
-_RequiredOriginGroupsOutputTypeDef = TypedDict(
-    "_RequiredOriginGroupsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalOriginGroupsOutputTypeDef = TypedDict(
-    "_OptionalOriginGroupsOutputTypeDef",
-    {
-        "Items": List[OriginGroupOutputTypeDef],
-    },
-    total=False,
-)
-
-class OriginGroupsOutputTypeDef(
-    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
-):
-    pass
 
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": Sequence[OriginGroupTypeDef],
+        "Items": List[OriginGroupTypeDef],
     },
     total=False,
 )
 
+
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
-_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
+
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
     total=False,
 )
 
-class FieldLevelEncryptionConfigOutputTypeDef(
-    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
-    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
+
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
 ):
     pass
 
+
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
     total=False,
 )
 
+
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
-    {
-        "CallerReference": str,
-    },
-)
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
-        "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
-    total=False,
 )
 
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
-):
-    pass
-
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
-    },
-)
-
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
-    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
-ResponseHeadersPolicyConfigUnionTypeDef = Union[
-    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5360,20 +4405,22 @@
     "_OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5381,68 +4428,80 @@
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
-_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
-    "_RequiredCacheBehaviorsOutputTypeDef",
-    {
-        "Quantity": int,
-    },
-)
-_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
-    "_OptionalCacheBehaviorsOutputTypeDef",
-    {
-        "Items": List[CacheBehaviorOutputTypeDef],
-    },
-    total=False,
-)
-
-class CacheBehaviorsOutputTypeDef(
-    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
-):
-    pass
-
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": Sequence[CacheBehaviorTypeDef],
+        "Items": List[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
+
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
+
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
+
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5471,67 +4530,36 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
-ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
-    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-]
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -5542,69 +4570,55 @@
     "_OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-FieldLevelEncryptionProfileTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
-    },
-)
 
-GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
-    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
-        "ETag": str,
+        "KeyGroupList": KeyGroupListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+
+FieldLevelEncryptionProfileTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
-    total=False,
 )
 
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
-):
-    pass
-
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
+    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
-    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -5612,32 +4626,49 @@
     "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-ListRealtimeLogConfigsResultTypeDef = TypedDict(
-    "ListRealtimeLogConfigsResultTypeDef",
+
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+    },
+    total=False,
+)
 
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
+
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+):
+    pass
+
+
+ListRealtimeLogConfigsResultTypeDef = TypedDict(
+    "ListRealtimeLogConfigsResultTypeDef",
     {
-        "KeyGroupList": KeyGroupListTypeDef,
+        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
@@ -5672,84 +4703,85 @@
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+    },
+)
+
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
+_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
     },
 )
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
+_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+        "IfMatch": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+
+class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
 
-FieldLevelEncryptionConfigUnionTypeDef = Union[
-    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-]
-_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
     },
     total=False,
 )
 
-class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
 ):
     pass
 
+
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5778,123 +4810,91 @@
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDistributionConfigOutputTypeDef = TypedDict(
-    "_RequiredDistributionConfigOutputTypeDef",
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigOutputTypeDef = TypedDict(
-    "_OptionalDistributionConfigOutputTypeDef",
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
     {
-        "Aliases": AliasesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
-class DistributionConfigOutputTypeDef(
-    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
+
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
 ):
     pass
 
+
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesOutputTypeDef,
-        "Origins": OriginsOutputTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
-        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Aliases": AliasesTypeDef,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsOutputTypeDef,
+        "Restrictions": RestrictionsTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsOutputTypeDef,
+        "OriginGroups": OriginGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
+
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
-    {
-        "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "Comment": str,
-        "Enabled": bool,
-    },
-)
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
-    {
-        "Aliases": AliasesTypeDef,
-        "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
-        "Logging": LoggingConfigTypeDef,
-        "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
-        "WebACLId": str,
-        "HttpVersion": HttpVersionType,
-        "IsIPV6Enabled": bool,
-        "ContinuousDeploymentPolicyId": str,
-        "Staging": bool,
-    },
-    total=False,
-)
-
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
-):
-    pass
 
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
@@ -5940,19 +4940,21 @@
     {
         "NextMarker": str,
         "Items": List[OriginRequestPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class OriginRequestPolicyListTypeDef(
     _RequiredOriginRequestPolicyListTypeDef, _OptionalOriginRequestPolicyListTypeDef
 ):
     pass
 
+
 ContinuousDeploymentPolicySummaryTypeDef = TypedDict(
     "ContinuousDeploymentPolicySummaryTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
     },
 )
 
@@ -6068,53 +5070,95 @@
     {
         "NextMarker": str,
         "Items": List[ResponseHeadersPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
+
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
+
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
+
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
+
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigOutputTypeDef,
+        "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+
+class UpdateDistributionRequestRequestTypeDef(
+    _RequiredUpdateDistributionRequestRequestTypeDef,
+    _OptionalUpdateDistributionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredDistributionListTypeDef = TypedDict(
     "_RequiredDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -6125,53 +5169,18 @@
     {
         "NextMarker": str,
         "Items": List[DistributionSummaryTypeDef],
     },
     total=False,
 )
 
+
 class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
     pass
 
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-
-_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-class UpdateDistributionRequestRequestTypeDef(
-    _RequiredUpdateDistributionRequestRequestTypeDef,
-    _OptionalUpdateDistributionRequestRequestTypeDef,
-):
-    pass
 
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
     },
@@ -6181,17 +5190,19 @@
     {
         "NextMarker": str,
         "Items": List[CachePolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
+
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6208,27 +5219,36 @@
     {
         "NextMarker": str,
         "Items": List[ContinuousDeploymentPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class ContinuousDeploymentPolicyListTypeDef(
     _RequiredContinuousDeploymentPolicyListTypeDef, _OptionalContinuousDeploymentPolicyListTypeDef
 ):
     pass
 
+
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
+
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6302,21 +5322,14 @@
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
-
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.py` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.pyi` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-2.5.2.post2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

