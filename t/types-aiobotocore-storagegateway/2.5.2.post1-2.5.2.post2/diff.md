# Comparing `tmp/types-aiobotocore-storagegateway-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-storagegateway-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-storagegateway-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-storagegateway-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-storagegateway-2.5.2.post1.tar` & `types-aiobotocore-storagegateway-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71775 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71665 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    78425 2023-08-02 14:50:23.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78346 2023-08-02 14:50:23.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-storagegateway-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:38.000000 types-aiobotocore-storagegateway-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14775 2023-08-04 13:59:28.346643 types-aiobotocore-storagegateway-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13229 2023-08-04 13:54:38.000000 types-aiobotocore-storagegateway-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.346643 types-aiobotocore-storagegateway-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:54:38.000000 types-aiobotocore-storagegateway-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2809 2023-08-04 13:54:39.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2808 2023-08-04 13:54:39.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:54:39.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    71745 2023-08-04 13:54:43.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    71635 2023-08-04 13:54:39.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10909 2023-08-04 13:54:43.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10907 2023-08-04 13:54:43.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13761 2023-08-04 13:54:43.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13748 2023-08-04 13:54:43.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:39.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    76744 2023-08-04 13:54:45.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    76667 2023-08-04 13:54:44.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:38.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14775 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:28.000000 types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/LICENSE` & `types-aiobotocore-storagegateway-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/setup.py` & `types-aiobotocore-storagegateway-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-storagegateway",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.pyi` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__main__.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.StorageGateway 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -93,15 +93,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationUnionTypeDef,
+    EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,15 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsUnionTypeDef,
+    SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -257,15 +257,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -1121,15 +1121,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1273,15 +1273,15 @@
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     async def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_local_groups)
```

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.pyi` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -93,15 +93,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationUnionTypeDef,
+    EndpointNetworkConfigurationTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,15 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsUnionTypeDef,
+    SMBLocalGroupsTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -246,15 +246,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -1036,15 +1036,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1179,15 +1179,15 @@
         Controls whether the shares on an S3 File Gateway are visible in a net view or
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share_visibility)
         """
     async def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_local_groups)
```

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActiveDirectoryStatusType",
     "AvailabilityMonitorTestStatusType",
     "CaseSensitivityType",
     "DescribeTapeArchivesPaginatorName",
     "DescribeTapeRecoveryPointsPaginatorName",
     "DescribeTapesPaginatorName",
@@ -45,15 +44,14 @@
     "StorageGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActiveDirectoryStatusType = Literal[
     "ACCESS_DENIED", "DETACHED", "JOINED", "JOINING", "NETWORK_ERROR", "TIMEOUT", "UNKNOWN_ERROR"
 ]
 AvailabilityMonitorTestStatusType = Literal["COMPLETE", "FAILED", "PENDING"]
 CaseSensitivityType = Literal["CaseSensitive", "ClientSpecified"]
 DescribeTapeArchivesPaginatorName = Literal["describe_tape_archives"]
 DescribeTapeRecoveryPointsPaginatorName = Literal["describe_tape_recovery_points"]
@@ -94,14 +92,15 @@
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
@@ -197,14 +196,15 @@
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
@@ -283,26 +283,28 @@
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

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.pyi` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActiveDirectoryStatusType",
     "AvailabilityMonitorTestStatusType",
     "CaseSensitivityType",
     "DescribeTapeArchivesPaginatorName",
     "DescribeTapeRecoveryPointsPaginatorName",
     "DescribeTapesPaginatorName",
@@ -44,14 +45,15 @@
     "StorageGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActiveDirectoryStatusType = Literal[
     "ACCESS_DENIED", "DETACHED", "JOINED", "JOINING", "NETWORK_ERROR", "TIMEOUT", "UNKNOWN_ERROR"
 ]
 AvailabilityMonitorTestStatusType = Literal["COMPLETE", "FAILED", "PENDING"]
 CaseSensitivityType = Literal["CaseSensitive", "ClientSpecified"]
 DescribeTapeArchivesPaginatorName = Literal["describe_tape_archives"]
 DescribeTapeRecoveryPointsPaginatorName = Literal["describe_tape_recovery_points"]
@@ -92,14 +94,15 @@
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
@@ -195,14 +198,15 @@
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
@@ -281,26 +285,28 @@
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

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.pyi` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.py` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_storagegateway.type_defs import TagTypeDef
 
     data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -42,15 +42,14 @@
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -72,15 +71,15 @@
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
@@ -90,15 +89,14 @@
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
     "DetachVolumeInputRequestTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
     "DiskTypeDef",
-    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     "ListFileSharesInputRequestTypeDef",
@@ -117,15 +115,14 @@
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     "StartGatewayInputRequestTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
@@ -217,23 +214,24 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
@@ -242,28 +240,24 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
-    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "SMBLocalGroupsUnionTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -392,49 +386,22 @@
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
 
-_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
-    },
-)
-_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-    },
-    total=False,
-)
-
-
-class BandwidthRateLimitIntervalOutputTypeDef(
-    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
-    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
-):
-    pass
-
-
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -704,16 +671,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsOutputTypeDef = TypedDict(
-    "SMBLocalGroupsOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -956,22 +923,14 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
-EndpointNetworkConfigurationOutputTypeDef = TypedDict(
-    "EndpointNetworkConfigurationOutputTypeDef",
-    {
-        "IpAddresses": List[str],
-    },
-    total=False,
-)
-
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1260,22 +1219,14 @@
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
-    {
-        "GatewayAdmins": Sequence[str],
-    },
-    total=False,
-)
-
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
@@ -2456,22 +2407,27 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+    },
+)
+
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2656,19 +2612,27 @@
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+    },
+)
+
 DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
         "TapeARNs": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2862,17 +2826,14 @@
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointNetworkConfigurationUnionTypeDef = Union[
-    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2885,15 +2846,15 @@
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
         "Tags": List[TagTypeDef],
         "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
@@ -2947,23 +2908,14 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-    },
-)
-
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2972,22 +2924,14 @@
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-    },
-)
-
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.pyi` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_storagegateway.type_defs import TagTypeDef
 
     data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -41,15 +41,14 @@
     "AddUploadBufferInputRequestTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
     "AssignTapePoolInputRequestTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
     "AttachVolumeInputRequestTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
     "CancelRetrievalInputRequestTypeDef",
     "ChapInfoTypeDef",
     "NFSFileShareDefaultsTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -71,15 +70,15 @@
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
@@ -89,15 +88,14 @@
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
     "DetachVolumeInputRequestTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
     "DiskTypeDef",
-    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     "ListFileSharesInputRequestTypeDef",
@@ -116,15 +114,14 @@
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
     "RefreshCacheInputRequestTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
     "ResetCacheInputRequestTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     "StartGatewayInputRequestTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
@@ -216,23 +213,24 @@
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
@@ -241,28 +239,24 @@
     "ListTapesInputListTapesPaginateTypeDef",
     "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
-    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
-    "SMBLocalGroupsUnionTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -385,47 +379,22 @@
 )
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
-_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
-    },
-)
-_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-    },
-    total=False,
-)
-
-class BandwidthRateLimitIntervalOutputTypeDef(
-    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
-    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
-):
-    pass
-
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -687,16 +656,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsOutputTypeDef = TypedDict(
-    "SMBLocalGroupsOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -929,22 +898,14 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
-EndpointNetworkConfigurationOutputTypeDef = TypedDict(
-    "EndpointNetworkConfigurationOutputTypeDef",
-    {
-        "IpAddresses": List[str],
-    },
-    total=False,
-)
-
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1227,22 +1188,14 @@
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
-    {
-        "GatewayAdmins": Sequence[str],
-    },
-    total=False,
-)
-
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
@@ -2389,22 +2342,27 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+    },
+)
+
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2585,19 +2543,27 @@
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
+    },
+)
+
 DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
     "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
         "TapeARNs": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2783,17 +2749,14 @@
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointNetworkConfigurationUnionTypeDef = Union[
-    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
-]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2806,15 +2769,15 @@
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
         "Tags": List[TagTypeDef],
         "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
@@ -2868,23 +2831,14 @@
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-    },
-)
-
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2893,22 +2847,14 @@
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-    },
-)
-
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt` & `types-aiobotocore-storagegateway-2.5.2.post2/types_aiobotocore_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

