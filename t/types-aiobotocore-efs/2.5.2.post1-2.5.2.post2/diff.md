# Comparing `tmp/types-aiobotocore-efs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-efs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-efs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-efs-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-efs-2.5.2.post1.tar` & `types-aiobotocore-efs-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-efs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.505594 types-aiobotocore-efs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25225 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24710 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24679 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.276061 types-aiobotocore-efs-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-08-04 12:00:50.276061 types-aiobotocore-efs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.276061 types-aiobotocore-efs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.268061 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-08-04 11:45:30.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:29.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.276061 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:50.000000 types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/LICENSE` & `types-aiobotocore-efs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/README.md` & `types-aiobotocore-efs-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-efs
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore efs type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,121 +297,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_efs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `EFS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/literals/).
+
 ```python
-from types_aiobotocore_efs.literals import (
-    DescribeFileSystemsPaginatorName,
-    DescribeMountTargetsPaginatorName,
-    DescribeTagsPaginatorName,
-    LifeCycleStateType,
-    PerformanceModeType,
-    ReplicationStatusType,
-    ResourceIdTypeType,
-    ResourceType,
-    StatusType,
-    ThroughputModeType,
-    TransitionToIARulesType,
-    TransitionToPrimaryStorageClassRulesType,
-    EFSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_efs.literals import DescribeFileSystemsPaginatorName
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_efs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EFS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/type_defs/).
+
 ```python
-from types_aiobotocore_efs.type_defs import (
-    PosixUserOutputTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    BackupPolicyTypeDef,
-    PosixUserTypeDef,
-    CreateMountTargetRequestRequestTypeDef,
-    DestinationToCreateTypeDef,
-    CreationInfoTypeDef,
-    DeleteAccessPointRequestRequestTypeDef,
-    DeleteFileSystemPolicyRequestRequestTypeDef,
-    DeleteFileSystemRequestRequestTypeDef,
-    DeleteMountTargetRequestRequestTypeDef,
-    DeleteReplicationConfigurationRequestRequestTypeDef,
-    DeleteTagsRequestRequestTypeDef,
-    DescribeAccessPointsRequestRequestTypeDef,
-    DescribeAccountPreferencesRequestRequestTypeDef,
-    ResourceIdPreferenceTypeDef,
-    DescribeBackupPolicyRequestRequestTypeDef,
-    DescribeFileSystemPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeFileSystemsRequestRequestTypeDef,
-    DescribeLifecycleConfigurationRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetsRequestRequestTypeDef,
-    MountTargetDescriptionTypeDef,
-    DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestRequestTypeDef,
-    DestinationTypeDef,
-    FileSystemSizeTypeDef,
-    LifecyclePolicyTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    PutAccountPreferencesRequestRequestTypeDef,
-    PutFileSystemPolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateFileSystemRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    MountTargetDescriptionResponseTypeDef,
-    CreateFileSystemRequestRequestTypeDef,
-    CreateTagsRequestRequestTypeDef,
-    DescribeTagsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    BackupPolicyDescriptionTypeDef,
-    PutBackupPolicyRequestRequestTypeDef,
-    PosixUserUnionTypeDef,
-    CreateReplicationConfigurationRequestRequestTypeDef,
-    RootDirectoryTypeDef,
-    DescribeAccountPreferencesResponseTypeDef,
-    PutAccountPreferencesResponseTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
-    DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseTypeDef,
-    ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseTypeDef,
-    FileSystemDescriptionTypeDef,
-    LifecycleConfigurationDescriptionTypeDef,
-    PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseTypeDef,
-    AccessPointDescriptionTypeDef,
-    CreateAccessPointRequestRequestTypeDef,
-    DescribeReplicationConfigurationsResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
-    DescribeAccessPointsResponseTypeDef,
-)
+from types_aiobotocore_efs.type_defs import PosixUserTypeDef
 
 
-def get_value() -> PosixUserOutputTypeDef:
+def get_value() -> PosixUserTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/setup.py` & `types-aiobotocore-efs-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-efs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.pyi` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__main__.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EFS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EFS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
-    PosixUserUnionTypeDef,
+    PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -138,15 +138,15 @@
 
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserUnionTypeDef = ...,
+        PosixUser: PosixUserTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.pyi` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
-    PosixUserUnionTypeDef,
+    PosixUserTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -131,15 +131,15 @@
         """
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserUnionTypeDef = ...,
+        PosixUser: PosixUserTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.pyi` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.pyi` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.py` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_efs.type_defs import PosixUserOutputTypeDef
+    from types_aiobotocore_efs.type_defs import PosixUserTypeDef
 
-    data: PosixUserOutputTypeDef = ...
+    data: PosixUserTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -33,19 +33,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "PosixUserOutputTypeDef",
+    "PosixUserTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
-    "PosixUserTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
@@ -80,15 +79,14 @@
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
-    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
@@ -103,31 +101,31 @@
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
-_RequiredPosixUserOutputTypeDef = TypedDict(
-    "_RequiredPosixUserOutputTypeDef",
+_RequiredPosixUserTypeDef = TypedDict(
+    "_RequiredPosixUserTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
-_OptionalPosixUserOutputTypeDef = TypedDict(
-    "_OptionalPosixUserOutputTypeDef",
+_OptionalPosixUserTypeDef = TypedDict(
+    "_OptionalPosixUserTypeDef",
     {
-        "SecondaryGids": List[int],
+        "SecondaryGids": Sequence[int],
     },
     total=False,
 )
 
 
-class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
+class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -149,34 +147,14 @@
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
     },
 )
 
-_RequiredPosixUserTypeDef = TypedDict(
-    "_RequiredPosixUserTypeDef",
-    {
-        "Uid": int,
-        "Gid": int,
-    },
-)
-_OptionalPosixUserTypeDef = TypedDict(
-    "_OptionalPosixUserTypeDef",
-    {
-        "SecondaryGids": Sequence[int],
-    },
-    total=False,
-)
-
-
-class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
-    pass
-
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -681,15 +659,14 @@
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
-PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
@@ -879,15 +856,15 @@
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserOutputTypeDef,
+        "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -896,15 +873,15 @@
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserOutputTypeDef,
+        "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.pyi` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_efs.type_defs import PosixUserOutputTypeDef
+    from types_aiobotocore_efs.type_defs import PosixUserTypeDef
 
-    data: PosixUserOutputTypeDef = ...
+    data: PosixUserTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -32,19 +32,18 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "PosixUserOutputTypeDef",
+    "PosixUserTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
-    "PosixUserTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
@@ -79,15 +78,14 @@
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
-    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
@@ -102,30 +100,30 @@
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
-_RequiredPosixUserOutputTypeDef = TypedDict(
-    "_RequiredPosixUserOutputTypeDef",
+_RequiredPosixUserTypeDef = TypedDict(
+    "_RequiredPosixUserTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
-_OptionalPosixUserOutputTypeDef = TypedDict(
-    "_OptionalPosixUserOutputTypeDef",
+_OptionalPosixUserTypeDef = TypedDict(
+    "_OptionalPosixUserTypeDef",
     {
-        "SecondaryGids": List[int],
+        "SecondaryGids": Sequence[int],
     },
     total=False,
 )
 
-class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
+class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -146,32 +144,14 @@
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
     },
 )
 
-_RequiredPosixUserTypeDef = TypedDict(
-    "_RequiredPosixUserTypeDef",
-    {
-        "Uid": int,
-        "Gid": int,
-    },
-)
-_OptionalPosixUserTypeDef = TypedDict(
-    "_OptionalPosixUserTypeDef",
-    {
-        "SecondaryGids": Sequence[int],
-    },
-    total=False,
-)
-
-class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
-    pass
-
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -656,15 +636,14 @@
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
-PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
@@ -850,15 +829,15 @@
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserOutputTypeDef,
+        "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -867,15 +846,15 @@
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserOutputTypeDef,
+        "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/SOURCES.txt` & `types-aiobotocore-efs-2.5.2.post2/types_aiobotocore_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

