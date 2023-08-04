# Comparing `tmp/types-aiobotocore-iam-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iam-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iam-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-iam-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:49 2023, max compression
```

## Comparing `types-aiobotocore-iam-2.5.2.post1.tar` & `types-aiobotocore-iam-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:39:58.000000 types-aiobotocore-iam-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-08-02 14:40:01.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40084 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40048 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   154892 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   154511 2023-08-02 14:40:01.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   146306 2023-08-02 14:40:06.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146091 2023-08-02 14:40:05.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.099937 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-08-04 12:24:59.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-08-04 12:24:59.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    40084 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40048 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   154916 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154535 2023-08-04 12:25:00.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   146322 2023-08-04 12:25:05.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146107 2023-08-04 12:25:04.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iam-2.5.2.post1/LICENSE` & `types-aiobotocore-iam-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/setup.py` & `types-aiobotocore-iam-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iam",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__main__.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IAM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseTypeDef,
+    AttachedPermissionsBoundaryTypeDef,
     RoleLastUsedResponseTypeDef,
     RoleTypeDef,
     ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
     UserResponseTypeDef,
 )
@@ -1588,15 +1589,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     async def get_available_subresources(self) -> Sequence[str]:
@@ -2523,15 +2524,15 @@
     role_name: Awaitable[str]
     role_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     assume_role_policy_document: Awaitable[str]
     description: Awaitable[str]
     max_session_duration: Awaitable[int]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
```

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseTypeDef,
+    AttachedPermissionsBoundaryTypeDef,
     RoleLastUsedResponseTypeDef,
     RoleTypeDef,
     ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
     UserResponseTypeDef,
 )
@@ -1382,15 +1383,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     async def get_available_subresources(self) -> Sequence[str]:
@@ -2328,15 +2329,15 @@
     role_name: Awaitable[str]
     role_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     assume_role_policy_document: Awaitable[str]
     description: Awaitable[str]
     max_session_duration: Awaitable[int]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
```

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     "ResponseMetadataTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
@@ -263,14 +262,15 @@
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     "AttachedPermissionsBoundaryResponseTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
     "CreateAccessKeyResponseTypeDef",
     "DeleteServiceLinkedRoleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
@@ -330,16 +330,14 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "UserResponseTypeDef",
-    "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
@@ -381,64 +379,66 @@
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
     "GetSSHPublicKeyResponseTypeDef",
     "UploadSSHPublicKeyResponseTypeDef",
     "GroupDetailTypeDef",
-    "UserDetailTypeDef",
     "ListEntitiesForPolicyResponseTypeDef",
     "ListMFADevicesResponseTypeDef",
     "ListOpenIDConnectProvidersResponseTypeDef",
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     "ListSAMLProvidersResponseTypeDef",
     "ListSSHPublicKeysResponseTypeDef",
     "ListServerCertificatesResponseTypeDef",
     "ServerCertificateTypeDef",
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
-    "PolicyDocumentFixedTypeDef",
+    "PolicyDocumentTypeDef",
     "StatementTypeDef",
-    "RoleTypeDef",
     "ServiceLastAccessedTypeDef",
+    "RoleTypeDef",
+    "UserDetailTypeDef",
+    "UserResponseTypeDef",
+    "UserTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
     "PolicyVersionTypeDef",
     "ResourceSpecificResultTypeDef",
+    "GetServiceLastAccessedDetailsResponseTypeDef",
     "CreateRoleResponseTypeDef",
     "CreateServiceLinkedRoleResponseTypeDef",
     "GetRoleResponseTypeDef",
     "InstanceProfileTypeDef",
     "ListRolesResponseTypeDef",
     "UpdateRoleDescriptionResponseTypeDef",
-    "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
     "CreatePolicyVersionResponseTypeDef",
     "GetPolicyVersionResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ManagedPolicyDetailTypeDef",
     "EvaluationResultTypeDef",
     "CreateInstanceProfileResponseTypeDef",
     "GetInstanceProfileResponseTypeDef",
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
     "SimulatePolicyResponseTypeDef",
     "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
 _RequiredAccessDetailTypeDef = TypedDict(
     "_RequiredAccessDetailTypeDef",
     {
@@ -622,23 +622,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
-    {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-    },
-    total=False,
-)
-
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
     total=False,
@@ -3096,14 +3087,23 @@
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
+    {
+        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
+        "PermissionsBoundaryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAccessKeyResponseTypeDef = TypedDict(
     "CreateAccessKeyResponseTypeDef",
     {
         "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3998,54 +3998,14 @@
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
 
-UserResponseTypeDef = TypedDict(
-    "UserResponseTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
-
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4833,31 +4793,14 @@
         "CreateDate": datetime,
         "GroupPolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
     total=False,
 )
 
-UserDetailTypeDef = TypedDict(
-    "UserDetailTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailTypeDef],
-        "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ListEntitiesForPolicyResponseTypeDef = TypedDict(
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
         "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
@@ -4975,16 +4918,16 @@
     "UploadSigningCertificateResponseTypeDef",
     {
         "Certificate": SigningCertificateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyDocumentFixedTypeDef = TypedDict(
-    "PolicyDocumentFixedTypeDef",
+PolicyDocumentTypeDef = TypedDict(
+    "PolicyDocumentTypeDef",
     {
         "Version": str,
         "Statement": List[PolicyDocumentStatementTypeDef],
     },
 )
 
 StatementTypeDef = TypedDict(
@@ -4994,14 +4937,40 @@
         "SourcePolicyType": PolicySourceTypeType,
         "StartPosition": PositionTypeDef,
         "EndPosition": PositionTypeDef,
     },
     total=False,
 )
 
+_RequiredServiceLastAccessedTypeDef = TypedDict(
+    "_RequiredServiceLastAccessedTypeDef",
+    {
+        "ServiceName": str,
+        "ServiceNamespace": str,
+    },
+)
+_OptionalServiceLastAccessedTypeDef = TypedDict(
+    "_OptionalServiceLastAccessedTypeDef",
+    {
+        "LastAuthenticated": datetime,
+        "LastAuthenticatedEntity": str,
+        "LastAuthenticatedRegion": str,
+        "TotalAuthenticatedEntities": int,
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+    },
+    total=False,
+)
+
+
+class ServiceLastAccessedTypeDef(
+    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
+):
+    pass
+
+
 _RequiredRoleTypeDef = TypedDict(
     "_RequiredRoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
@@ -5022,37 +4991,68 @@
 )
 
 
 class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
     pass
 
 
-_RequiredServiceLastAccessedTypeDef = TypedDict(
-    "_RequiredServiceLastAccessedTypeDef",
+UserDetailTypeDef = TypedDict(
+    "UserDetailTypeDef",
     {
-        "ServiceName": str,
-        "ServiceNamespace": str,
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "UserPolicyList": List[PolicyDetailTypeDef],
+        "GroupList": List[str],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
     },
+    total=False,
 )
-_OptionalServiceLastAccessedTypeDef = TypedDict(
-    "_OptionalServiceLastAccessedTypeDef",
+
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
-        "LastAuthenticated": datetime,
-        "LastAuthenticatedEntity": str,
-        "LastAuthenticatedRegion": str,
-        "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
+    {
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
-class ServiceLastAccessedTypeDef(
-    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
-):
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
@@ -5074,74 +5074,14 @@
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
-    {
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredVirtualMFADeviceTypeDef = TypedDict(
-    "_RequiredVirtualMFADeviceTypeDef",
-    {
-        "SerialNumber": str,
-    },
-)
-_OptionalVirtualMFADeviceTypeDef = TypedDict(
-    "_OptionalVirtualMFADeviceTypeDef",
-    {
-        "Base32StringSeed": bytes,
-        "QRCodePNG": bytes,
-        "User": UserTypeDef,
-        "EnableDate": datetime,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
-    pass
-
-
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5178,15 +5118,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyVersionTypeDef = TypedDict(
     "PolicyVersionTypeDef",
     {
-        "Document": PolicyDocumentFixedTypeDef,
+        "Document": PolicyDocumentTypeDef,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -5211,14 +5151,29 @@
 
 class ResourceSpecificResultTypeDef(
     _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
 ):
     pass
 
 
+GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseTypeDef",
+    {
+        "JobStatus": jobStatusTypeType,
+        "JobType": AccessAdvisorUsageGranularityTypeType,
+        "JobCreationDate": datetime,
+        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
+        "JobCompletionDate": datetime,
+        "IsTruncated": bool,
+        "Marker": str,
+        "Error": ErrorDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5277,47 +5232,74 @@
     "UpdateRoleDescriptionResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
-        "JobStatus": jobStatusTypeType,
-        "JobType": AccessAdvisorUsageGranularityTypeType,
-        "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
-        "JobCompletionDate": datetime,
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredVirtualMFADeviceTypeDef = TypedDict(
+    "_RequiredVirtualMFADeviceTypeDef",
+    {
+        "SerialNumber": str,
+    },
+)
+_OptionalVirtualMFADeviceTypeDef = TypedDict(
+    "_OptionalVirtualMFADeviceTypeDef",
+    {
+        "Base32StringSeed": bytes,
+        "QRCodePNG": bytes,
+        "User": UserTypeDef,
+        "EnableDate": datetime,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
+    pass
+
+
 CreatePolicyVersionResponseTypeDef = TypedDict(
     "CreatePolicyVersionResponseTypeDef",
     {
         "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5436,14 +5418,32 @@
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
     total=False,
 )
 
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
+    {
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
+    {
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     "ResponseMetadataTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
@@ -262,14 +261,15 @@
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     "AttachedPermissionsBoundaryResponseTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
     "CreateAccessKeyResponseTypeDef",
     "DeleteServiceLinkedRoleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
@@ -329,16 +329,14 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "UserResponseTypeDef",
-    "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
@@ -380,64 +378,66 @@
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
     "GetSSHPublicKeyResponseTypeDef",
     "UploadSSHPublicKeyResponseTypeDef",
     "GroupDetailTypeDef",
-    "UserDetailTypeDef",
     "ListEntitiesForPolicyResponseTypeDef",
     "ListMFADevicesResponseTypeDef",
     "ListOpenIDConnectProvidersResponseTypeDef",
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     "ListSAMLProvidersResponseTypeDef",
     "ListSSHPublicKeysResponseTypeDef",
     "ListServerCertificatesResponseTypeDef",
     "ServerCertificateTypeDef",
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
-    "PolicyDocumentFixedTypeDef",
+    "PolicyDocumentTypeDef",
     "StatementTypeDef",
-    "RoleTypeDef",
     "ServiceLastAccessedTypeDef",
+    "RoleTypeDef",
+    "UserDetailTypeDef",
+    "UserResponseTypeDef",
+    "UserTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
     "PolicyVersionTypeDef",
     "ResourceSpecificResultTypeDef",
+    "GetServiceLastAccessedDetailsResponseTypeDef",
     "CreateRoleResponseTypeDef",
     "CreateServiceLinkedRoleResponseTypeDef",
     "GetRoleResponseTypeDef",
     "InstanceProfileTypeDef",
     "ListRolesResponseTypeDef",
     "UpdateRoleDescriptionResponseTypeDef",
-    "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
     "CreatePolicyVersionResponseTypeDef",
     "GetPolicyVersionResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ManagedPolicyDetailTypeDef",
     "EvaluationResultTypeDef",
     "CreateInstanceProfileResponseTypeDef",
     "GetInstanceProfileResponseTypeDef",
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
     "SimulatePolicyResponseTypeDef",
     "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
 _RequiredAccessDetailTypeDef = TypedDict(
     "_RequiredAccessDetailTypeDef",
     {
@@ -617,23 +617,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
-    {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-    },
-    total=False,
-)
-
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
     total=False,
@@ -2981,14 +2972,23 @@
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
+    {
+        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
+        "PermissionsBoundaryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAccessKeyResponseTypeDef = TypedDict(
     "CreateAccessKeyResponseTypeDef",
     {
         "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3849,52 +3849,14 @@
 
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
-UserResponseTypeDef = TypedDict(
-    "UserResponseTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4632,31 +4594,14 @@
         "CreateDate": datetime,
         "GroupPolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
     total=False,
 )
 
-UserDetailTypeDef = TypedDict(
-    "UserDetailTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailTypeDef],
-        "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 ListEntitiesForPolicyResponseTypeDef = TypedDict(
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
         "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
@@ -4772,16 +4717,16 @@
     "UploadSigningCertificateResponseTypeDef",
     {
         "Certificate": SigningCertificateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyDocumentFixedTypeDef = TypedDict(
-    "PolicyDocumentFixedTypeDef",
+PolicyDocumentTypeDef = TypedDict(
+    "PolicyDocumentTypeDef",
     {
         "Version": str,
         "Statement": List[PolicyDocumentStatementTypeDef],
     },
 )
 
 StatementTypeDef = TypedDict(
@@ -4791,14 +4736,38 @@
         "SourcePolicyType": PolicySourceTypeType,
         "StartPosition": PositionTypeDef,
         "EndPosition": PositionTypeDef,
     },
     total=False,
 )
 
+_RequiredServiceLastAccessedTypeDef = TypedDict(
+    "_RequiredServiceLastAccessedTypeDef",
+    {
+        "ServiceName": str,
+        "ServiceNamespace": str,
+    },
+)
+_OptionalServiceLastAccessedTypeDef = TypedDict(
+    "_OptionalServiceLastAccessedTypeDef",
+    {
+        "LastAuthenticated": datetime,
+        "LastAuthenticatedEntity": str,
+        "LastAuthenticatedRegion": str,
+        "TotalAuthenticatedEntities": int,
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+    },
+    total=False,
+)
+
+class ServiceLastAccessedTypeDef(
+    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
+):
+    pass
+
 _RequiredRoleTypeDef = TypedDict(
     "_RequiredRoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
@@ -4817,36 +4786,67 @@
     },
     total=False,
 )
 
 class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
     pass
 
-_RequiredServiceLastAccessedTypeDef = TypedDict(
-    "_RequiredServiceLastAccessedTypeDef",
+UserDetailTypeDef = TypedDict(
+    "UserDetailTypeDef",
     {
-        "ServiceName": str,
-        "ServiceNamespace": str,
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "UserPolicyList": List[PolicyDetailTypeDef],
+        "GroupList": List[str],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
     },
+    total=False,
 )
-_OptionalServiceLastAccessedTypeDef = TypedDict(
-    "_OptionalServiceLastAccessedTypeDef",
+
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
-        "LastAuthenticated": datetime,
-        "LastAuthenticatedEntity": str,
-        "LastAuthenticatedRegion": str,
-        "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUserTypeDef = TypedDict(
+    "_RequiredUserTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+    },
+)
+_OptionalUserTypeDef = TypedDict(
+    "_OptionalUserTypeDef",
+    {
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-class ServiceLastAccessedTypeDef(
-    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
-):
+class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4867,72 +4867,14 @@
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
-    {
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredVirtualMFADeviceTypeDef = TypedDict(
-    "_RequiredVirtualMFADeviceTypeDef",
-    {
-        "SerialNumber": str,
-    },
-)
-_OptionalVirtualMFADeviceTypeDef = TypedDict(
-    "_OptionalVirtualMFADeviceTypeDef",
-    {
-        "Base32StringSeed": bytes,
-        "QRCodePNG": bytes,
-        "User": UserTypeDef,
-        "EnableDate": datetime,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
-    pass
-
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4969,15 +4911,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyVersionTypeDef = TypedDict(
     "PolicyVersionTypeDef",
     {
-        "Document": PolicyDocumentFixedTypeDef,
+        "Document": PolicyDocumentTypeDef,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -5000,14 +4942,29 @@
 )
 
 class ResourceSpecificResultTypeDef(
     _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
 ):
     pass
 
+GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseTypeDef",
+    {
+        "JobStatus": jobStatusTypeType,
+        "JobType": AccessAdvisorUsageGranularityTypeType,
+        "JobCreationDate": datetime,
+        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
+        "JobCompletionDate": datetime,
+        "IsTruncated": bool,
+        "Marker": str,
+        "Error": ErrorDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5064,47 +5021,72 @@
     "UpdateRoleDescriptionResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
-        "JobStatus": jobStatusTypeType,
-        "JobType": AccessAdvisorUsageGranularityTypeType,
-        "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
-        "JobCompletionDate": datetime,
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredVirtualMFADeviceTypeDef = TypedDict(
+    "_RequiredVirtualMFADeviceTypeDef",
+    {
+        "SerialNumber": str,
+    },
+)
+_OptionalVirtualMFADeviceTypeDef = TypedDict(
+    "_OptionalVirtualMFADeviceTypeDef",
+    {
+        "Base32StringSeed": bytes,
+        "QRCodePNG": bytes,
+        "User": UserTypeDef,
+        "EnableDate": datetime,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
+    pass
+
 CreatePolicyVersionResponseTypeDef = TypedDict(
     "CreatePolicyVersionResponseTypeDef",
     {
         "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5221,14 +5203,32 @@
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
     total=False,
 )
 
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
+    {
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
+    {
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.py` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.pyi` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/SOURCES.txt` & `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

