# Comparing `tmp/types-aiobotocore-workmail-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-workmail-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workmail-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-workmail-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-workmail-2.5.2.post1.tar` & `types-aiobotocore-workmail-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.157424 types-aiobotocore-workmail-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:19.000000 types-aiobotocore-workmail-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-08-02 14:53:11.157424 types-aiobotocore-workmail-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-02 14:51:19.000000 types-aiobotocore-workmail-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.157424 types-aiobotocore-workmail-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:19.000000 types-aiobotocore-workmail-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.157424 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60381 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60283 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:20.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60480 2023-08-02 14:51:21.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60400 2023-08-02 14:51:21.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:19.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.157424 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:11.000000 types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.156643 types-aiobotocore-workmail-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14171 2023-08-04 13:59:30.156643 types-aiobotocore-workmail-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12649 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.156643 types-aiobotocore-workmail-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.146643 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2345 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2344 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60366 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60268 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10179 2023-08-04 13:56:15.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10177 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11068 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11057 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59709 2023-08-04 13:56:16.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59630 2023-08-04 13:56:15.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:14.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.156643 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14171 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:30.000000 types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workmail-2.5.2.post1/LICENSE` & `types-aiobotocore-workmail-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.2.post1/setup.py` & `types-aiobotocore-workmail-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workmail",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkMail 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__init__.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__init__.pyi` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/__main__.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkMail 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WorkMail 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/client.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
-    ImpersonationRuleUnionTypeDef,
+    ImpersonationRuleTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
@@ -243,15 +243,15 @@
 
     async def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleUnionTypeDef],
+        Rules: Sequence[ImpersonationRuleTypeDef],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -1039,15 +1039,15 @@
     async def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleUnionTypeDef],
+        Rules: Sequence[ImpersonationRuleTypeDef],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_impersonation_role)
```

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/client.pyi` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     GetDefaultRetentionPolicyResponseTypeDef,
     GetImpersonationRoleEffectResponseTypeDef,
     GetImpersonationRoleResponseTypeDef,
     GetMailboxDetailsResponseTypeDef,
     GetMailDomainResponseTypeDef,
     GetMobileDeviceAccessEffectResponseTypeDef,
     GetMobileDeviceAccessOverrideResponseTypeDef,
-    ImpersonationRuleUnionTypeDef,
+    ImpersonationRuleTypeDef,
     LambdaAvailabilityProviderTypeDef,
     ListAccessControlRulesResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
     ListGroupMembersResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListImpersonationRolesResponseTypeDef,
@@ -229,15 +229,15 @@
         """
     async def create_impersonation_role(
         self,
         *,
         OrganizationId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleUnionTypeDef],
+        Rules: Sequence[ImpersonationRuleTypeDef],
         ClientToken: str = ...,
         Description: str = ...
     ) -> CreateImpersonationRoleResponseTypeDef:
         """
         Creates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.create_impersonation_role)
@@ -956,15 +956,15 @@
     async def update_impersonation_role(
         self,
         *,
         OrganizationId: str,
         ImpersonationRoleId: str,
         Name: str,
         Type: ImpersonationRoleTypeType,
-        Rules: Sequence[ImpersonationRuleUnionTypeDef],
+        Rules: Sequence[ImpersonationRuleTypeDef],
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an impersonation role for the given WorkMail organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail.Client.update_impersonation_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmail/client/#update_impersonation_role)
```

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/literals.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccessControlRuleEffectType",
     "AccessEffectType",
     "AvailabilityProviderTypeType",
     "DnsRecordVerificationStatusType",
     "EntityStateType",
     "FolderNameType",
@@ -46,15 +45,14 @@
     "WorkMailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessControlRuleEffectType = Literal["ALLOW", "DENY"]
 AccessEffectType = Literal["ALLOW", "DENY"]
 AvailabilityProviderTypeType = Literal["EWS", "LAMBDA"]
 DnsRecordVerificationStatusType = Literal["FAILED", "PENDING", "VERIFIED"]
 EntityStateType = Literal["DELETED", "DISABLED", "ENABLED"]
 FolderNameType = Literal["DELETED_ITEMS", "DRAFTS", "INBOX", "JUNK_EMAIL", "SENT_ITEMS"]
 ImpersonationRoleTypeType = Literal["FULL_ACCESS", "READ_ONLY"]
@@ -86,14 +84,15 @@
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
@@ -189,14 +188,15 @@
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
@@ -275,26 +275,28 @@
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

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/literals.pyi` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccessControlRuleEffectType",
     "AccessEffectType",
     "AvailabilityProviderTypeType",
     "DnsRecordVerificationStatusType",
     "EntityStateType",
     "FolderNameType",
@@ -45,14 +46,15 @@
     "WorkMailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AccessControlRuleEffectType = Literal["ALLOW", "DENY"]
 AccessEffectType = Literal["ALLOW", "DENY"]
 AvailabilityProviderTypeType = Literal["EWS", "LAMBDA"]
 DnsRecordVerificationStatusType = Literal["FAILED", "PENDING", "VERIFIED"]
 EntityStateType = Literal["DELETED", "DISABLED", "ENABLED"]
 FolderNameType = Literal["DELETED_ITEMS", "DRAFTS", "INBOX", "JUNK_EMAIL", "SENT_ITEMS"]
 ImpersonationRoleTypeType = Literal["FULL_ACCESS", "READ_ONLY"]
@@ -84,14 +86,15 @@
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
@@ -187,14 +190,15 @@
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
@@ -273,26 +277,28 @@
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

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/paginator.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/paginator.pyi` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/type_defs.py` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_workmail.type_defs import AccessControlRuleTypeDef
 
     data: AccessControlRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AccessControlRuleEffectType,
     AccessEffectType,
     AvailabilityProviderTypeType,
     DnsRecordVerificationStatusType,
     EntityStateType,
@@ -33,28 +33,28 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
@@ -83,23 +83,21 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
-    "ImpersonationRuleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "ListGroupsRequestRequestTypeDef",
@@ -160,25 +158,26 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
+    "CreateImpersonationRoleRequestRequestTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
+    "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
-    "ImpersonationRuleUnionTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
@@ -192,16 +191,14 @@
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
-    "CreateImpersonationRoleRequestRequestTypeDef",
-    "UpdateImpersonationRoleRequestRequestTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
@@ -314,14 +311,37 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
+_RequiredImpersonationRuleTypeDef = TypedDict(
+    "_RequiredImpersonationRuleTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleTypeDef = TypedDict(
+    "_OptionalImpersonationRuleTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": Sequence[str],
+        "NotTargetUsers": Sequence[str],
+    },
+    total=False,
+)
+
+class ImpersonationRuleTypeDef(
+    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
+):
+    pass
+
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -339,22 +359,20 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
-
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
@@ -472,22 +490,20 @@
     "_OptionalDeleteOrganizationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -616,21 +632,19 @@
     "_OptionalFolderConfigurationTypeDef",
     {
         "Period": int,
     },
     total=False,
 )
 
-
 class FolderConfigurationTypeDef(
     _RequiredFolderConfigurationTypeDef, _OptionalFolderConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetAccessControlEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetAccessControlEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "IpAddress": str,
         "Action": str,
     },
@@ -640,22 +654,20 @@
     {
         "UserId": str,
         "ImpersonationRoleId": str,
     },
     total=False,
 )
 
-
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
-
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -681,39 +693,14 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
-
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -739,22 +726,20 @@
         "DeviceModel": str,
         "DeviceOperatingSystem": str,
         "DeviceUserAgent": str,
     },
     total=False,
 )
 
-
 class GetMobileDeviceAccessEffectRequestRequestTypeDef(
     _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef,
     _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef,
 ):
     pass
 
-
 MobileDeviceAccessMatchedRuleTypeDef = TypedDict(
     "MobileDeviceAccessMatchedRuleTypeDef",
     {
         "MobileDeviceAccessRuleId": str,
         "Name": str,
     },
     total=False,
@@ -790,39 +775,14 @@
         "Type": ImpersonationRoleTypeType,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
-_RequiredImpersonationRuleTypeDef = TypedDict(
-    "_RequiredImpersonationRuleTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleTypeDef = TypedDict(
-    "_OptionalImpersonationRuleTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": Sequence[str],
-        "NotTargetUsers": Sequence[str],
-    },
-    total=False,
-)
-
-
-class ImpersonationRuleTypeDef(
-    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
-):
-    pass
-
-
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -848,21 +808,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -870,22 +828,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -894,21 +850,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupMembersRequestRequestTypeDef(
     _RequiredListGroupMembersRequestRequestTypeDef, _OptionalListGroupMembersRequestRequestTypeDef
 ):
     pass
 
-
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "Id": str,
         "Name": str,
         "Type": MemberTypeType,
         "State": EntityStateType,
@@ -929,21 +883,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListImpersonationRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListImpersonationRolesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListImpersonationRolesRequestRequestTypeDef = TypedDict(
@@ -951,22 +903,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListImpersonationRolesRequestRequestTypeDef(
     _RequiredListImpersonationRolesRequestRequestTypeDef,
     _OptionalListImpersonationRolesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListMailDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailDomainsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListMailDomainsRequestRequestTypeDef = TypedDict(
@@ -974,21 +924,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMailDomainsRequestRequestTypeDef(
     _RequiredListMailDomainsRequestRequestTypeDef, _OptionalListMailDomainsRequestRequestTypeDef
 ):
     pass
 
-
 MailDomainSummaryTypeDef = TypedDict(
     "MailDomainSummaryTypeDef",
     {
         "DomainName": str,
         "DefaultDomain": bool,
     },
     total=False,
@@ -1005,22 +953,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMailboxExportJobsRequestRequestTypeDef(
     _RequiredListMailboxExportJobsRequestRequestTypeDef,
     _OptionalListMailboxExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 MailboxExportJobTypeDef = TypedDict(
     "MailboxExportJobTypeDef",
     {
         "JobId": str,
         "EntityId": str,
         "Description": str,
         "S3BucketName": str,
@@ -1045,22 +991,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMailboxPermissionsRequestRequestTypeDef(
     _RequiredListMailboxPermissionsRequestRequestTypeDef,
     _OptionalListMailboxPermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeId": str,
         "GranteeType": MemberTypeType,
         "PermissionValues": List[PermissionTypeType],
     },
@@ -1079,22 +1023,20 @@
         "DeviceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMobileDeviceAccessOverridesRequestRequestTypeDef(
     _RequiredListMobileDeviceAccessOverridesRequestRequestTypeDef,
     _OptionalListMobileDeviceAccessOverridesRequestRequestTypeDef,
 ):
     pass
 
-
 MobileDeviceAccessOverrideTypeDef = TypedDict(
     "MobileDeviceAccessOverrideTypeDef",
     {
         "UserId": str,
         "DeviceId": str,
         "Effect": MobileDeviceAccessRuleEffectType,
         "Description": str,
@@ -1165,22 +1107,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1188,21 +1128,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
@@ -1239,21 +1177,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "DisplayName": str,
@@ -1285,22 +1221,20 @@
         "NotUserIds": Sequence[str],
         "ImpersonationRoleIds": Sequence[str],
         "NotImpersonationRoleIds": Sequence[str],
     },
     total=False,
 )
 
-
 class PutAccessControlRuleRequestRequestTypeDef(
     _RequiredPutAccessControlRuleRequestRequestTypeDef,
     _OptionalPutAccessControlRuleRequestRequestTypeDef,
 ):
     pass
 
-
 PutEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "RoleArn": str,
         "LogGroupArn": str,
     },
@@ -1337,22 +1271,20 @@
     "_OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class PutMobileDeviceAccessOverrideRequestRequestTypeDef(
     _RequiredPutMobileDeviceAccessOverrideRequestRequestTypeDef,
     _OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRegisterMailDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1360,22 +1292,20 @@
     "_OptionalRegisterMailDomainRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class RegisterMailDomainRequestRequestTypeDef(
     _RequiredRegisterMailDomainRequestRequestTypeDef,
     _OptionalRegisterMailDomainRequestRequestTypeDef,
 ):
     pass
 
-
 RegisterToWorkMailRequestRequestTypeDef = TypedDict(
     "RegisterToWorkMailRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1406,22 +1336,20 @@
     "_OptionalStartMailboxExportJobRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1464,22 +1392,20 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
-
 UpdatePrimaryEmailAddressRequestRequestTypeDef = TypedDict(
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1736,21 +1662,19 @@
     {
         "Name": str,
         "BookingOptions": BookingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1760,22 +1684,20 @@
         "ClientToken": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class CreateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
@@ -1784,22 +1706,20 @@
         "DomainName": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class TestAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredTestAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalTestAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1808,21 +1728,81 @@
     {
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleTypeDef],
+    },
+)
+_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+class CreateImpersonationRoleRequestRequestTypeDef(
+    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
+    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
+
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleTypeDef],
+    },
+)
+_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateImpersonationRoleRequestRequestTypeDef(
+    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
+    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
 
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
@@ -1834,22 +1814,20 @@
         "Domains": Sequence[DomainTypeDef],
         "KmsKeyArn": str,
         "EnableInteroperability": bool,
     },
     total=False,
 )
 
-
 class CreateOrganizationRequestRequestTypeDef(
     _RequiredCreateOrganizationRequestRequestTypeDef,
     _OptionalCreateOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1891,46 +1869,30 @@
     {
         "Id": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class PutRetentionPolicyRequestRequestTypeDef(
     _RequiredPutRetentionPolicyRequestRequestTypeDef,
     _OptionalPutRetentionPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1950,15 +1912,14 @@
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImpersonationRuleUnionTypeDef = Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]
 _RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
     "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1966,44 +1927,40 @@
     "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAliasesRequestListAliasesPaginateTypeDef(
     _RequiredListAliasesRequestListAliasesPaginateTypeDef,
     _OptionalListAliasesRequestListAliasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
     _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -2011,44 +1968,40 @@
     "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
     _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
     _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -2056,22 +2009,20 @@
     "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
     _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
 ):
     pass
 
-
 ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2087,66 +2038,60 @@
     "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
     _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListResourcesRequestListResourcesPaginateTypeDef(
     _RequiredListResourcesRequestListResourcesPaginateTypeDef,
     _OptionalListResourcesRequestListResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2243,58 +2188,7 @@
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
-    },
-)
-_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class CreateImpersonationRoleRequestRequestTypeDef(
-    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
-    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
-    },
-)
-_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateImpersonationRoleRequestRequestTypeDef(
-    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
-    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail/type_defs.pyi` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_workmail.type_defs import AccessControlRuleTypeDef
 
     data: AccessControlRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AccessControlRuleEffectType,
     AccessEffectType,
     AvailabilityProviderTypeType,
     DnsRecordVerificationStatusType,
     EntityStateType,
@@ -33,27 +33,29 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
     "DeleteAccessControlRuleRequestRequestTypeDef",
     "DeleteAliasRequestRequestTypeDef",
@@ -82,23 +84,21 @@
     "DnsRecordTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
-    "ImpersonationRuleOutputTypeDef",
     "GetMailDomainRequestRequestTypeDef",
     "GetMailboxDetailsRequestRequestTypeDef",
     "GetMobileDeviceAccessEffectRequestRequestTypeDef",
     "MobileDeviceAccessMatchedRuleTypeDef",
     "GetMobileDeviceAccessOverrideRequestRequestTypeDef",
     "GroupTypeDef",
     "ImpersonationRoleTypeDef",
-    "ImpersonationRuleTypeDef",
     "ListAccessControlRulesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAvailabilityConfigurationsRequestRequestTypeDef",
     "ListGroupMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "ListGroupsRequestRequestTypeDef",
@@ -159,25 +159,26 @@
     "TestAvailabilityConfigurationResponseTypeDef",
     "AvailabilityConfigurationTypeDef",
     "DescribeResourceResponseTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "CreateAvailabilityConfigurationRequestRequestTypeDef",
     "TestAvailabilityConfigurationRequestRequestTypeDef",
     "UpdateAvailabilityConfigurationRequestRequestTypeDef",
+    "CreateImpersonationRoleRequestRequestTypeDef",
+    "GetImpersonationRoleResponseTypeDef",
+    "UpdateImpersonationRoleRequestRequestTypeDef",
     "CreateOrganizationRequestRequestTypeDef",
     "ListResourceDelegatesResponseTypeDef",
     "GetMailDomainResponseTypeDef",
     "GetDefaultRetentionPolicyResponseTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectResponseTypeDef",
-    "GetImpersonationRoleResponseTypeDef",
     "GetMobileDeviceAccessEffectResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "ListImpersonationRolesResponseTypeDef",
-    "ImpersonationRuleUnionTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     "ListGroupMembersRequestListGroupMembersPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     "ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
@@ -191,16 +192,14 @@
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
-    "CreateImpersonationRoleRequestRequestTypeDef",
-    "UpdateImpersonationRoleRequestRequestTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
         "Effect": AccessControlRuleEffectType,
@@ -313,14 +312,39 @@
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
 
+_RequiredImpersonationRuleTypeDef = TypedDict(
+    "_RequiredImpersonationRuleTypeDef",
+    {
+        "ImpersonationRuleId": str,
+        "Effect": AccessEffectType,
+    },
+)
+_OptionalImpersonationRuleTypeDef = TypedDict(
+    "_OptionalImpersonationRuleTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "TargetUsers": Sequence[str],
+        "NotTargetUsers": Sequence[str],
+    },
+    total=False,
+)
+
+
+class ImpersonationRuleTypeDef(
+    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
+):
+    pass
+
+
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -338,20 +362,22 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
+
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
@@ -469,20 +495,22 @@
     "_OptionalDeleteOrganizationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -611,19 +639,21 @@
     "_OptionalFolderConfigurationTypeDef",
     {
         "Period": int,
     },
     total=False,
 )
 
+
 class FolderConfigurationTypeDef(
     _RequiredFolderConfigurationTypeDef, _OptionalFolderConfigurationTypeDef
 ):
     pass
 
+
 _RequiredGetAccessControlEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetAccessControlEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "IpAddress": str,
         "Action": str,
     },
@@ -633,20 +663,22 @@
     {
         "UserId": str,
         "ImpersonationRoleId": str,
     },
     total=False,
 )
 
+
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
+
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -672,37 +704,14 @@
     "GetImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
     },
 )
 
-_RequiredImpersonationRuleOutputTypeDef = TypedDict(
-    "_RequiredImpersonationRuleOutputTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleOutputTypeDef = TypedDict(
-    "_OptionalImpersonationRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": List[str],
-        "NotTargetUsers": List[str],
-    },
-    total=False,
-)
-
-class ImpersonationRuleOutputTypeDef(
-    _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
-):
-    pass
-
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -728,20 +737,22 @@
         "DeviceModel": str,
         "DeviceOperatingSystem": str,
         "DeviceUserAgent": str,
     },
     total=False,
 )
 
+
 class GetMobileDeviceAccessEffectRequestRequestTypeDef(
     _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef,
     _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef,
 ):
     pass
 
+
 MobileDeviceAccessMatchedRuleTypeDef = TypedDict(
     "MobileDeviceAccessMatchedRuleTypeDef",
     {
         "MobileDeviceAccessRuleId": str,
         "Name": str,
     },
     total=False,
@@ -777,37 +788,14 @@
         "Type": ImpersonationRoleTypeType,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
-_RequiredImpersonationRuleTypeDef = TypedDict(
-    "_RequiredImpersonationRuleTypeDef",
-    {
-        "ImpersonationRuleId": str,
-        "Effect": AccessEffectType,
-    },
-)
-_OptionalImpersonationRuleTypeDef = TypedDict(
-    "_OptionalImpersonationRuleTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "TargetUsers": Sequence[str],
-        "NotTargetUsers": Sequence[str],
-    },
-    total=False,
-)
-
-class ImpersonationRuleTypeDef(
-    _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
-):
-    pass
-
 ListAccessControlRulesRequestRequestTypeDef = TypedDict(
     "ListAccessControlRulesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -833,19 +821,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -853,20 +843,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -875,19 +867,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListGroupMembersRequestRequestTypeDef(
     _RequiredListGroupMembersRequestRequestTypeDef, _OptionalListGroupMembersRequestRequestTypeDef
 ):
     pass
 
+
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "Id": str,
         "Name": str,
         "Type": MemberTypeType,
         "State": EntityStateType,
@@ -908,19 +902,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListImpersonationRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListImpersonationRolesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListImpersonationRolesRequestRequestTypeDef = TypedDict(
@@ -928,20 +924,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListImpersonationRolesRequestRequestTypeDef(
     _RequiredListImpersonationRolesRequestRequestTypeDef,
     _OptionalListImpersonationRolesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListMailDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailDomainsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListMailDomainsRequestRequestTypeDef = TypedDict(
@@ -949,19 +947,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMailDomainsRequestRequestTypeDef(
     _RequiredListMailDomainsRequestRequestTypeDef, _OptionalListMailDomainsRequestRequestTypeDef
 ):
     pass
 
+
 MailDomainSummaryTypeDef = TypedDict(
     "MailDomainSummaryTypeDef",
     {
         "DomainName": str,
         "DefaultDomain": bool,
     },
     total=False,
@@ -978,20 +978,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMailboxExportJobsRequestRequestTypeDef(
     _RequiredListMailboxExportJobsRequestRequestTypeDef,
     _OptionalListMailboxExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 MailboxExportJobTypeDef = TypedDict(
     "MailboxExportJobTypeDef",
     {
         "JobId": str,
         "EntityId": str,
         "Description": str,
         "S3BucketName": str,
@@ -1016,20 +1018,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMailboxPermissionsRequestRequestTypeDef(
     _RequiredListMailboxPermissionsRequestRequestTypeDef,
     _OptionalListMailboxPermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeId": str,
         "GranteeType": MemberTypeType,
         "PermissionValues": List[PermissionTypeType],
     },
@@ -1048,20 +1052,22 @@
         "DeviceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMobileDeviceAccessOverridesRequestRequestTypeDef(
     _RequiredListMobileDeviceAccessOverridesRequestRequestTypeDef,
     _OptionalListMobileDeviceAccessOverridesRequestRequestTypeDef,
 ):
     pass
 
+
 MobileDeviceAccessOverrideTypeDef = TypedDict(
     "MobileDeviceAccessOverrideTypeDef",
     {
         "UserId": str,
         "DeviceId": str,
         "Effect": MobileDeviceAccessRuleEffectType,
         "Description": str,
@@ -1132,20 +1138,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1153,19 +1161,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
@@ -1202,19 +1212,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "DisplayName": str,
@@ -1246,20 +1258,22 @@
         "NotUserIds": Sequence[str],
         "ImpersonationRoleIds": Sequence[str],
         "NotImpersonationRoleIds": Sequence[str],
     },
     total=False,
 )
 
+
 class PutAccessControlRuleRequestRequestTypeDef(
     _RequiredPutAccessControlRuleRequestRequestTypeDef,
     _OptionalPutAccessControlRuleRequestRequestTypeDef,
 ):
     pass
 
+
 PutEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "RoleArn": str,
         "LogGroupArn": str,
     },
@@ -1296,20 +1310,22 @@
     "_OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class PutMobileDeviceAccessOverrideRequestRequestTypeDef(
     _RequiredPutMobileDeviceAccessOverrideRequestRequestTypeDef,
     _OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRegisterMailDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1317,20 +1333,22 @@
     "_OptionalRegisterMailDomainRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class RegisterMailDomainRequestRequestTypeDef(
     _RequiredRegisterMailDomainRequestRequestTypeDef,
     _OptionalRegisterMailDomainRequestRequestTypeDef,
 ):
     pass
 
+
 RegisterToWorkMailRequestRequestTypeDef = TypedDict(
     "RegisterToWorkMailRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1361,20 +1379,22 @@
     "_OptionalStartMailboxExportJobRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1417,20 +1437,22 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
+
 UpdatePrimaryEmailAddressRequestRequestTypeDef = TypedDict(
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1687,19 +1709,21 @@
     {
         "Name": str,
         "BookingOptions": BookingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1709,20 +1733,22 @@
         "ClientToken": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class CreateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
@@ -1731,20 +1757,22 @@
         "DomainName": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class TestAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredTestAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalTestAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1753,20 +1781,88 @@
     {
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleTypeDef],
+    },
+)
+_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class CreateImpersonationRoleRequestRequestTypeDef(
+    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
+    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
+
+
+GetImpersonationRoleResponseTypeDef = TypedDict(
+    "GetImpersonationRoleResponseTypeDef",
+    {
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Description": str,
+        "Rules": List[ImpersonationRuleTypeDef],
+        "DateCreated": datetime,
+        "DateModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "OrganizationId": str,
+        "ImpersonationRoleId": str,
+        "Name": str,
+        "Type": ImpersonationRoleTypeType,
+        "Rules": Sequence[ImpersonationRuleTypeDef],
+    },
+)
+_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateImpersonationRoleRequestRequestTypeDef(
+    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
+    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
 _OptionalCreateOrganizationRequestRequestTypeDef = TypedDict(
@@ -1777,20 +1873,22 @@
         "Domains": Sequence[DomainTypeDef],
         "KmsKeyArn": str,
         "EnableInteroperability": bool,
     },
     total=False,
 )
 
+
 class CreateOrganizationRequestRequestTypeDef(
     _RequiredCreateOrganizationRequestRequestTypeDef,
     _OptionalCreateOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1832,44 +1930,32 @@
     {
         "Id": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class PutRetentionPolicyRequestRequestTypeDef(
     _RequiredPutRetentionPolicyRequestRequestTypeDef,
     _OptionalPutRetentionPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetImpersonationRoleResponseTypeDef = TypedDict(
-    "GetImpersonationRoleResponseTypeDef",
-    {
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Description": str,
-        "Rules": List[ImpersonationRuleOutputTypeDef],
-        "DateCreated": datetime,
-        "DateModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMobileDeviceAccessEffectResponseTypeDef = TypedDict(
     "GetMobileDeviceAccessEffectResponseTypeDef",
     {
         "Effect": MobileDeviceAccessRuleEffectType,
         "MatchedRules": List[MobileDeviceAccessMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1889,15 +1975,14 @@
     {
         "Roles": List[ImpersonationRoleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImpersonationRuleUnionTypeDef = Union[ImpersonationRuleTypeDef, ImpersonationRuleOutputTypeDef]
 _RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
     "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1905,40 +1990,44 @@
     "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAliasesRequestListAliasesPaginateTypeDef(
     _RequiredListAliasesRequestListAliasesPaginateTypeDef,
     _OptionalListAliasesRequestListAliasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
     _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -1946,40 +2035,44 @@
     "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
     _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
     _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -1987,20 +2080,22 @@
     "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
     _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
 ):
     pass
 
+
 ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2016,60 +2111,66 @@
     "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
     _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListResourcesRequestListResourcesPaginateTypeDef(
     _RequiredListResourcesRequestListResourcesPaginateTypeDef,
     _OptionalListResourcesRequestListResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2166,55 +2267,7 @@
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
-    },
-)
-_OptionalCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImpersonationRoleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-    },
-    total=False,
-)
-
-class CreateImpersonationRoleRequestRequestTypeDef(
-    _RequiredCreateImpersonationRoleRequestRequestTypeDef,
-    _OptionalCreateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "OrganizationId": str,
-        "ImpersonationRoleId": str,
-        "Name": str,
-        "Type": ImpersonationRoleTypeType,
-        "Rules": Sequence[ImpersonationRuleUnionTypeDef],
-    },
-)
-_OptionalUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateImpersonationRoleRequestRequestTypeDef(
-    _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
-    _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-workmail-2.5.2.post1/types_aiobotocore_workmail.egg-info/SOURCES.txt` & `types-aiobotocore-workmail-2.5.2.post2/types_aiobotocore_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

