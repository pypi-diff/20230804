# Comparing `tmp/types-aiobotocore-datasync-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-datasync-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datasync-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-datasync-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-datasync-2.5.2.post1.tar` & `types-aiobotocore-datasync-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.657607 types-aiobotocore-datasync-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-08-02 14:52:09.653607 types-aiobotocore-datasync-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19422 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.657607 types-aiobotocore-datasync-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.653607 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47739 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47665 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-02 14:36:10.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55860 2023-08-02 14:36:12.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-08-02 14:36:11.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.653607 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:09.000000 types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.603846 types-aiobotocore-datasync-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:28.000000 types-aiobotocore-datasync-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-08-04 12:00:44.603846 types-aiobotocore-datasync-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-04 11:43:28.000000 types-aiobotocore-datasync-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.603846 types-aiobotocore-datasync-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:43:28.000000 types-aiobotocore-datasync-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.603846 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-04 11:43:29.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 11:43:29.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:43:29.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47714 2023-08-04 11:43:30.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47640 2023-08-04 11:43:29.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-08-04 11:43:30.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-04 11:43:30.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-04 11:43:30.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-04 11:43:30.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:29.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55303 2023-08-04 11:43:32.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-08-04 11:43:31.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:28.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.603846 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:44.000000 types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datasync-2.5.2.post1/LICENSE` & `types-aiobotocore-datasync-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/setup.py` & `types-aiobotocore-datasync-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datasync",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DataSync 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__init__.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__init__.pyi` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/__main__.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataSync 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DataSync 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
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

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/client.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,28 +67,28 @@
     DescribeLocationSmbResponseTypeDef,
     DescribeStorageSystemResourceMetricsResponseTypeDef,
     DescribeStorageSystemResourcesResponseTypeDef,
     DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
-    Ec2ConfigUnionTypeDef,
+    Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
     ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
     ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
-    OnPremConfigUnionTypeDef,
+    OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
     StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
@@ -198,15 +198,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
 
     async def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
-        Ec2Config: Ec2ConfigUnionTypeDef,
+        Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
     ) -> CreateLocationEfsResponseTypeDef:
         """
@@ -309,15 +309,15 @@
         """
 
     async def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
-        OnPremConfig: OnPremConfigUnionTypeDef,
+        OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
@@ -836,15 +836,15 @@
         """
 
     async def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
-        OnPremConfig: OnPremConfigUnionTypeDef = ...,
+        OnPremConfig: OnPremConfigTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates some of the parameters of a previously created location for Network File
         System (NFS) access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
```

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/client.pyi` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,28 +67,28 @@
     DescribeLocationSmbResponseTypeDef,
     DescribeStorageSystemResourceMetricsResponseTypeDef,
     DescribeStorageSystemResourcesResponseTypeDef,
     DescribeStorageSystemResponseTypeDef,
     DescribeTaskExecutionResponseTypeDef,
     DescribeTaskResponseTypeDef,
     DiscoveryServerConfigurationTypeDef,
-    Ec2ConfigUnionTypeDef,
+    Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
     ListAgentsResponseTypeDef,
     ListDiscoveryJobsResponseTypeDef,
     ListLocationsResponseTypeDef,
     ListStorageSystemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTaskExecutionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
-    OnPremConfigUnionTypeDef,
+    OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
     StartDiscoveryJobResponseTypeDef,
     StartTaskExecutionResponseTypeDef,
     TagListEntryTypeDef,
@@ -188,15 +188,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
     async def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
-        Ec2Config: Ec2ConfigUnionTypeDef,
+        Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
     ) -> CreateLocationEfsResponseTypeDef:
         """
@@ -293,15 +293,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_hdfs)
         """
     async def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
-        OnPremConfig: OnPremConfigUnionTypeDef,
+        OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationNfsResponseTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
@@ -777,15 +777,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_location_hdfs)
         """
     async def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
-        OnPremConfig: OnPremConfigUnionTypeDef = ...,
+        OnPremConfig: OnPremConfigTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates some of the parameters of a previously created location for Network File
         System (NFS) access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
```

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/literals.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/literals.pyi` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/paginator.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/paginator.pyi` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/type_defs.py` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,22 +86,20 @@
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
-    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
-    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
@@ -159,36 +157,34 @@
     "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobResponseTypeDef",
     "StartTaskExecutionResponseTypeDef",
     "ListAgentsResponseTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
     "DescribeTaskResponseTypeDef",
     "UpdateTaskRequestRequestTypeDef",
     "DescribeAgentResponseTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
-    "Ec2ConfigUnionTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
-    "OnPremConfigUnionTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
@@ -446,22 +442,14 @@
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-Ec2ConfigOutputTypeDef = TypedDict(
-    "Ec2ConfigOutputTypeDef",
-    {
-        "SubnetArn": str,
-        "SecurityGroupArns": List[str],
-    },
-)
-
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -496,21 +484,14 @@
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-OnPremConfigOutputTypeDef = TypedDict(
-    "OnPremConfigOutputTypeDef",
-    {
-        "AgentArns": List[str],
-    },
-)
-
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -1294,14 +1275,28 @@
 
 class CreateLocationEfsRequestRequestTypeDef(
     _RequiredCreateLocationEfsRequestRequestTypeDef, _OptionalCreateLocationEfsRequestRequestTypeDef
 ):
     pass
 
 
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
     },
@@ -1411,14 +1406,26 @@
 
 class CreateLocationNfsRequestRequestTypeDef(
     _RequiredCreateLocationNfsRequestRequestTypeDef, _OptionalCreateLocationNfsRequestRequestTypeDef
 ):
     pass
 
 
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigTypeDef,
+        "MountOptions": NfsMountOptionsTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationNfsRequestRequestTypeDef = TypedDict(
@@ -1684,42 +1691,14 @@
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
         "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigOutputTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-Ec2ConfigUnionTypeDef = Union[Ec2ConfigTypeDef, Ec2ConfigOutputTypeDef]
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigOutputTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OnPremConfigUnionTypeDef = Union[OnPremConfigTypeDef, OnPremConfigOutputTypeDef]
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync/type_defs.pyi` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -85,22 +85,20 @@
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
-    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
-    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
@@ -158,36 +156,34 @@
     "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobResponseTypeDef",
     "StartTaskExecutionResponseTypeDef",
     "ListAgentsResponseTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
+    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
+    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
     "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
     "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
     "DescribeTaskResponseTypeDef",
     "UpdateTaskRequestRequestTypeDef",
     "DescribeAgentResponseTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
-    "Ec2ConfigUnionTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
-    "OnPremConfigUnionTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
@@ -441,22 +437,14 @@
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-Ec2ConfigOutputTypeDef = TypedDict(
-    "Ec2ConfigOutputTypeDef",
-    {
-        "SubnetArn": str,
-        "SecurityGroupArns": List[str],
-    },
-)
-
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -491,21 +479,14 @@
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-OnPremConfigOutputTypeDef = TypedDict(
-    "OnPremConfigOutputTypeDef",
-    {
-        "AgentArns": List[str],
-    },
-)
-
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -1265,14 +1246,28 @@
 )
 
 class CreateLocationEfsRequestRequestTypeDef(
     _RequiredCreateLocationEfsRequestRequestTypeDef, _OptionalCreateLocationEfsRequestRequestTypeDef
 ):
     pass
 
+DescribeLocationEfsResponseTypeDef = TypedDict(
+    "DescribeLocationEfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
     },
@@ -1376,14 +1371,26 @@
 )
 
 class CreateLocationNfsRequestRequestTypeDef(
     _RequiredCreateLocationNfsRequestRequestTypeDef, _OptionalCreateLocationNfsRequestRequestTypeDef
 ):
     pass
 
+DescribeLocationNfsResponseTypeDef = TypedDict(
+    "DescribeLocationNfsResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigTypeDef,
+        "MountOptions": NfsMountOptionsTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationNfsRequestRequestTypeDef = TypedDict(
@@ -1633,42 +1640,14 @@
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
         "PrivateLinkConfig": PrivateLinkConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigOutputTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-Ec2ConfigUnionTypeDef = Union[Ec2ConfigTypeDef, Ec2ConfigOutputTypeDef]
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigOutputTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OnPremConfigUnionTypeDef = Union[OnPremConfigTypeDef, OnPremConfigOutputTypeDef]
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-datasync-2.5.2.post1/types_aiobotocore_datasync.egg-info/SOURCES.txt` & `types-aiobotocore-datasync-2.5.2.post2/types_aiobotocore_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

