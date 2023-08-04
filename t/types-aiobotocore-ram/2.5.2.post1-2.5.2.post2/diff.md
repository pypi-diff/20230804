# Comparing `tmp/types-aiobotocore-ram-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ram-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ram-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-ram-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-ram-2.5.2.post1.tar` & `types-aiobotocore-ram-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.585489 types-aiobotocore-ram-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-08-02 14:52:50.585489 types-aiobotocore-ram-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.585489 types-aiobotocore-ram-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.577489 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41013 2023-08-02 14:47:19.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40948 2023-08-02 14:47:19.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:18.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.585489 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:50.000000 types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13594 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12092 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:49:48.000000 types-aiobotocore-ram-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1805 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1804 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33737 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33688 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10754 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10752 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9025 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9017 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41115 2023-08-04 13:49:53.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41050 2023-08-04 13:49:53.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13594 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:22.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ram-2.5.2.post1/LICENSE` & `types-aiobotocore-ram-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post1/setup.py` & `types-aiobotocore-ram-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ram",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RAM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__init__.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__init__.pyi` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/__main__.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RAM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.RAM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
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

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/client.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,26 +76,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RAMClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -119,15 +116,14 @@
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     UnmatchedPolicyPermissionException: Type[BotocoreClientError]
 
-
 class RAMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
     """
 
     meta: ClientMeta
@@ -136,41 +132,39 @@
     def exceptions(self) -> Exceptions:
         """
         RAMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#exceptions)
         """
-
     async def accept_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> AcceptResourceShareInvitationResponseTypeDef:
         """
         Accepts an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.accept_resource_share_invitation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#accept_resource_share_invitation)
         """
-
     async def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share)
         """
-
     async def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
@@ -179,31 +173,28 @@
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#close)
         """
-
     async def create_permission(
         self,
         *,
         name: str,
         resourceType: str,
         policyTemplate: str,
         clientToken: str = ...,
@@ -212,134 +203,125 @@
         """
         Creates a customer managed permission for a specified resource type that you can
         attach to resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_permission)
         """
-
     async def create_permission_version(
         self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
     ) -> CreatePermissionVersionResponseTypeDef:
         """
         Creates a new version of the specified customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_permission_version)
         """
-
     async def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
-        permissionArns: Sequence[str] = ...
+        permissionArns: Sequence[str] = ...,
+        sources: Sequence[str] = ...
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_resource_share)
         """
-
     async def delete_permission(
         self, *, permissionArn: str, clientToken: str = ...
     ) -> DeletePermissionResponseTypeDef:
         """
         Deletes the specified customer managed permission in the Amazon Web Services
         Region in which you call this operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_permission)
         """
-
     async def delete_permission_version(
         self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
     ) -> DeletePermissionVersionResponseTypeDef:
         """
         Deletes one version of a customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_permission_version)
         """
-
     async def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_resource_share)
         """
-
     async def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#disassociate_resource_share)
         """
-
     async def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
         Removes a managed permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#disassociate_resource_share_permission)
         """
-
     async def enable_sharing_with_aws_organization(
         self,
     ) -> EnableSharingWithAwsOrganizationResponseTypeDef:
         """
         Enables resource sharing within your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.enable_sharing_with_aws_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#enable_sharing_with_aws_organization)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#generate_presigned_url)
         """
-
     async def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
         Retrieves the contents of a managed permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_permission)
         """
-
     async def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -347,15 +329,14 @@
         """
         Retrieves the resource policies for the specified resources that you own and
         have shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_policies)
         """
-
     async def get_resource_share_associations(
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
@@ -366,30 +347,28 @@
         """
         Retrieves the lists of resources and principals that associated for resource
         shares that you own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_associations)
         """
-
     async def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_invitations)
         """
-
     async def get_resource_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
@@ -402,15 +381,14 @@
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_shares)
         """
-
     async def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
@@ -418,15 +396,14 @@
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_pending_invitation_resources)
         """
-
     async def list_permission_associations(
         self,
         *,
         permissionArn: str = ...,
         permissionVersion: int = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         resourceType: str = ...,
@@ -438,25 +415,23 @@
         """
         Lists information about the managed permission and its associations to any
         resource shares that use this managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permission_associations)
         """
-
     async def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permission_versions)
         """
-
     async def list_permissions(
         self,
         *,
         resourceType: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         permissionType: PermissionTypeFilterType = ...
@@ -464,15 +439,14 @@
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permissions)
         """
-
     async def list_principals(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
@@ -483,15 +457,14 @@
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_principals)
         """
-
     async def list_replace_permission_associations_work(
         self,
         *,
         workIds: Sequence[str] = ...,
         status: ReplacePermissionAssociationsWorkStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -499,39 +472,36 @@
         """
         Retrieves the current status of the asynchronous tasks performed by RAM when you
         perform the  ReplacePermissionAssociationsWork operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_replace_permission_associations_work)
         """
-
     async def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_share_permissions)
         """
-
     async def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_types)
         """
-
     async def list_resources(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
@@ -543,52 +513,48 @@
         """
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resources)
         """
-
     async def promote_permission_created_from_policy(
         self, *, permissionArn: str, name: str, clientToken: str = ...
     ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
         """
         When you attach a resource-based policy to a resource, RAM automatically creates
         a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
         permission that has the same IAM permissions as the original resource-based
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#promote_permission_created_from_policy)
         """
-
     async def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
         When you attach a resource-based policy to a resource, RAM automatically creates
         a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
         permission that has the same IAM permissions as the original resource-based
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#promote_resource_share_created_from_policy)
         """
-
     async def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> RejectResourceShareInvitationResponseTypeDef:
         """
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#reject_resource_share_invitation)
         """
-
     async def replace_permission_associations(
         self,
         *,
         fromPermissionArn: str,
         toPermissionArn: str,
         fromPermissionVersion: int = ...,
         clientToken: str = ...
@@ -596,117 +562,105 @@
         """
         Updates all resource shares that use a managed permission to a different managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#replace_permission_associations)
         """
-
     async def set_default_permission_version(
         self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
     ) -> SetDefaultPermissionVersionResponseTypeDef:
         """
         Designates the specified version number as the default version for the specified
         customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#set_default_permission_version)
         """
-
     async def tag_resource(
         self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
     ) -> Dict[str, Any]:
         """
         Adds the specified tag keys and values to a resource share or managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#tag_resource)
         """
-
     async def untag_resource(
         self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
     ) -> Dict[str, Any]:
         """
         Removes the specified tag key and value pairs from the specified resource share
         or managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#untag_resource)
         """
-
     async def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#update_resource_share)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_associations"]
     ) -> GetResourceShareAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_invitations"]
     ) -> GetResourceShareInvitationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_shares"]
     ) -> GetResourceSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_principals"]) -> ListPrincipalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_resources"]) -> ListResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "RAMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
         """
```

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/client.pyi` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("RAMClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InvalidClientTokenException: Type[BotocoreClientError]
     InvalidMaxResultsException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
@@ -116,14 +119,15 @@
     ServiceUnavailableException: Type[BotocoreClientError]
     TagLimitExceededException: Type[BotocoreClientError]
     TagPolicyViolationException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     UnmatchedPolicyPermissionException: Type[BotocoreClientError]
 
+
 class RAMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
     """
 
     meta: ClientMeta
@@ -132,38 +136,42 @@
     def exceptions(self) -> Exceptions:
         """
         RAMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#exceptions)
         """
+
     async def accept_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> AcceptResourceShareInvitationResponseTypeDef:
         """
         Accepts an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.accept_resource_share_invitation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#accept_resource_share_invitation)
         """
+
     async def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share)
         """
+
     async def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
@@ -172,28 +180,31 @@
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#close)
         """
+
     async def create_permission(
         self,
         *,
         name: str,
         resourceType: str,
         policyTemplate: str,
         clientToken: str = ...,
@@ -202,123 +213,136 @@
         """
         Creates a customer managed permission for a specified resource type that you can
         attach to resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_permission)
         """
+
     async def create_permission_version(
         self, *, permissionArn: str, policyTemplate: str, clientToken: str = ...
     ) -> CreatePermissionVersionResponseTypeDef:
         """
         Creates a new version of the specified customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_permission_version)
         """
+
     async def create_resource_share(
         self,
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
-        permissionArns: Sequence[str] = ...
+        permissionArns: Sequence[str] = ...,
+        sources: Sequence[str] = ...
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_resource_share)
         """
+
     async def delete_permission(
         self, *, permissionArn: str, clientToken: str = ...
     ) -> DeletePermissionResponseTypeDef:
         """
         Deletes the specified customer managed permission in the Amazon Web Services
         Region in which you call this operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_permission)
         """
+
     async def delete_permission_version(
         self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
     ) -> DeletePermissionVersionResponseTypeDef:
         """
         Deletes one version of a customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_permission_version)
         """
+
     async def delete_resource_share(
         self, *, resourceShareArn: str, clientToken: str = ...
     ) -> DeleteResourceShareResponseTypeDef:
         """
         Deletes the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.delete_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#delete_resource_share)
         """
+
     async def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#disassociate_resource_share)
         """
+
     async def disassociate_resource_share_permission(
         self, *, resourceShareArn: str, permissionArn: str, clientToken: str = ...
     ) -> DisassociateResourceSharePermissionResponseTypeDef:
         """
         Removes a managed permission from a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#disassociate_resource_share_permission)
         """
+
     async def enable_sharing_with_aws_organization(
         self,
     ) -> EnableSharingWithAwsOrganizationResponseTypeDef:
         """
         Enables resource sharing within your organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.enable_sharing_with_aws_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#enable_sharing_with_aws_organization)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#generate_presigned_url)
         """
+
     async def get_permission(
         self, *, permissionArn: str, permissionVersion: int = ...
     ) -> GetPermissionResponseTypeDef:
         """
         Retrieves the contents of a managed permission in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_permission)
         """
+
     async def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -326,14 +350,15 @@
         """
         Retrieves the resource policies for the specified resources that you own and
         have shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_policies)
         """
+
     async def get_resource_share_associations(
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
@@ -344,28 +369,30 @@
         """
         Retrieves the lists of resources and principals that associated for resource
         shares that you own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_associations)
         """
+
     async def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_invitations)
         """
+
     async def get_resource_shares(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
@@ -378,14 +405,15 @@
         """
         Retrieves details about the resource shares that you own or that are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_shares)
         """
+
     async def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
@@ -393,14 +421,15 @@
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_pending_invitation_resources)
         """
+
     async def list_permission_associations(
         self,
         *,
         permissionArn: str = ...,
         permissionVersion: int = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         resourceType: str = ...,
@@ -412,23 +441,25 @@
         """
         Lists information about the managed permission and its associations to any
         resource shares that use this managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permission_associations)
         """
+
     async def list_permission_versions(
         self, *, permissionArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListPermissionVersionsResponseTypeDef:
         """
         Lists the available versions of the specified RAM permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permission_versions)
         """
+
     async def list_permissions(
         self,
         *,
         resourceType: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         permissionType: PermissionTypeFilterType = ...
@@ -436,14 +467,15 @@
         """
         Retrieves a list of available RAM permissions that you can use for the supported
         resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_permissions)
         """
+
     async def list_principals(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
@@ -454,14 +486,15 @@
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_principals)
         """
+
     async def list_replace_permission_associations_work(
         self,
         *,
         workIds: Sequence[str] = ...,
         status: ReplacePermissionAssociationsWorkStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -469,36 +502,39 @@
         """
         Retrieves the current status of the asynchronous tasks performed by RAM when you
         perform the  ReplacePermissionAssociationsWork operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_replace_permission_associations_work)
         """
+
     async def list_resource_share_permissions(
         self, *, resourceShareArn: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListResourceSharePermissionsResponseTypeDef:
         """
         Lists the RAM permissions that are associated with a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_share_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_share_permissions)
         """
+
     async def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_types)
         """
+
     async def list_resources(
         self,
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
@@ -510,48 +546,52 @@
         """
         Lists the resources that you added to a resource share or the resources that are
         shared with you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resources)
         """
+
     async def promote_permission_created_from_policy(
         self, *, permissionArn: str, name: str, clientToken: str = ...
     ) -> PromotePermissionCreatedFromPolicyResponseTypeDef:
         """
         When you attach a resource-based policy to a resource, RAM automatically creates
         a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
         permission that has the same IAM permissions as the original resource-based
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_permission_created_from_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#promote_permission_created_from_policy)
         """
+
     async def promote_resource_share_created_from_policy(
         self, *, resourceShareArn: str
     ) -> PromoteResourceShareCreatedFromPolicyResponseTypeDef:
         """
         When you attach a resource-based policy to a resource, RAM automatically creates
         a resource share of `featureSet`= `CREATED_FROM_POLICY` with a managed
         permission that has the same IAM permissions as the original resource-based
         policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.promote_resource_share_created_from_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#promote_resource_share_created_from_policy)
         """
+
     async def reject_resource_share_invitation(
         self, *, resourceShareInvitationArn: str, clientToken: str = ...
     ) -> RejectResourceShareInvitationResponseTypeDef:
         """
         Rejects an invitation to a resource share from another Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.reject_resource_share_invitation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#reject_resource_share_invitation)
         """
+
     async def replace_permission_associations(
         self,
         *,
         fromPermissionArn: str,
         toPermissionArn: str,
         fromPermissionVersion: int = ...,
         clientToken: str = ...
@@ -559,105 +599,117 @@
         """
         Updates all resource shares that use a managed permission to a different managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#replace_permission_associations)
         """
+
     async def set_default_permission_version(
         self, *, permissionArn: str, permissionVersion: int, clientToken: str = ...
     ) -> SetDefaultPermissionVersionResponseTypeDef:
         """
         Designates the specified version number as the default version for the specified
         customer managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.set_default_permission_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#set_default_permission_version)
         """
+
     async def tag_resource(
         self, *, tags: Sequence[TagTypeDef], resourceShareArn: str = ..., resourceArn: str = ...
     ) -> Dict[str, Any]:
         """
         Adds the specified tag keys and values to a resource share or managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#tag_resource)
         """
+
     async def untag_resource(
         self, *, tagKeys: Sequence[str], resourceShareArn: str = ..., resourceArn: str = ...
     ) -> Dict[str, Any]:
         """
         Removes the specified tag key and value pairs from the specified resource share
         or managed permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#untag_resource)
         """
+
     async def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#update_resource_share)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_associations"]
     ) -> GetResourceShareAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_share_invitations"]
     ) -> GetResourceShareInvitationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_shares"]
     ) -> GetResourceSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_principals"]) -> ListPrincipalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_resources"]) -> ListResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "RAMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/)
         """
```

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/literals.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
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
@@ -187,14 +188,15 @@
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
@@ -273,26 +275,28 @@
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
@@ -461,14 +465,15 @@
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

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/literals.pyi` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
@@ -185,14 +186,15 @@
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
@@ -271,26 +273,28 @@
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
@@ -459,14 +463,15 @@
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

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/paginator.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/paginator.pyi` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/type_defs.py` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 
 class AssociateResourceShareRequestRequestTypeDef(
     _RequiredAssociateResourceShareRequestRequestTypeDef,
@@ -368,14 +369,15 @@
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
@@ -1023,14 +1025,15 @@
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "allowExternalPrincipals": bool,
         "clientToken": str,
         "permissionArns": Sequence[str],
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
```

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram/type_defs.pyi` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 class AssociateResourceShareRequestRequestTypeDef(
     _RequiredAssociateResourceShareRequestRequestTypeDef,
     _OptionalAssociateResourceShareRequestRequestTypeDef,
@@ -351,14 +352,15 @@
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
     _OptionalDisassociateResourceShareRequestRequestTypeDef,
@@ -974,14 +976,15 @@
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "allowExternalPrincipals": bool,
         "clientToken": str,
         "permissionArns": Sequence[str],
+        "sources": Sequence[str],
     },
     total=False,
 )
 
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
```

### Comparing `types-aiobotocore-ram-2.5.2.post1/types_aiobotocore_ram.egg-info/SOURCES.txt` & `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

