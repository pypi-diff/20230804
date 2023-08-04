# Comparing `tmp/types-aiobotocore-fms-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-fms-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-fms-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-fms-2.5.2.post1.tar` & `types-aiobotocore-fms-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.141583 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32996 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-08-02 14:38:52.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64322 2023-08-02 14:38:52.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:19.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.668262 types-aiobotocore-fms-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:00:55.668262 types-aiobotocore-fms-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.668262 types-aiobotocore-fms-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.668262 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32946 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 11:46:21.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-04 11:46:21.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-04 11:46:20.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-04 11:46:20.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-08-04 11:46:23.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59360 2023-08-04 11:46:22.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:19.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.668262 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:55.000000 types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fms-2.5.2.post1/LICENSE` & `types-aiobotocore-fms-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/setup.py` & `types-aiobotocore-fms-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fms",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.pyi` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__main__.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.FMS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeUnionTypeDef,
-    AppsListDataUnionTypeDef,
+    AdminScopeTypeDef,
+    AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -58,21 +58,21 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyUnionTypeDef,
-    ProtocolsListDataUnionTypeDef,
+    PolicyTypeDef,
+    ProtocolsListDataTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetUnionTypeDef,
+    ResourceSetTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -488,25 +488,25 @@
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     async def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_admin_account)
         """
 
     async def put_apps_list(
-        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_apps_list)
         """
@@ -519,35 +519,35 @@
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_notification_channel)
         """
 
     async def put_policy(
-        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_policy)
         """
 
     async def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_protocols_list)
         """
 
     async def put_resource_set(
-        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_resource_set)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.pyi` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeUnionTypeDef,
-    AppsListDataUnionTypeDef,
+    AdminScopeTypeDef,
+    AppsListDataTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -58,21 +58,21 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyUnionTypeDef,
-    ProtocolsListDataUnionTypeDef,
+    PolicyTypeDef,
+    ProtocolsListDataTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetUnionTypeDef,
+    ResourceSetTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -446,24 +446,24 @@
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#list_third_party_firewall_firewall_policies)
         """
     async def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_admin_account)
         """
     async def put_apps_list(
-        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_apps_list)
         """
@@ -474,33 +474,33 @@
         Designates the IAM role and Amazon Simple Notification Service (SNS) topic that
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_notification_channel)
         """
     async def put_policy(
-        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_policy)
         """
     async def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_protocols_list)
         """
     async def put_resource_set(
-        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_resource_set)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.pyi` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.pyi` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.py` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_fms.type_defs import AccountScopeOutputTypeDef
+    from types_aiobotocore_fms.type_defs import AccountScopeTypeDef
 
-    data: AccountScopeOutputTypeDef = ...
+    data: AccountScopeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -43,26 +43,21 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
-    "OrganizationalUnitScopeOutputTypeDef",
-    "PolicyTypeScopeOutputTypeDef",
-    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
-    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -82,18 +77,19 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataOutputTypeDef",
+    "ProtocolsListDataTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetOutputTypeDef",
+    "ResourceSetTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
     "ListAppsListsRequestRequestTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
@@ -130,22 +126,17 @@
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
-    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
-    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -155,14 +146,15 @@
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAppsListsRequestListAppsListsPaginateTypeDef",
@@ -172,72 +164,56 @@
     "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
-    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "GetAppsListResponseTypeDef",
-    "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
-    "AppsListDataUnionTypeDef",
+    "GetAppsListResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
-    "ProtocolsListDataUnionTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
-    "ResourceSetUnionTypeDef",
+    "PutAppsListResponseTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
-    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyResponseTypeDef",
-    "PolicyUnionTypeDef",
     "PutPolicyRequestRequestTypeDef",
+    "PutPolicyResponseTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
-AccountScopeOutputTypeDef = TypedDict(
-    "AccountScopeOutputTypeDef",
-    {
-        "Accounts": List[str],
-        "AllAccountsEnabled": bool,
-        "ExcludeSpecifiedAccounts": bool,
-    },
-    total=False,
-)
-
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": Sequence[str],
+        "Accounts": List[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -255,80 +231,51 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
-OrganizationalUnitScopeOutputTypeDef = TypedDict(
-    "OrganizationalUnitScopeOutputTypeDef",
-    {
-        "OrganizationalUnits": List[str],
-        "AllOrganizationalUnitsEnabled": bool,
-        "ExcludeSpecifiedOrganizationalUnits": bool,
-    },
-    total=False,
-)
-
-PolicyTypeScopeOutputTypeDef = TypedDict(
-    "PolicyTypeScopeOutputTypeDef",
-    {
-        "PolicyTypes": List[SecurityServiceTypeType],
-        "AllPolicyTypesEnabled": bool,
-    },
-    total=False,
-)
-
-RegionScopeOutputTypeDef = TypedDict(
-    "RegionScopeOutputTypeDef",
-    {
-        "Regions": List[str],
-        "AllRegionsEnabled": bool,
-    },
-    total=False,
-)
-
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": Sequence[str],
+        "OrganizationalUnits": List[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": Sequence[SecurityServiceTypeType],
+        "PolicyTypes": List[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": Sequence[str],
+        "Regions": List[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -589,14 +536,15 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -610,70 +558,68 @@
 
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredProtocolsListDataOutputTypeDef = TypedDict(
-    "_RequiredProtocolsListDataOutputTypeDef",
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataOutputTypeDef = TypedDict(
-    "_OptionalProtocolsListDataOutputTypeDef",
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
 
-class ProtocolsListDataOutputTypeDef(
-    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
 
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetOutputTypeDef = TypedDict(
-    "_RequiredResourceSetOutputTypeDef",
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetOutputTypeDef = TypedDict(
-    "_OptionalResourceSetOutputTypeDef",
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
 
-class ResourceSetOutputTypeDef(
-    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
-):
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
 
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
@@ -1293,62 +1239,25 @@
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
 
-AdminScopeOutputTypeDef = TypedDict(
-    "AdminScopeOutputTypeDef",
-    {
-        "AccountScope": AccountScopeOutputTypeDef,
-        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
-        "RegionScope": RegionScopeOutputTypeDef,
-        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
-    },
-    total=False,
-)
-
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
-_RequiredAppsListDataOutputTypeDef = TypedDict(
-    "_RequiredAppsListDataOutputTypeDef",
-    {
-        "ListName": str,
-        "AppsList": List[AppTypeDef],
-    },
-)
-_OptionalAppsListDataOutputTypeDef = TypedDict(
-    "_OptionalAppsListDataOutputTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
-    },
-    total=False,
-)
-
-
-class AppsListDataOutputTypeDef(
-    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
-):
-    pass
-
-
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1356,110 +1265,34 @@
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": Sequence[AppTypeDef],
+        "AppsList": List[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": TimestampTypeDef,
-        "LastUpdateTime": TimestampTypeDef,
-        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
-    {
-        "ListName": str,
-        "ProtocolsList": Sequence[str],
-    },
-)
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": TimestampTypeDef,
-        "LastUpdateTime": TimestampTypeDef,
-        "PreviousProtocolsList": Mapping[str, Sequence[str]],
-    },
-    total=False,
-)
-
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
-):
-    pass
-
-
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
-    {
-        "Name": str,
-        "ResourceTypeList": Sequence[str],
-    },
-)
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
-    {
-        "Id": str,
-        "Description": str,
-        "UpdateToken": str,
-        "LastUpdateTime": TimestampTypeDef,
-        "ResourceSetStatus": ResourceSetStatusType,
-    },
-    total=False,
-)
-
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
-    pass
-
-
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1614,45 +1447,71 @@
         "ViolationTarget": str,
         "ExpectedRoutes": List[ExpectedRouteTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
+
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataOutputTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataOutputTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetOutputTypeDef,
+        "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetOutputTypeDef,
+        "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
@@ -1788,14 +1647,56 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
@@ -1955,21 +1856,20 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeOutputTypeDef,
+        "AdminScope": AdminScopeTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
@@ -1983,42 +1883,32 @@
 
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
     {
-        "AppsList": AppsListDataOutputTypeDef,
-        "AppsListArn": str,
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataOutputTypeDef,
+        "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
-    {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
@@ -2032,58 +1922,23 @@
 
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
 
-ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "AppsList": AppsListDataTypeDef,
+        "AppsListArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
-
-ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2159,26 +2014,26 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPolicyOutputTypeDef = TypedDict(
-    "_RequiredPolicyOutputTypeDef",
+_RequiredPolicyTypeDef = TypedDict(
+    "_RequiredPolicyTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
-_OptionalPolicyOutputTypeDef = TypedDict(
-    "_OptionalPolicyOutputTypeDef",
+_OptionalPolicyTypeDef = TypedDict(
+    "_OptionalPolicyTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
@@ -2187,46 +2042,14 @@
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
 
-class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
-    pass
-
-
-_RequiredPolicyTypeDef = TypedDict(
-    "_RequiredPolicyTypeDef",
-    {
-        "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
-        "ResourceType": str,
-        "ExcludeResourceTags": bool,
-        "RemediationEnabled": bool,
-    },
-)
-_OptionalPolicyTypeDef = TypedDict(
-    "_OptionalPolicyTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyUpdateToken": str,
-        "ResourceTypeList": Sequence[str],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "DeleteUnusedFMManagedResources": bool,
-        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
-        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
-        "ResourceSetIds": Sequence[str],
-        "PolicyDescription": str,
-        "PolicyStatus": CustomerPolicyStatusType,
-    },
-    total=False,
-)
-
-
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
 
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
@@ -2248,30 +2071,20 @@
 ):
     pass
 
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
@@ -2285,14 +2098,23 @@
 
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
 
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
```

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.pyi` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_fms.type_defs import AccountScopeOutputTypeDef
+    from types_aiobotocore_fms.type_defs import AccountScopeTypeDef
 
-    data: AccountScopeOutputTypeDef = ...
+    data: AccountScopeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -42,26 +42,21 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
-    "OrganizationalUnitScopeOutputTypeDef",
-    "PolicyTypeScopeOutputTypeDef",
-    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
-    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -81,18 +76,19 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataOutputTypeDef",
+    "ProtocolsListDataTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetOutputTypeDef",
+    "ResourceSetTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
     "ListAppsListsRequestRequestTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
@@ -129,22 +125,17 @@
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
-    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
-    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -154,14 +145,15 @@
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAppsListsRequestListAppsListsPaginateTypeDef",
@@ -171,72 +163,56 @@
     "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
-    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "GetAppsListResponseTypeDef",
-    "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
-    "AppsListDataUnionTypeDef",
+    "GetAppsListResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
-    "ProtocolsListDataUnionTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
-    "ResourceSetUnionTypeDef",
+    "PutAppsListResponseTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
-    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyResponseTypeDef",
-    "PolicyUnionTypeDef",
     "PutPolicyRequestRequestTypeDef",
+    "PutPolicyResponseTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
-AccountScopeOutputTypeDef = TypedDict(
-    "AccountScopeOutputTypeDef",
-    {
-        "Accounts": List[str],
-        "AllAccountsEnabled": bool,
-        "ExcludeSpecifiedAccounts": bool,
-    },
-    total=False,
-)
-
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": Sequence[str],
+        "Accounts": List[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -254,80 +230,51 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
-OrganizationalUnitScopeOutputTypeDef = TypedDict(
-    "OrganizationalUnitScopeOutputTypeDef",
-    {
-        "OrganizationalUnits": List[str],
-        "AllOrganizationalUnitsEnabled": bool,
-        "ExcludeSpecifiedOrganizationalUnits": bool,
-    },
-    total=False,
-)
-
-PolicyTypeScopeOutputTypeDef = TypedDict(
-    "PolicyTypeScopeOutputTypeDef",
-    {
-        "PolicyTypes": List[SecurityServiceTypeType],
-        "AllPolicyTypesEnabled": bool,
-    },
-    total=False,
-)
-
-RegionScopeOutputTypeDef = TypedDict(
-    "RegionScopeOutputTypeDef",
-    {
-        "Regions": List[str],
-        "AllRegionsEnabled": bool,
-    },
-    total=False,
-)
-
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": Sequence[str],
+        "OrganizationalUnits": List[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": Sequence[SecurityServiceTypeType],
+        "PolicyTypes": List[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": Sequence[str],
+        "Regions": List[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -584,14 +531,15 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
@@ -603,67 +551,65 @@
 )
 
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-_RequiredProtocolsListDataOutputTypeDef = TypedDict(
-    "_RequiredProtocolsListDataOutputTypeDef",
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataOutputTypeDef = TypedDict(
-    "_OptionalProtocolsListDataOutputTypeDef",
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-class ProtocolsListDataOutputTypeDef(
-    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetOutputTypeDef = TypedDict(
-    "_RequiredResourceSetOutputTypeDef",
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetOutputTypeDef = TypedDict(
-    "_OptionalResourceSetOutputTypeDef",
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-class ResourceSetOutputTypeDef(
-    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
-):
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
@@ -1252,60 +1198,25 @@
 
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-AdminScopeOutputTypeDef = TypedDict(
-    "AdminScopeOutputTypeDef",
-    {
-        "AccountScope": AccountScopeOutputTypeDef,
-        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
-        "RegionScope": RegionScopeOutputTypeDef,
-        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
-    },
-    total=False,
-)
-
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
-_RequiredAppsListDataOutputTypeDef = TypedDict(
-    "_RequiredAppsListDataOutputTypeDef",
-    {
-        "ListName": str,
-        "AppsList": List[AppTypeDef],
-    },
-)
-_OptionalAppsListDataOutputTypeDef = TypedDict(
-    "_OptionalAppsListDataOutputTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
-    },
-    total=False,
-)
-
-class AppsListDataOutputTypeDef(
-    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
-):
-    pass
-
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1313,102 +1224,32 @@
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": Sequence[AppTypeDef],
+        "AppsList": List[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": TimestampTypeDef,
-        "LastUpdateTime": TimestampTypeDef,
-        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
-    {
-        "ListName": str,
-        "ProtocolsList": Sequence[str],
-    },
-)
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
-    {
-        "ListId": str,
-        "ListUpdateToken": str,
-        "CreateTime": TimestampTypeDef,
-        "LastUpdateTime": TimestampTypeDef,
-        "PreviousProtocolsList": Mapping[str, Sequence[str]],
-    },
-    total=False,
-)
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
-):
-    pass
-
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
-    {
-        "Name": str,
-        "ResourceTypeList": Sequence[str],
-    },
-)
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
-    {
-        "Id": str,
-        "Description": str,
-        "UpdateToken": str,
-        "LastUpdateTime": TimestampTypeDef,
-        "ResourceSetStatus": ResourceSetStatusType,
-    },
-    total=False,
-)
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
-    pass
-
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1563,45 +1404,69 @@
         "ViolationTarget": str,
         "ExpectedRoutes": List[ExpectedRouteTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataOutputTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataOutputTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetOutputTypeDef,
+        "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetOutputTypeDef,
+        "ResourceSet": ResourceSetTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
@@ -1733,14 +1598,52 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
@@ -1900,21 +1803,20 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeOutputTypeDef,
+        "AdminScope": AdminScopeTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
@@ -1926,42 +1828,32 @@
 )
 
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
     {
-        "AppsList": AppsListDataOutputTypeDef,
-        "AppsListArn": str,
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataOutputTypeDef,
+        "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
-    {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
@@ -1973,54 +1865,23 @@
 )
 
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-    },
-)
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
-    {
-        "TagList": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-    },
-)
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "AppsList": AppsListDataTypeDef,
+        "AppsListArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
-
-ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2094,26 +1955,26 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPolicyOutputTypeDef = TypedDict(
-    "_RequiredPolicyOutputTypeDef",
+_RequiredPolicyTypeDef = TypedDict(
+    "_RequiredPolicyTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
-_OptionalPolicyOutputTypeDef = TypedDict(
-    "_OptionalPolicyOutputTypeDef",
+_OptionalPolicyTypeDef = TypedDict(
+    "_OptionalPolicyTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
@@ -2121,44 +1982,14 @@
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
-    pass
-
-_RequiredPolicyTypeDef = TypedDict(
-    "_RequiredPolicyTypeDef",
-    {
-        "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
-        "ResourceType": str,
-        "ExcludeResourceTags": bool,
-        "RemediationEnabled": bool,
-    },
-)
-_OptionalPolicyTypeDef = TypedDict(
-    "_OptionalPolicyTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyUpdateToken": str,
-        "ResourceTypeList": Sequence[str],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "DeleteUnusedFMManagedResources": bool,
-        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
-        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
-        "ResourceSetIds": Sequence[str],
-        "PolicyDescription": str,
-        "PolicyStatus": CustomerPolicyStatusType,
-    },
-    total=False,
-)
-
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
@@ -2177,30 +2008,20 @@
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
@@ -2212,14 +2033,23 @@
 )
 
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
```

### Comparing `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/SOURCES.txt` & `types-aiobotocore-fms-2.5.2.post2/types_aiobotocore_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

