# Comparing `tmp/types-aiobotocore-workspaces-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-workspaces-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-workspaces-2.5.2.post1.tar` & `types-aiobotocore-workspaces-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.373424 types-aiobotocore-workspaces-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-08-02 14:53:11.373424 types-aiobotocore-workspaces-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.373424 types-aiobotocore-workspaces-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.373424 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50872 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50790 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-08-02 14:51:23.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55981 2023-08-02 14:51:24.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55936 2023-08-02 14:51:24.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:22.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.373424 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14495 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12965 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2597 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2596 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50842 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50760 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13374 2023-08-04 13:56:20.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13372 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11220 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11210 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    53880 2023-08-04 13:56:21.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    53839 2023-08-04 13:56:20.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14495 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/LICENSE` & `types-aiobotocore-workspaces-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/setup.py` & `types-aiobotocore-workspaces-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkSpaces 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__init__.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__init__.pyi` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/__main__.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpaces 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WorkSpaces 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
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

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/client.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,27 +80,27 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesUnionTypeDef,
-    WorkspaceRequestUnionTypeDef,
+    WorkspacePropertiesTypeDef,
+    WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -246,15 +246,15 @@
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_ip_group)
         """
 
     async def create_standby_workspaces(
-        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_standby_workspaces)
         """
@@ -302,15 +302,15 @@
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspace_image)
         """
 
     async def create_workspaces(
-        self, *, Workspaces: Sequence[WorkspaceRequestUnionTypeDef]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspaces)
         """
@@ -740,15 +740,15 @@
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_creation_properties)
         """
 
     async def modify_workspace_properties(
-        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesUnionTypeDef
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/client.pyi` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -80,27 +80,27 @@
     RebootRequestTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildRequestTypeDef,
     RebuildWorkspacesResultTypeDef,
     RootStorageTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
-    StandbyWorkspaceUnionTypeDef,
+    StandbyWorkspaceTypeDef,
     StartRequestTypeDef,
     StartWorkspacesResultTypeDef,
     StopRequestTypeDef,
     StopWorkspacesResultTypeDef,
     TagTypeDef,
     TerminateRequestTypeDef,
     TerminateWorkspacesResultTypeDef,
     UserStorageTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
-    WorkspacePropertiesUnionTypeDef,
-    WorkspaceRequestUnionTypeDef,
+    WorkspacePropertiesTypeDef,
+    WorkspaceRequestTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -232,15 +232,15 @@
         """
         Creates an IP access control group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_ip_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_ip_group)
         """
     async def create_standby_workspaces(
-        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef]
+        self, *, PrimaryRegion: str, StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef]
     ) -> CreateStandbyWorkspacesResultTypeDef:
         """
         Creates a standby WorkSpace in a secondary Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_standby_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_standby_workspaces)
         """
@@ -283,15 +283,15 @@
         """
         Creates a new WorkSpace image from an existing WorkSpace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspace_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspace_image)
         """
     async def create_workspaces(
-        self, *, Workspaces: Sequence[WorkspaceRequestUnionTypeDef]
+        self, *, Workspaces: Sequence[WorkspaceRequestTypeDef]
     ) -> CreateWorkspacesResultTypeDef:
         """
         Creates one or more WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.create_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#create_workspaces)
         """
@@ -682,15 +682,15 @@
         """
         Modify the default properties used to create WorkSpaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_creation_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_creation_properties)
         """
     async def modify_workspace_properties(
-        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesUnionTypeDef
+        self, *, WorkspaceId: str, WorkspaceProperties: WorkspacePropertiesTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies the specified WorkSpace properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Client.modify_workspace_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/client/#modify_workspace_properties)
         """
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/literals.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
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
@@ -280,14 +281,15 @@
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
@@ -366,26 +368,28 @@
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

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/literals.pyi` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
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
@@ -278,14 +279,15 @@
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
@@ -364,26 +366,28 @@
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

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/paginator.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/paginator.pyi` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/type_defs.py` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
-    "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
@@ -164,15 +163,14 @@
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
@@ -196,38 +194,34 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
+    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "WorkspacePropertiesUnionTypeDef",
-    "WorkspaceRequestOutputTypeDef",
-    "WorkspaceTypeDef",
     "DescribeIpGroupsResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
-    "StandbyWorkspaceUnionTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
-    "WorkspaceRequestUnionTypeDef",
     "DescribeWorkspacesResultTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "CreateWorkspacesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
@@ -965,27 +959,14 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
-WorkspacePropertiesOutputTypeDef = TypedDict(
-    "WorkspacePropertiesOutputTypeDef",
-    {
-        "RunningMode": RunningModeType,
-        "RunningModeAutoStopTimeoutInMinutes": int,
-        "RootVolumeSizeGib": int,
-        "UserVolumeSizeGib": int,
-        "ComputeTypeName": ComputeType,
-        "Protocols": List[ProtocolType],
-    },
-    total=False,
-)
-
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1390,37 +1371,14 @@
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1798,14 +1756,37 @@
 RebuildWorkspacesRequestRequestTypeDef = TypedDict(
     "RebuildWorkspacesRequestRequestTypeDef",
     {
         "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
     },
 )
 
+WorkspaceTypeDef = TypedDict(
+    "WorkspaceTypeDef",
+    {
+        "WorkspaceId": str,
+        "DirectoryId": str,
+        "UserName": str,
+        "IpAddress": str,
+        "State": WorkspaceStateType,
+        "BundleId": str,
+        "SubnetId": str,
+        "ErrorMessage": str,
+        "ErrorCode": str,
+        "ComputerName": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesTypeDef,
+        "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
+    },
+    total=False,
+)
+
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1837,67 +1818,14 @@
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
     total=False,
 )
 
-WorkspacePropertiesUnionTypeDef = Union[
-    WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef
-]
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
-    {
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-    },
-)
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
-
-WorkspaceTypeDef = TypedDict(
-    "WorkspaceTypeDef",
-    {
-        "WorkspaceId": str,
-        "DirectoryId": str,
-        "UserName": str,
-        "IpAddress": str,
-        "State": WorkspaceStateType,
-        "BundleId": str,
-        "SubnetId": str,
-        "ErrorMessage": str,
-        "ErrorCode": str,
-        "ComputerName": str,
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "ModificationStates": List[ModificationStateTypeDef],
-        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
-    },
-    total=False,
-)
-
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1943,25 +1871,32 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
-        "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
+        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-StandbyWorkspaceUnionTypeDef = Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1980,68 +1915,59 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
     {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
     },
 )
 
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
-        "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
+        "WorkspaceRequest": WorkspaceRequestTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-WorkspaceRequestUnionTypeDef = Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesResultTypeDef = TypedDict(
-    "CreateStandbyWorkspacesResultTypeDef",
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
     {
-        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
-        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
+CreateStandbyWorkspacesResultTypeDef = TypedDict(
+    "CreateStandbyWorkspacesResultTypeDef",
     {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[StandbyWorkspaceUnionTypeDef],
+        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
+        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces/type_defs.pyi` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,14 @@
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
-    "WorkspacePropertiesOutputTypeDef",
     "AssociateConnectionAliasResultTypeDef",
     "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInResultTypeDef",
     "CreateConnectionAliasResultTypeDef",
     "CreateIpGroupResultTypeDef",
     "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
@@ -163,15 +162,14 @@
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
     "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
-    "StandbyWorkspaceOutputTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
     "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
     "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
@@ -195,38 +193,34 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
+    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "WorkspacePropertiesUnionTypeDef",
-    "WorkspaceRequestOutputTypeDef",
-    "WorkspaceTypeDef",
     "DescribeIpGroupsResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
-    "StandbyWorkspaceUnionTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
-    "WorkspaceRequestUnionTypeDef",
     "DescribeWorkspacesResultTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
     "CreateWorkspacesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
@@ -952,27 +946,14 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
-WorkspacePropertiesOutputTypeDef = TypedDict(
-    "WorkspacePropertiesOutputTypeDef",
-    {
-        "RunningMode": RunningModeType,
-        "RunningModeAutoStopTimeoutInMinutes": int,
-        "RootVolumeSizeGib": int,
-        "UserVolumeSizeGib": int,
-        "ComputeTypeName": ComputeType,
-        "Protocols": List[ProtocolType],
-    },
-    total=False,
-)
-
 AssociateConnectionAliasResultTypeDef = TypedDict(
     "AssociateConnectionAliasResultTypeDef",
     {
         "ConnectionIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1361,35 +1342,14 @@
 
 class RegisterWorkspaceDirectoryRequestRequestTypeDef(
     _RequiredRegisterWorkspaceDirectoryRequestRequestTypeDef,
     _OptionalRegisterWorkspaceDirectoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_RequiredStandbyWorkspaceOutputTypeDef",
-    {
-        "PrimaryWorkspaceId": str,
-        "DirectoryId": str,
-    },
-)
-_OptionalStandbyWorkspaceOutputTypeDef = TypedDict(
-    "_OptionalStandbyWorkspaceOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class StandbyWorkspaceOutputTypeDef(
-    _RequiredStandbyWorkspaceOutputTypeDef, _OptionalStandbyWorkspaceOutputTypeDef
-):
-    pass
-
 _RequiredStandbyWorkspaceTypeDef = TypedDict(
     "_RequiredStandbyWorkspaceTypeDef",
     {
         "PrimaryWorkspaceId": str,
         "DirectoryId": str,
     },
 )
@@ -1757,14 +1717,37 @@
 RebuildWorkspacesRequestRequestTypeDef = TypedDict(
     "RebuildWorkspacesRequestRequestTypeDef",
     {
         "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
     },
 )
 
+WorkspaceTypeDef = TypedDict(
+    "WorkspaceTypeDef",
+    {
+        "WorkspaceId": str,
+        "DirectoryId": str,
+        "UserName": str,
+        "IpAddress": str,
+        "State": WorkspaceStateType,
+        "BundleId": str,
+        "SubnetId": str,
+        "ErrorMessage": str,
+        "ErrorCode": str,
+        "ComputerName": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesTypeDef,
+        "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
+    },
+    total=False,
+)
+
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1796,65 +1779,14 @@
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
     total=False,
 )
 
-WorkspacePropertiesUnionTypeDef = Union[
-    WorkspacePropertiesTypeDef, WorkspacePropertiesOutputTypeDef
-]
-_RequiredWorkspaceRequestOutputTypeDef = TypedDict(
-    "_RequiredWorkspaceRequestOutputTypeDef",
-    {
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-    },
-)
-_OptionalWorkspaceRequestOutputTypeDef = TypedDict(
-    "_OptionalWorkspaceRequestOutputTypeDef",
-    {
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class WorkspaceRequestOutputTypeDef(
-    _RequiredWorkspaceRequestOutputTypeDef, _OptionalWorkspaceRequestOutputTypeDef
-):
-    pass
-
-WorkspaceTypeDef = TypedDict(
-    "WorkspaceTypeDef",
-    {
-        "WorkspaceId": str,
-        "DirectoryId": str,
-        "UserName": str,
-        "IpAddress": str,
-        "State": WorkspaceStateType,
-        "BundleId": str,
-        "SubnetId": str,
-        "ErrorMessage": str,
-        "ErrorCode": str,
-        "ComputerName": str,
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
-        "ModificationStates": List[ModificationStateTypeDef],
-        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
-    },
-    total=False,
-)
-
 DescribeIpGroupsResultTypeDef = TypedDict(
     "DescribeIpGroupsResultTypeDef",
     {
         "Result": List[WorkspacesIpGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1898,25 +1830,32 @@
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateStandbyWorkspacesRequestRequestTypeDef",
+    {
+        "PrimaryRegion": str,
+        "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
+    },
+)
+
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
-        "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
+        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-StandbyWorkspaceUnionTypeDef = Union[StandbyWorkspaceTypeDef, StandbyWorkspaceOutputTypeDef]
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1935,68 +1874,59 @@
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
     {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
     },
 )
 
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
-        "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
+        "WorkspaceRequest": WorkspaceRequestTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-WorkspaceRequestUnionTypeDef = Union[WorkspaceRequestTypeDef, WorkspaceRequestOutputTypeDef]
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesResultTypeDef = TypedDict(
-    "CreateStandbyWorkspacesResultTypeDef",
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
     {
-        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
-        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateStandbyWorkspacesRequestRequestTypeDef",
+CreateStandbyWorkspacesResultTypeDef = TypedDict(
+    "CreateStandbyWorkspacesResultTypeDef",
     {
-        "PrimaryRegion": str,
-        "StandbyWorkspaces": Sequence[StandbyWorkspaceUnionTypeDef],
+        "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
+        "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post1/types_aiobotocore_workspaces.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

