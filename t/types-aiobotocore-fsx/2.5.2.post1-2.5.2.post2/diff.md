# Comparing `tmp/types-aiobotocore-fsx-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-fsx-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fsx-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-fsx-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:56 2023, max compression
```

## Comparing `types-aiobotocore-fsx-2.5.2.post1.tar` & `types-aiobotocore-fsx-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.553582 types-aiobotocore-fsx-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-08-02 14:52:19.553582 types-aiobotocore-fsx-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21058 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.553582 types-aiobotocore-fsx-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.549581 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40826 2023-08-02 14:39:04.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-08-02 14:39:04.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-08-02 14:39:06.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-08-02 14:39:05.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-02 14:39:04.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-02 14:39:04.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80925 2023-08-02 14:39:07.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80828 2023-08-02 14:39:06.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:03.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.553582 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:19.000000 types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.004274 types-aiobotocore-fsx-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-08-04 12:00:55.996274 types-aiobotocore-fsx-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:56.004274 types-aiobotocore-fsx-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.996274 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40811 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40756 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-08-04 11:46:35.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-08-04 11:46:35.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79330 2023-08-04 11:46:38.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79233 2023-08-04 11:46:37.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:34.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.996274 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:55.000000 types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fsx-2.5.2.post1/LICENSE` & `types-aiobotocore-fsx-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/setup.py` & `types-aiobotocore-fsx-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fsx",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FSx 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__init__.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__init__.pyi` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/__main__.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FSx 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.FSx 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/client.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     DescribeVolumesResponseTypeDef,
     DisassociateFileSystemAliasesResponseTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
     ListTagsForResourceResponseTypeDef,
     ReleaseFileSystemNfsV3LocksResponseTypeDef,
     RestoreVolumeFromSnapshotResponseTypeDef,
-    S3DataRepositoryConfigurationUnionTypeDef,
+    S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
     UpdateDataRepositoryAssociationResponseTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
     UpdateFileCacheResponseTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
@@ -258,15 +258,15 @@
         self,
         *,
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationUnionTypeDef = ...,
+        S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
@@ -728,15 +728,15 @@
 
     async def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationUnionTypeDef = ...
+        S3: S3DataRepositoryConfigurationTypeDef = ...
     ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_data_repository_association)
```

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/client.pyi` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     DescribeVolumesResponseTypeDef,
     DisassociateFileSystemAliasesResponseTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
     ListTagsForResourceResponseTypeDef,
     ReleaseFileSystemNfsV3LocksResponseTypeDef,
     RestoreVolumeFromSnapshotResponseTypeDef,
-    S3DataRepositoryConfigurationUnionTypeDef,
+    S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
     UpdateDataRepositoryAssociationResponseTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
     UpdateFileCacheResponseTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
@@ -247,15 +247,15 @@
         self,
         *,
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationUnionTypeDef = ...,
+        S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
@@ -685,15 +685,15 @@
         """
     async def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationUnionTypeDef = ...
+        S3: S3DataRepositoryConfigurationTypeDef = ...
     ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_data_repository_association)
```

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/literals.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/literals.pyi` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/paginator.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/paginator.pyi` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/type_defs.py` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
 
     data: ActiveDirectoryBackupAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
@@ -67,24 +67,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
-    "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "LustreLogCreateConfigurationTypeDef",
@@ -117,16 +114,14 @@
     "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "LustreLogConfigurationTypeDef",
     "FileSystemEndpointTypeDef",
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LustreRootSquashConfigurationOutputTypeDef",
-    "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
@@ -146,15 +141,14 @@
     "DescribeFileSystemAliasesResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DisassociateFileSystemAliasesResponseTypeDef",
     "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "RestoreVolumeFromSnapshotResponseTypeDef",
     "UpdateFileSystemResponseTypeDef",
     "NFSDataRepositoryConfigurationTypeDef",
-    "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemLustreResponseTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
@@ -191,25 +185,23 @@
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
-    "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
-    "DataRepositoryAssociationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
-    "S3DataRepositoryConfigurationUnionTypeDef",
+    "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
@@ -219,43 +211,43 @@
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
-    "OpenZFSVolumeConfigurationTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
+    "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "VolumeTypeDef",
     "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
+    "VolumeTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
+    "CreateFileSystemFromBackupRequestRequestTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
-    "CreateFileSystemFromBackupRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
     "CopyBackupResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
 )
 
 ActiveDirectoryBackupAttributesTypeDef = TypedDict(
     "ActiveDirectoryBackupAttributesTypeDef",
@@ -295,57 +287,39 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
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
         "RetryAttempts": int,
     },
 )
 
-AutoExportPolicyOutputTypeDef = TypedDict(
-    "AutoExportPolicyOutputTypeDef",
-    {
-        "Events": List[EventTypeType],
-    },
-    total=False,
-)
-
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
-AutoImportPolicyOutputTypeDef = TypedDict(
-    "AutoImportPolicyOutputTypeDef",
-    {
-        "Events": List[EventTypeType],
-    },
-    total=False,
-)
-
 AutoImportPolicyTypeDef = TypedDict(
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
@@ -385,19 +359,17 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
-
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
-
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -411,26 +383,24 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
-
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
-        "NoSquashNids": Sequence[str],
+        "NoSquashNids": List[str],
     },
     total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
@@ -454,22 +424,20 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -477,22 +445,20 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
-
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -562,21 +528,19 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -584,86 +548,78 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
-
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -709,22 +665,20 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -769,22 +723,20 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -799,42 +751,38 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
-
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
-
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
-
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -867,44 +815,25 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-LustreRootSquashConfigurationOutputTypeDef = TypedDict(
-    "LustreRootSquashConfigurationOutputTypeDef",
-    {
-        "RootSquash": str,
-        "NoSquashNids": List[str],
-    },
-    total=False,
-)
-
-OpenZFSClientConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSClientConfigurationOutputTypeDef",
-    {
-        "Clients": str,
-        "Options": List[str],
-    },
-)
-
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
-        "Options": Sequence[str],
+        "Options": List[str],
     },
 )
 
 OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
@@ -923,22 +852,20 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -947,22 +874,20 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
-
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -1020,21 +945,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -1042,21 +965,19 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
-
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1190,35 +1111,24 @@
         "Version": Literal["NFS3"],
     },
 )
 _OptionalNFSDataRepositoryConfigurationTypeDef = TypedDict(
     "_OptionalNFSDataRepositoryConfigurationTypeDef",
     {
         "DnsIps": List[str],
-        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
+        "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
-
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
-
-S3DataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "S3DataRepositoryConfigurationOutputTypeDef",
-    {
-        "AutoImportPolicy": AutoImportPolicyOutputTypeDef,
-        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1238,21 +1148,19 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
-
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1272,21 +1180,19 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1388,22 +1294,20 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
-
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1412,22 +1316,20 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
-
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1477,22 +1379,20 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1544,22 +1444,20 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1575,22 +1473,20 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -1604,21 +1500,19 @@
         "OntapVolumeType": InputOntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
     },
     total=False,
 )
 
-
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
-
 OntapVolumeConfigurationTypeDef = TypedDict(
     "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
@@ -1695,21 +1589,19 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
-
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
-
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1757,22 +1649,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1834,22 +1724,20 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
-
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1880,25 +1768,18 @@
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
     total=False,
 )
 
-OpenZFSNfsExportOutputTypeDef = TypedDict(
-    "OpenZFSNfsExportOutputTypeDef",
-    {
-        "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
-    },
-)
-
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
-        "ClientConfigurations": Sequence[OpenZFSClientConfigurationTypeDef],
+        "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
@@ -1955,21 +1836,19 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1983,37 +1862,14 @@
         "CopyTagsToBackups": bool,
         "Aliases": List[AliasTypeDef],
         "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
     total=False,
 )
 
-DataRepositoryAssociationTypeDef = TypedDict(
-    "DataRepositoryAssociationTypeDef",
-    {
-        "AssociationId": str,
-        "ResourceARN": str,
-        "FileSystemId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
-        "FileSystemPath": str,
-        "DataRepositoryPath": str,
-        "BatchImportMetaDataOnCreate": bool,
-        "ImportedFileChunkSize": int,
-        "S3": S3DataRepositoryConfigurationOutputTypeDef,
-        "Tags": List[TagTypeDef],
-        "CreationTime": datetime,
-        "FileCacheId": str,
-        "FileCachePath": str,
-        "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "DataRepositoryPath": str,
     },
 )
@@ -2026,25 +1882,43 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+DataRepositoryAssociationTypeDef = TypedDict(
+    "DataRepositoryAssociationTypeDef",
+    {
+        "AssociationId": str,
+        "ResourceARN": str,
+        "FileSystemId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
+        "FileSystemPath": str,
+        "DataRepositoryPath": str,
+        "BatchImportMetaDataOnCreate": bool,
+        "ImportedFileChunkSize": int,
+        "S3": S3DataRepositoryConfigurationTypeDef,
+        "Tags": List[TagTypeDef],
+        "CreationTime": datetime,
+        "FileCacheId": str,
+        "FileCachePath": str,
+        "DataRepositorySubdirectories": List[str],
+        "NFS": NFSDataRepositoryConfigurationTypeDef,
+    },
+    total=False,
+)
 
-S3DataRepositoryConfigurationUnionTypeDef = Union[
-    S3DataRepositoryConfigurationTypeDef, S3DataRepositoryConfigurationOutputTypeDef
-]
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -2053,22 +1927,20 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -2078,21 +1950,19 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -2113,21 +1983,19 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
-
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2149,22 +2017,20 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
-
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2174,37 +2040,35 @@
         "ClientRequestToken": str,
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVolumeFromBackupRequestRequestTypeDef(
     _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
     _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
 ):
     pass
 
-
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
         "LogConfiguration": LustreLogConfigurationTypeDef,
-        "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
+        "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
@@ -2241,21 +2105,19 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
-
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2339,35 +2201,14 @@
     "UpdateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OpenZFSVolumeConfigurationTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationTypeDef",
-    {
-        "ParentVolumeId": str,
-        "VolumePath": str,
-        "StorageCapacityReservationGiB": int,
-        "StorageCapacityQuotaGiB": int,
-        "RecordSizeKiB": int,
-        "DataCompressionType": OpenZFSDataCompressionTypeType,
-        "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
-        "ReadOnly": bool,
-        "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
-        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
-        "RestoreToSnapshot": str,
-        "DeleteIntermediateSnaphots": bool,
-        "DeleteClonedVolumes": bool,
-    },
-    total=False,
-)
-
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
     },
 )
 _OptionalCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
@@ -2382,35 +2223,54 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "CopyTagsToSnapshots": bool,
         "ReadOnly": bool,
     },
     total=False,
 )
 
+OpenZFSVolumeConfigurationTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationTypeDef",
+    {
+        "ParentVolumeId": str,
+        "VolumePath": str,
+        "StorageCapacityReservationGiB": int,
+        "StorageCapacityQuotaGiB": int,
+        "RecordSizeKiB": int,
+        "DataCompressionType": OpenZFSDataCompressionTypeType,
+        "CopyTagsToSnapshots": bool,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
+        "ReadOnly": bool,
+        "NfsExports": List[OpenZFSNfsExportTypeDef],
+        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
+        "RestoreToSnapshot": str,
+        "DeleteIntermediateSnaphots": bool,
+        "DeleteClonedVolumes": bool,
+    },
+    total=False,
+)
+
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
@@ -2436,21 +2296,19 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2459,22 +2317,20 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
-
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
@@ -2565,33 +2421,14 @@
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeRequestRequestTypeDef",
     {
         "VolumeType": VolumeTypeType,
         "Name": str,
     },
 )
@@ -2602,21 +2439,19 @@
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2630,21 +2465,38 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
 
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
@@ -2655,21 +2507,19 @@
         "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
         "Name": str,
         "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
-
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2687,14 +2537,74 @@
     "UpdateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFileSystemFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "SecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
+        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
+        "StorageType": StorageTypeType,
+        "KmsKeyId": str,
+        "FileSystemTypeVersion": str,
+        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
+        "StorageCapacity": int,
+    },
+    total=False,
+)
+
+class CreateFileSystemFromBackupRequestRequestTypeDef(
+    _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
+    _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFileSystemRequestRequestTypeDef",
+    {
+        "FileSystemType": FileSystemTypeType,
+        "StorageCapacity": int,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFileSystemRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "StorageType": StorageTypeType,
+        "SecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
+        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
+        "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
+        "FileSystemTypeVersion": str,
+        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateFileSystemRequestRequestTypeDef(
+    _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
+):
+    pass
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
@@ -2730,19 +2640,17 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
-
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
-
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2768,78 +2676,14 @@
     "UpdateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFileSystemFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "SecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
-        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
-        "StorageType": StorageTypeType,
-        "KmsKeyId": str,
-        "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
-        "StorageCapacity": int,
-    },
-    total=False,
-)
-
-
-class CreateFileSystemFromBackupRequestRequestTypeDef(
-    _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
-    _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFileSystemRequestRequestTypeDef",
-    {
-        "FileSystemType": FileSystemTypeType,
-        "StorageCapacity": int,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFileSystemRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "StorageType": StorageTypeType,
-        "SecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
-        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
-        "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
-        "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateFileSystemRequestRequestTypeDef(
-    _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
-):
-    pass
-
-
 CopyBackupResponseTypeDef = TypedDict(
     "CopyBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx/type_defs.pyi` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
 
     data: ActiveDirectoryBackupAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
@@ -67,23 +67,22 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
-    "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "LustreLogCreateConfigurationTypeDef",
@@ -116,16 +115,14 @@
     "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "LustreLogConfigurationTypeDef",
     "FileSystemEndpointTypeDef",
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LustreRootSquashConfigurationOutputTypeDef",
-    "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
@@ -145,15 +142,14 @@
     "DescribeFileSystemAliasesResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DisassociateFileSystemAliasesResponseTypeDef",
     "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "RestoreVolumeFromSnapshotResponseTypeDef",
     "UpdateFileSystemResponseTypeDef",
     "NFSDataRepositoryConfigurationTypeDef",
-    "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemLustreResponseTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
@@ -190,25 +186,23 @@
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
-    "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
-    "DataRepositoryAssociationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
-    "S3DataRepositoryConfigurationUnionTypeDef",
+    "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
@@ -218,43 +212,43 @@
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
-    "OpenZFSVolumeConfigurationTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
+    "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "VolumeTypeDef",
     "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
+    "VolumeTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
+    "CreateFileSystemFromBackupRequestRequestTypeDef",
+    "CreateFileSystemRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
-    "CreateFileSystemFromBackupRequestRequestTypeDef",
-    "CreateFileSystemRequestRequestTypeDef",
     "CopyBackupResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
 )
 
 ActiveDirectoryBackupAttributesTypeDef = TypedDict(
     "ActiveDirectoryBackupAttributesTypeDef",
@@ -294,55 +288,41 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
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
         "RetryAttempts": int,
     },
 )
 
-AutoExportPolicyOutputTypeDef = TypedDict(
-    "AutoExportPolicyOutputTypeDef",
-    {
-        "Events": List[EventTypeType],
-    },
-    total=False,
-)
-
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
-AutoImportPolicyOutputTypeDef = TypedDict(
-    "AutoImportPolicyOutputTypeDef",
-    {
-        "Events": List[EventTypeType],
-    },
-    total=False,
-)
-
 AutoImportPolicyTypeDef = TypedDict(
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
@@ -382,17 +362,19 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
+
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
+
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -406,24 +388,26 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
+
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
-        "NoSquashNids": Sequence[str],
+        "NoSquashNids": List[str],
     },
     total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
@@ -447,20 +431,22 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
+
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -468,20 +454,22 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
+
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -551,19 +539,21 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -571,78 +561,86 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
+
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -688,20 +686,22 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -746,20 +746,22 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -774,38 +776,42 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
+
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
+
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
+
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -838,42 +844,27 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-LustreRootSquashConfigurationOutputTypeDef = TypedDict(
-    "LustreRootSquashConfigurationOutputTypeDef",
-    {
-        "RootSquash": str,
-        "NoSquashNids": List[str],
-    },
-    total=False,
-)
-
-OpenZFSClientConfigurationOutputTypeDef = TypedDict(
-    "OpenZFSClientConfigurationOutputTypeDef",
-    {
-        "Clients": str,
-        "Options": List[str],
-    },
-)
 
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
-        "Options": Sequence[str],
+        "Options": List[str],
     },
 )
 
 OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
@@ -892,20 +883,22 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -914,20 +907,22 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
+
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -985,19 +980,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -1005,19 +1002,21 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
+
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1151,32 +1150,25 @@
         "Version": Literal["NFS3"],
     },
 )
 _OptionalNFSDataRepositoryConfigurationTypeDef = TypedDict(
     "_OptionalNFSDataRepositoryConfigurationTypeDef",
     {
         "DnsIps": List[str],
-        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
+        "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
+
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
-S3DataRepositoryConfigurationOutputTypeDef = TypedDict(
-    "S3DataRepositoryConfigurationOutputTypeDef",
-    {
-        "AutoImportPolicy": AutoImportPolicyOutputTypeDef,
-        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
-    },
-    total=False,
-)
 
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
@@ -1197,19 +1189,21 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
+
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1229,19 +1223,21 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1343,20 +1339,22 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
+
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1365,20 +1363,22 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
+
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1428,20 +1428,22 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1493,20 +1495,22 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1522,20 +1526,22 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -1549,19 +1555,21 @@
         "OntapVolumeType": InputOntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
     },
     total=False,
 )
 
+
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
+
 OntapVolumeConfigurationTypeDef = TypedDict(
     "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
@@ -1638,19 +1646,21 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
+
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
+
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1698,20 +1708,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1773,20 +1785,22 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
+
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1817,25 +1831,18 @@
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
     total=False,
 )
 
-OpenZFSNfsExportOutputTypeDef = TypedDict(
-    "OpenZFSNfsExportOutputTypeDef",
-    {
-        "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
-    },
-)
-
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
-        "ClientConfigurations": Sequence[OpenZFSClientConfigurationTypeDef],
+        "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
@@ -1892,19 +1899,21 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1918,37 +1927,14 @@
         "CopyTagsToBackups": bool,
         "Aliases": List[AliasTypeDef],
         "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
     total=False,
 )
 
-DataRepositoryAssociationTypeDef = TypedDict(
-    "DataRepositoryAssociationTypeDef",
-    {
-        "AssociationId": str,
-        "ResourceARN": str,
-        "FileSystemId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
-        "FileSystemPath": str,
-        "DataRepositoryPath": str,
-        "BatchImportMetaDataOnCreate": bool,
-        "ImportedFileChunkSize": int,
-        "S3": S3DataRepositoryConfigurationOutputTypeDef,
-        "Tags": List[TagTypeDef],
-        "CreationTime": datetime,
-        "FileCacheId": str,
-        "FileCachePath": str,
-        "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "DataRepositoryPath": str,
     },
 )
@@ -1961,23 +1947,45 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-S3DataRepositoryConfigurationUnionTypeDef = Union[
-    S3DataRepositoryConfigurationTypeDef, S3DataRepositoryConfigurationOutputTypeDef
-]
+
+DataRepositoryAssociationTypeDef = TypedDict(
+    "DataRepositoryAssociationTypeDef",
+    {
+        "AssociationId": str,
+        "ResourceARN": str,
+        "FileSystemId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
+        "FileSystemPath": str,
+        "DataRepositoryPath": str,
+        "BatchImportMetaDataOnCreate": bool,
+        "ImportedFileChunkSize": int,
+        "S3": S3DataRepositoryConfigurationTypeDef,
+        "Tags": List[TagTypeDef],
+        "CreationTime": datetime,
+        "FileCacheId": str,
+        "FileCachePath": str,
+        "DataRepositorySubdirectories": List[str],
+        "NFS": NFSDataRepositoryConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -1986,20 +1994,22 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -2009,19 +2019,21 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -2042,19 +2054,21 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
+
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2076,20 +2090,22 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
+
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2099,35 +2115,37 @@
         "ClientRequestToken": str,
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVolumeFromBackupRequestRequestTypeDef(
     _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
     _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
 ):
     pass
 
+
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
         "LogConfiguration": LustreLogConfigurationTypeDef,
-        "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
+        "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
@@ -2164,19 +2182,21 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
+
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2260,35 +2280,14 @@
     "UpdateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OpenZFSVolumeConfigurationTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationTypeDef",
-    {
-        "ParentVolumeId": str,
-        "VolumePath": str,
-        "StorageCapacityReservationGiB": int,
-        "StorageCapacityQuotaGiB": int,
-        "RecordSizeKiB": int,
-        "DataCompressionType": OpenZFSDataCompressionTypeType,
-        "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
-        "ReadOnly": bool,
-        "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
-        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
-        "RestoreToSnapshot": str,
-        "DeleteIntermediateSnaphots": bool,
-        "DeleteClonedVolumes": bool,
-    },
-    total=False,
-)
-
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
     },
 )
 _OptionalCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
@@ -2303,33 +2302,56 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "CopyTagsToSnapshots": bool,
         "ReadOnly": bool,
     },
     total=False,
 )
 
+OpenZFSVolumeConfigurationTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationTypeDef",
+    {
+        "ParentVolumeId": str,
+        "VolumePath": str,
+        "StorageCapacityReservationGiB": int,
+        "StorageCapacityQuotaGiB": int,
+        "RecordSizeKiB": int,
+        "DataCompressionType": OpenZFSDataCompressionTypeType,
+        "CopyTagsToSnapshots": bool,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
+        "ReadOnly": bool,
+        "NfsExports": List[OpenZFSNfsExportTypeDef],
+        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
+        "RestoreToSnapshot": str,
+        "DeleteIntermediateSnaphots": bool,
+        "DeleteClonedVolumes": bool,
+    },
+    total=False,
+)
+
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
@@ -2355,19 +2377,21 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2376,20 +2400,22 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
+
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
@@ -2480,33 +2506,14 @@
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeRequestRequestTypeDef",
     {
         "VolumeType": VolumeTypeType,
         "Name": str,
     },
 )
@@ -2517,19 +2524,21 @@
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2543,20 +2552,41 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
@@ -2566,19 +2596,21 @@
         "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
         "Name": str,
         "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
+
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2596,14 +2628,78 @@
     "UpdateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFileSystemFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "SecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
+        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
+        "StorageType": StorageTypeType,
+        "KmsKeyId": str,
+        "FileSystemTypeVersion": str,
+        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
+        "StorageCapacity": int,
+    },
+    total=False,
+)
+
+
+class CreateFileSystemFromBackupRequestRequestTypeDef(
+    _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
+    _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFileSystemRequestRequestTypeDef",
+    {
+        "FileSystemType": FileSystemTypeType,
+        "StorageCapacity": int,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFileSystemRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "StorageType": StorageTypeType,
+        "SecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
+        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
+        "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
+        "FileSystemTypeVersion": str,
+        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateFileSystemRequestRequestTypeDef(
+    _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
+):
+    pass
+
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
@@ -2639,17 +2735,19 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
+
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2675,74 +2773,14 @@
     "UpdateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFileSystemFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "SecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
-        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
-        "StorageType": StorageTypeType,
-        "KmsKeyId": str,
-        "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
-        "StorageCapacity": int,
-    },
-    total=False,
-)
-
-class CreateFileSystemFromBackupRequestRequestTypeDef(
-    _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
-    _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFileSystemRequestRequestTypeDef",
-    {
-        "FileSystemType": FileSystemTypeType,
-        "StorageCapacity": int,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFileSystemRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "StorageType": StorageTypeType,
-        "SecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "WindowsConfiguration": CreateFileSystemWindowsConfigurationTypeDef,
-        "LustreConfiguration": CreateFileSystemLustreConfigurationTypeDef,
-        "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
-        "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateFileSystemRequestRequestTypeDef(
-    _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
-):
-    pass
-
 CopyBackupResponseTypeDef = TypedDict(
     "CopyBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fsx-2.5.2.post1/types_aiobotocore_fsx.egg-info/SOURCES.txt` & `types-aiobotocore-fsx-2.5.2.post2/types_aiobotocore_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

