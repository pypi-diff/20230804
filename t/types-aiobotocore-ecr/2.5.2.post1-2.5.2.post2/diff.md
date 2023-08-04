# Comparing `tmp/types-aiobotocore-ecr-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ecr-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:49 2023, max compression
```

## Comparing `types-aiobotocore-ecr-2.5.2.post1.tar` & `types-aiobotocore-ecr-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.297595 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35749 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35691 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-08-02 14:37:52.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-08-02 14:37:52.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.964049 types-aiobotocore-ecr-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-08-04 12:00:49.964049 types-aiobotocore-ecr-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:49.964049 types-aiobotocore-ecr-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35705 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35647 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-08-04 11:45:18.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-08-04 11:45:18.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51943 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51870 2023-08-04 11:45:18.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-04 11:45:17.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.964049 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-2.5.2.post1/LICENSE` & `types-aiobotocore-ecr-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/setup.py` & `types-aiobotocore-ecr-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__main__.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECR 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ECR 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleUnionTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    RegistryScanningRuleTypeDef,
+    ReplicationConfigurationTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -576,28 +576,25 @@
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_policy)
         """
 
     async def put_registry_scanning_configuration(
-        self,
-        *,
-        scanType: ScanTypeType = ...,
-        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
+        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_scanning_configuration)
         """
 
     async def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
+        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_replication_configuration)
         """
```

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleUnionTypeDef,
-    ReplicationConfigurationUnionTypeDef,
+    RegistryScanningRuleTypeDef,
+    ReplicationConfigurationTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -535,27 +535,24 @@
         """
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_policy)
         """
     async def put_registry_scanning_configuration(
-        self,
-        *,
-        scanType: ScanTypeType = ...,
-        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
+        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_scanning_configuration)
         """
     async def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
+        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_replication_configuration)
         """
```

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,42 +147,37 @@
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "RegistryScanningRuleOutputTypeDef",
     "RegistryScanningRuleTypeDef",
     "RepositoryScanningConfigurationTypeDef",
-    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationResponseTypeDef",
     "PutReplicationConfigurationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
+    "PutReplicationConfigurationResponseTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -1717,27 +1712,19 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-RegistryScanningRuleOutputTypeDef = TypedDict(
-    "RegistryScanningRuleOutputTypeDef",
-    {
-        "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
-    },
-)
-
 RegistryScanningRuleTypeDef = TypedDict(
     "RegistryScanningRuleTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
@@ -1745,45 +1732,24 @@
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
         "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
-    {
-        "destinations": List[ReplicationDestinationTypeDef],
-    },
-)
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
-    {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
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
-        "destinations": Sequence[ReplicationDestinationTypeDef],
+        "destinations": List[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
+        "repositoryFilters": List[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
 
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
@@ -1878,46 +1844,45 @@
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleTypeDef],
+    },
+    total=False,
+)
+
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleOutputTypeDef],
+        "rules": List[RegistryScanningRuleTypeDef],
     },
     total=False,
 )
 
-RegistryScanningRuleUnionTypeDef = Union[
-    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
-]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationOutputTypeDef = TypedDict(
-    "ReplicationConfigurationOutputTypeDef",
-    {
-        "rules": List[ReplicationRuleOutputTypeDef],
-    },
-)
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": Sequence[ReplicationRuleTypeDef],
+        "rules": List[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1952,50 +1917,38 @@
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
-    },
-    total=False,
-)
-
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "replicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
```

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -146,42 +146,37 @@
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "RegistryScanningRuleOutputTypeDef",
     "RegistryScanningRuleTypeDef",
     "RepositoryScanningConfigurationTypeDef",
-    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
-    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
-    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationResponseTypeDef",
     "PutReplicationConfigurationRequestRequestTypeDef",
-    "ReplicationConfigurationUnionTypeDef",
+    "PutReplicationConfigurationResponseTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -1646,27 +1641,19 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-RegistryScanningRuleOutputTypeDef = TypedDict(
-    "RegistryScanningRuleOutputTypeDef",
-    {
-        "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
-    },
-)
-
 RegistryScanningRuleTypeDef = TypedDict(
     "RegistryScanningRuleTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
@@ -1674,43 +1661,24 @@
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
         "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredReplicationRuleOutputTypeDef = TypedDict(
-    "_RequiredReplicationRuleOutputTypeDef",
-    {
-        "destinations": List[ReplicationDestinationTypeDef],
-    },
-)
-_OptionalReplicationRuleOutputTypeDef = TypedDict(
-    "_OptionalReplicationRuleOutputTypeDef",
-    {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
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
-        "destinations": Sequence[ReplicationDestinationTypeDef],
+        "destinations": List[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
+        "repositoryFilters": List[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
@@ -1803,46 +1771,45 @@
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleTypeDef],
+    },
+    total=False,
+)
+
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleOutputTypeDef],
+        "rules": List[RegistryScanningRuleTypeDef],
     },
     total=False,
 )
 
-RegistryScanningRuleUnionTypeDef = Union[
-    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
-]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationOutputTypeDef = TypedDict(
-    "ReplicationConfigurationOutputTypeDef",
-    {
-        "rules": List[ReplicationRuleOutputTypeDef],
-    },
-)
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": Sequence[ReplicationRuleTypeDef],
+        "rules": List[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1877,50 +1844,38 @@
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
-    },
-    total=False,
-)
-
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "replicationConfiguration": ReplicationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationUnionTypeDef = Union[
-    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
```

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.py` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.pyi` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-2.5.2.post2/types_aiobotocore_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

