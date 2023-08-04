# Comparing `tmp/types-aiobotocore-wafv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-wafv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wafv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-wafv2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-wafv2-2.5.2.post1.tar` & `types-aiobotocore-wafv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.421429 types-aiobotocore-wafv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-08-02 14:53:09.417430 types-aiobotocore-wafv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.421429 types-aiobotocore-wafv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.413430 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39179 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88004 2023-08-02 14:51:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    87901 2023-08-02 14:51:08.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.417430 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12072 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10562 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      426 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      425 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39160 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39099 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13571 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13569 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    68634 2023-08-04 13:55:57.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    68553 2023-08-04 13:55:56.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12072 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      700 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/LICENSE` & `types-aiobotocore-wafv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/setup.py` & `types-aiobotocore-wafv2-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wafv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__main__.py` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WAFV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.py` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigUnionTypeDef,
+    AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionUnionTypeDef,
+    DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -57,22 +57,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleUnionTypeDef,
+    RuleTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TimeWindowUnionTypeDef,
+    TimeWindowTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -143,15 +143,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#can_paginate)
         """
 
     async def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#check_capacity)
@@ -215,15 +215,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
@@ -231,24 +231,24 @@
         """
 
     async def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionUnionTypeDef,
+        DefaultAction: DefaultActionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigUnionTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -484,15 +484,15 @@
 
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowUnionTypeDef,
+        TimeWindow: TimeWindowTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -647,15 +647,15 @@
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_web_acls)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_logging_configuration)
@@ -759,15 +759,15 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
@@ -775,24 +775,24 @@
 
     async def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionUnionTypeDef,
+        DefaultAction: DefaultActionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigUnionTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.pyi` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigUnionTypeDef,
+    AssociationConfigTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionUnionTypeDef,
+    DefaultActionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -57,22 +57,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleUnionTypeDef,
+    RuleTypeDef,
     TagTypeDef,
     TimestampTypeDef,
-    TimeWindowUnionTypeDef,
+    TimeWindowTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -137,15 +137,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#can_paginate)
         """
     async def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#check_capacity)
@@ -204,39 +204,39 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_rule_group)
         """
     async def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionUnionTypeDef,
+        DefaultAction: DefaultActionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigUnionTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -449,15 +449,15 @@
         """
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowUnionTypeDef,
+        TimeWindow: TimeWindowTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -597,15 +597,15 @@
         """
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_web_acls)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_logging_configuration)
@@ -701,39 +701,39 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
         """
     async def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionUnionTypeDef,
+        DefaultAction: DefaultActionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleUnionTypeDef] = ...,
+        Rules: Sequence[RuleTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigUnionTypeDef = ...
+        AssociationConfig: AssociationConfigTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.py` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,15 @@
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
@@ -478,14 +479,15 @@
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
@@ -564,26 +566,28 @@
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
@@ -744,14 +748,15 @@
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

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.pyi` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,15 @@
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
@@ -476,14 +477,15 @@
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
@@ -562,26 +564,28 @@
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
@@ -742,14 +746,15 @@
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

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.py` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,27 +56,25 @@
 
 
 __all__ = (
     "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
-    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
-    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
@@ -111,22 +109,19 @@
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
-    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
-    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
@@ -142,41 +137,32 @@
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
-    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RateLimitLabelNamespaceTypeDef",
-    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
-    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
-    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
-    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
-    "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
-    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
-    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
-    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
     "CheckCapacityResponseTypeDef",
     "CreateAPIKeyResponseTypeDef",
     "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyResponseTypeDef",
@@ -186,15 +172,14 @@
     "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "ConditionTypeDef",
-    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
@@ -203,125 +188,85 @@
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
-    "CustomRequestHandlingOutputTypeDef",
     "CustomRequestHandlingTypeDef",
-    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
-    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "HTTPRequestTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
-    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
-    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
-    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
     "TimeWindowTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "AssociationConfigUnionTypeDef",
-    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
-    "AllowActionOutputTypeDef",
-    "CaptchaActionOutputTypeDef",
-    "ChallengeActionOutputTypeDef",
-    "CountActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
-    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
-    "AWSManagedRulesACFPRuleSetOutputTypeDef",
-    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
-    "TimeWindowUnionTypeDef",
-    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
-    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
-    "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
-    "DefaultActionOutputTypeDef",
-    "RuleActionOutputTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
-    "ByteMatchStatementOutputTypeDef",
-    "RegexMatchStatementOutputTypeDef",
-    "RegexPatternSetReferenceStatementOutputTypeDef",
-    "SizeConstraintStatementOutputTypeDef",
-    "SqliMatchStatementOutputTypeDef",
-    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
-    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideOutputTypeDef",
-    "RuleOutputTypeDef",
-    "RuleSummaryTypeDef",
-    "DefaultActionUnionTypeDef",
     "RuleActionOverrideTypeDef",
+    "RuleSummaryTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
-    "ManagedRuleGroupStatementOutputTypeDef",
-    "RuleGroupReferenceStatementOutputTypeDef",
-    "RuleGroupTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
+    "PutLoggingConfigurationResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "RuleUnionTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementOutputTypeDef",
-    "GetRuleGroupResponseTypeDef",
-    "StatementTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
+    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementTypeDef",
+    "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -352,21 +297,14 @@
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
-AndStatementOutputTypeDef = TypedDict(
-    "AndStatementOutputTypeDef",
-    {
-        "Statements": List["StatementOutputTypeDef"],
-    },
-)
-
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -443,24 +381,14 @@
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
-CookieMatchPatternOutputTypeDef = TypedDict(
-    "CookieMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedCookies": List[str],
-        "ExcludedCookies": List[str],
-    },
-    total=False,
-)
-
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -868,22 +796,14 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowOutputTypeDef = TypedDict(
-    "TimeWindowOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-)
-
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -901,24 +821,14 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-HeaderMatchPatternOutputTypeDef = TypedDict(
-    "HeaderMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedHeaders": List[str],
-        "ExcludedHeaders": List[str],
-    },
-    total=False,
-)
-
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
@@ -930,23 +840,14 @@
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
-JsonMatchPatternOutputTypeDef = TypedDict(
-    "JsonMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedPaths": List[str],
-    },
-    total=False,
-)
-
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
@@ -1308,22 +1209,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
-    },
-)
-
-OrStatementOutputTypeDef = TypedDict(
-    "OrStatementOutputTypeDef",
-    {
-        "Statements": List[Dict[str, Any]],
+        "Statement": Dict[str, Any],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1357,74 +1251,40 @@
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
-ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
-    "ResponseInspectionBodyContainsOutputTypeDef",
-    {
-        "SuccessStrings": List[str],
-        "FailureStrings": List[str],
-    },
-)
-
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
-ResponseInspectionHeaderOutputTypeDef = TypedDict(
-    "ResponseInspectionHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "SuccessValues": List[str],
-        "FailureValues": List[str],
-    },
-)
-
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionJsonOutputTypeDef = TypedDict(
-    "ResponseInspectionJsonOutputTypeDef",
-    {
-        "Identifier": str,
-        "SuccessValues": List[str],
-        "FailureValues": List[str],
-    },
-)
-
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeOutputTypeDef",
-    {
-        "SuccessCodes": List[int],
-        "FailureCodes": List[int],
-    },
-)
-
 ResponseInspectionStatusCodeTypeDef = TypedDict(
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
     },
 )
@@ -1459,89 +1319,57 @@
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-AssociationConfigOutputTypeDef = TypedDict(
-    "AssociationConfigOutputTypeDef",
-    {
-        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
-    },
-    total=False,
-)
-
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
         "RequestBody": Mapping[
             Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
         ],
     },
     total=False,
 )
 
-RateLimitCookieOutputTypeDef = TypedDict(
-    "RateLimitCookieOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderOutputTypeDef = TypedDict(
-    "RateLimitHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitHeaderTypeDef = TypedDict(
     "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryArgumentOutputTypeDef = TypedDict(
-    "RateLimitQueryArgumentOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringOutputTypeDef = TypedDict(
-    "RateLimitQueryStringOutputTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
-        "TextTransformations": List[TextTransformationTypeDef],
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringTypeDef = TypedDict(
-    "RateLimitQueryStringTypeDef",
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
@@ -1681,23 +1509,14 @@
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
-CookiesOutputTypeDef = TypedDict(
-    "CookiesOutputTypeDef",
-    {
-        "MatchPattern": CookieMatchPatternOutputTypeDef,
-        "MatchScope": MapMatchScopeType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1883,50 +1702,21 @@
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomRequestHandlingOutputTypeDef = TypedDict(
-    "CustomRequestHandlingOutputTypeDef",
-    {
-        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
-    },
-)
-
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
-_RequiredCustomResponseOutputTypeDef = TypedDict(
-    "_RequiredCustomResponseOutputTypeDef",
-    {
-        "ResponseCode": int,
-    },
-)
-_OptionalCustomResponseOutputTypeDef = TypedDict(
-    "_OptionalCustomResponseOutputTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
-    },
-    total=False,
-)
-
-
-class CustomResponseOutputTypeDef(
-    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -1955,23 +1745,14 @@
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GeoMatchStatementOutputTypeDef = TypedDict(
-    "GeoMatchStatementOutputTypeDef",
-    {
-        "CountryCodes": List[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
-    },
-    total=False,
-)
-
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
@@ -2004,23 +1785,14 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
-HeadersOutputTypeDef = TypedDict(
-    "HeadersOutputTypeDef",
-    {
-        "MatchPattern": HeaderMatchPatternOutputTypeDef,
-        "MatchScope": MapMatchScopeType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -2043,35 +1815,14 @@
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
 
-_RequiredJsonBodyOutputTypeDef = TypedDict(
-    "_RequiredJsonBodyOutputTypeDef",
-    {
-        "MatchPattern": JsonMatchPatternOutputTypeDef,
-        "MatchScope": JsonMatchScopeType,
-    },
-)
-_OptionalJsonBodyOutputTypeDef = TypedDict(
-    "_OptionalJsonBodyOutputTypeDef",
-    {
-        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-    total=False,
-)
-
-
-class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
-    pass
-
-
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -2155,39 +1906,14 @@
 )
 
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
 
-_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
-    "_RequiredRequestInspectionACFPOutputTypeDef",
-    {
-        "PayloadType": PayloadTypeType,
-    },
-)
-_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
-    "_OptionalRequestInspectionACFPOutputTypeDef",
-    {
-        "UsernameField": UsernameFieldTypeDef,
-        "PasswordField": PasswordFieldTypeDef,
-        "EmailField": EmailFieldTypeDef,
-        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
-        "AddressFields": List[AddressFieldTypeDef],
-    },
-    total=False,
-)
-
-
-class RequestInspectionACFPOutputTypeDef(
-    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
-):
-    pass
-
-
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -2231,25 +1957,14 @@
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseInspectionOutputTypeDef = TypedDict(
-    "ResponseInspectionOutputTypeDef",
-    {
-        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
-        "Header": ResponseInspectionHeaderOutputTypeDef,
-        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
-        "Json": ResponseInspectionJsonOutputTypeDef,
-    },
-    total=False,
-)
-
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
@@ -2273,60 +1988,36 @@
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": TimestampTypeDef,
     },
 )
 
-AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
-RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
-    "RateBasedStatementCustomKeyOutputTypeDef",
-    {
-        "Header": RateLimitHeaderOutputTypeDef,
-        "Cookie": RateLimitCookieOutputTypeDef,
-        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
-        "QueryString": RateLimitQueryStringOutputTypeDef,
-        "HTTPMethod": Dict[str, Any],
-        "ForwardedIP": Dict[str, Any],
-        "IP": Dict[str, Any],
-        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
-    },
-    total=False,
-)
-
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
         "HTTPMethod": Mapping[str, Any],
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+        "UriPath": RateLimitUriPathTypeDef,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Behavior": FilterBehaviorType,
-        "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": Sequence[ConditionTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
@@ -2348,46 +2039,14 @@
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AllowActionOutputTypeDef = TypedDict(
-    "AllowActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptchaActionOutputTypeDef = TypedDict(
-    "CaptchaActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-ChallengeActionOutputTypeDef = TypedDict(
-    "ChallengeActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-CountActionOutputTypeDef = TypedDict(
-    "CountActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
@@ -2412,22 +2071,14 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
-BlockActionOutputTypeDef = TypedDict(
-    "BlockActionOutputTypeDef",
-    {
-        "CustomResponse": CustomResponseOutputTypeDef,
-    },
-    total=False,
-)
-
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2458,32 +2109,14 @@
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
 
-FieldToMatchOutputTypeDef = TypedDict(
-    "FieldToMatchOutputTypeDef",
-    {
-        "SingleHeader": SingleHeaderTypeDef,
-        "SingleQueryArgument": SingleQueryArgumentTypeDef,
-        "AllQueryArguments": Dict[str, Any],
-        "UriPath": Dict[str, Any],
-        "QueryString": Dict[str, Any],
-        "Body": BodyTypeDef,
-        "Method": Dict[str, Any],
-        "JsonBody": JsonBodyOutputTypeDef,
-        "Headers": HeadersOutputTypeDef,
-        "Cookies": CookiesOutputTypeDef,
-        "HeaderOrder": HeaderOrderTypeDef,
-    },
-    total=False,
-)
-
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2503,62 +2136,14 @@
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
-    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
-    {
-        "CreationPath": str,
-        "RegistrationPagePath": str,
-        "RequestInspection": RequestInspectionACFPOutputTypeDef,
-    },
-)
-_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
-    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
-    {
-        "ResponseInspection": ResponseInspectionOutputTypeDef,
-        "EnableRegexInPath": bool,
-    },
-    total=False,
-)
-
-
-class AWSManagedRulesACFPRuleSetOutputTypeDef(
-    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
-    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
-):
-    pass
-
-
-_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
-    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
-    {
-        "LoginPath": str,
-    },
-)
-_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
-    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
-    {
-        "RequestInspection": RequestInspectionTypeDef,
-        "ResponseInspection": ResponseInspectionOutputTypeDef,
-        "EnableRegexInPath": bool,
-    },
-    total=False,
-)
-
-
-class AWSManagedRulesATPRuleSetOutputTypeDef(
-    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
-):
-    pass
-
-
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
     },
@@ -2609,118 +2194,55 @@
         "RuleMetricName": str,
         "Scope": ScopeType,
         "TimeWindow": TimeWindowTypeDef,
         "MaxItems": int,
     },
 )
 
-TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
-_RequiredRateBasedStatementOutputTypeDef = TypedDict(
-    "_RequiredRateBasedStatementOutputTypeDef",
-    {
-        "Limit": int,
-        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
-    },
-)
-_OptionalRateBasedStatementOutputTypeDef = TypedDict(
-    "_OptionalRateBasedStatementOutputTypeDef",
-    {
-        "ScopeDownStatement": "StatementOutputTypeDef",
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
-        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class RateBasedStatementOutputTypeDef(
-    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
-):
-    pass
-
-
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
     },
     total=False,
 )
 
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
 
-LoggingFilterOutputTypeDef = TypedDict(
-    "LoggingFilterOutputTypeDef",
-    {
-        "Filters": List[FilterOutputTypeDef],
-        "DefaultBehavior": FilterBehaviorType,
-    },
-)
-
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
+        "Filters": List[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
-OverrideActionOutputTypeDef = TypedDict(
-    "OverrideActionOutputTypeDef",
-    {
-        "Count": CountActionOutputTypeDef,
-        "None": Dict[str, Any],
-    },
-    total=False,
-)
-
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
 )
 
-DefaultActionOutputTypeDef = TypedDict(
-    "DefaultActionOutputTypeDef",
-    {
-        "Block": BlockActionOutputTypeDef,
-        "Allow": AllowActionOutputTypeDef,
-    },
-    total=False,
-)
-
-RuleActionOutputTypeDef = TypedDict(
-    "RuleActionOutputTypeDef",
-    {
-        "Block": BlockActionOutputTypeDef,
-        "Allow": AllowActionOutputTypeDef,
-        "Count": CountActionOutputTypeDef,
-        "Captcha": CaptchaActionOutputTypeDef,
-        "Challenge": ChallengeActionOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -2739,87 +2261,19 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowOutputTypeDef,
+        "TimeWindow": TimeWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ByteMatchStatementOutputTypeDef = TypedDict(
-    "ByteMatchStatementOutputTypeDef",
-    {
-        "SearchString": bytes,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
-RegexMatchStatementOutputTypeDef = TypedDict(
-    "RegexMatchStatementOutputTypeDef",
-    {
-        "RegexString": str,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
-    "RegexPatternSetReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-SizeConstraintStatementOutputTypeDef = TypedDict(
-    "SizeConstraintStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
-    "_RequiredSqliMatchStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
-    "_OptionalSqliMatchStatementOutputTypeDef",
-    {
-        "SensitivityLevel": SensitivityLevelType,
-    },
-    total=False,
-)
-
-
-class SqliMatchStatementOutputTypeDef(
-    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
-):
-    pass
-
-
-XssMatchStatementOutputTypeDef = TypedDict(
-    "XssMatchStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
@@ -2880,142 +2334,69 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-ManagedRuleGroupConfigOutputTypeDef = TypedDict(
-    "ManagedRuleGroupConfigOutputTypeDef",
-    {
-        "LoginPath": str,
-        "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldTypeDef,
-        "PasswordField": PasswordFieldTypeDef,
-        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
-        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
-        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
-    },
-    total=False,
-)
-
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
-_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationOutputTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchOutputTypeDef],
-        "ManagedByFirewallManager": bool,
-        "LoggingFilter": LoggingFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class LoggingConfigurationOutputTypeDef(
-    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": Sequence[str],
+        "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": Sequence[FieldToMatchTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
 
-RuleActionOverrideOutputTypeDef = TypedDict(
-    "RuleActionOverrideOutputTypeDef",
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
     {
         "Name": str,
-        "ActionToUse": RuleActionOutputTypeDef,
+        "ActionToUse": RuleActionTypeDef,
     },
 )
 
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Priority": int,
-        "Statement": "StatementOutputTypeDef",
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
-    {
-        "Action": RuleActionOutputTypeDef,
-        "OverrideAction": OverrideActionOutputTypeDef,
-        "RuleLabels": List[LabelTypeDef],
-        "CaptchaConfig": CaptchaConfigTypeDef,
-        "ChallengeConfig": ChallengeConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
-    pass
-
-
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionOutputTypeDef,
+        "Action": RuleActionTypeDef,
     },
     total=False,
 )
 
-DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
-    {
-        "Name": str,
-        "ActionToUse": RuleActionTypeDef,
-    },
-)
-
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -3037,133 +2418,39 @@
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
-    "_RequiredManagedRuleGroupStatementOutputTypeDef",
-    {
-        "VendorName": str,
-        "Name": str,
-    },
-)
-_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
-    "_OptionalManagedRuleGroupStatementOutputTypeDef",
-    {
-        "Version": str,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-        "ScopeDownStatement": "StatementOutputTypeDef",
-        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
-        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class ManagedRuleGroupStatementOutputTypeDef(
-    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
-):
-    pass
-
-
-_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
-    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-    },
-)
-_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
-    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
-    {
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class RuleGroupReferenceStatementOutputTypeDef(
-    _RequiredRuleGroupReferenceStatementOutputTypeDef,
-    _OptionalRuleGroupReferenceStatementOutputTypeDef,
-):
-    pass
-
-
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleOutputTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
-
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
@@ -3208,82 +2495,33 @@
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
-        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
-        "XssMatchStatement": XssMatchStatementOutputTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
-        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
     {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3292,15 +2530,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
@@ -3319,15 +2557,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3337,29 +2575,57 @@
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
+
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
 class UpdateRuleGroupRequestRequestTypeDef(
@@ -3379,15 +2645,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
@@ -3396,50 +2662,90 @@
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
 
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
+    {
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+    },
+    total=False,
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionOutputTypeDef,
+        "OverrideAction": OverrideActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionOutputTypeDef,
+        "DefaultAction": DefaultActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigOutputTypeDef,
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.pyi` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -55,27 +55,25 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
-    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
-    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
@@ -110,22 +108,19 @@
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
-    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
-    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
@@ -141,41 +136,32 @@
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
-    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RateLimitLabelNamespaceTypeDef",
-    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
-    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
-    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
-    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
-    "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
-    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
-    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
-    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
+    "RateLimitUriPathTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
     "CheckCapacityResponseTypeDef",
     "CreateAPIKeyResponseTypeDef",
     "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyResponseTypeDef",
@@ -185,15 +171,14 @@
     "PutManagedRuleSetVersionsResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "ConditionTypeDef",
-    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
@@ -202,125 +187,85 @@
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
-    "CustomRequestHandlingOutputTypeDef",
     "CustomRequestHandlingTypeDef",
-    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
-    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     "HTTPRequestTypeDef",
-    "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
-    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
-    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
-    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
     "TimeWindowTypeDef",
     "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "AssociationConfigUnionTypeDef",
-    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
-    "AllowActionOutputTypeDef",
-    "CaptchaActionOutputTypeDef",
-    "ChallengeActionOutputTypeDef",
-    "CountActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
-    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
-    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
-    "AWSManagedRulesACFPRuleSetOutputTypeDef",
-    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
-    "TimeWindowUnionTypeDef",
-    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
-    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
-    "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
-    "DefaultActionOutputTypeDef",
-    "RuleActionOutputTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
-    "ByteMatchStatementOutputTypeDef",
-    "RegexMatchStatementOutputTypeDef",
-    "RegexPatternSetReferenceStatementOutputTypeDef",
-    "SizeConstraintStatementOutputTypeDef",
-    "SqliMatchStatementOutputTypeDef",
-    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
-    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideOutputTypeDef",
-    "RuleOutputTypeDef",
-    "RuleSummaryTypeDef",
-    "DefaultActionUnionTypeDef",
     "RuleActionOverrideTypeDef",
+    "RuleSummaryTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
-    "ManagedRuleGroupStatementOutputTypeDef",
-    "RuleGroupReferenceStatementOutputTypeDef",
-    "RuleGroupTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
+    "PutLoggingConfigurationResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "RuleUnionTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementOutputTypeDef",
-    "GetRuleGroupResponseTypeDef",
-    "StatementTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
+    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementTypeDef",
+    "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -351,21 +296,14 @@
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
-AndStatementOutputTypeDef = TypedDict(
-    "AndStatementOutputTypeDef",
-    {
-        "Statements": List["StatementOutputTypeDef"],
-    },
-)
-
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -442,24 +380,14 @@
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
-CookieMatchPatternOutputTypeDef = TypedDict(
-    "CookieMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedCookies": List[str],
-        "ExcludedCookies": List[str],
-    },
-    total=False,
-)
-
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -861,22 +789,14 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowOutputTypeDef = TypedDict(
-    "TimeWindowOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-)
-
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -894,24 +814,14 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-HeaderMatchPatternOutputTypeDef = TypedDict(
-    "HeaderMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedHeaders": List[str],
-        "ExcludedHeaders": List[str],
-    },
-    total=False,
-)
-
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
@@ -923,23 +833,14 @@
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
-JsonMatchPatternOutputTypeDef = TypedDict(
-    "JsonMatchPatternOutputTypeDef",
-    {
-        "All": Dict[str, Any],
-        "IncludedPaths": List[str],
-    },
-    total=False,
-)
-
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
@@ -1277,22 +1178,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
-    },
-)
-
-OrStatementOutputTypeDef = TypedDict(
-    "OrStatementOutputTypeDef",
-    {
-        "Statements": List[Dict[str, Any]],
+        "Statement": Dict[str, Any],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1326,74 +1220,40 @@
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
-ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
-    "ResponseInspectionBodyContainsOutputTypeDef",
-    {
-        "SuccessStrings": List[str],
-        "FailureStrings": List[str],
-    },
-)
-
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
-ResponseInspectionHeaderOutputTypeDef = TypedDict(
-    "ResponseInspectionHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "SuccessValues": List[str],
-        "FailureValues": List[str],
-    },
-)
-
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionJsonOutputTypeDef = TypedDict(
-    "ResponseInspectionJsonOutputTypeDef",
-    {
-        "Identifier": str,
-        "SuccessValues": List[str],
-        "FailureValues": List[str],
-    },
-)
-
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeOutputTypeDef",
-    {
-        "SuccessCodes": List[int],
-        "FailureCodes": List[int],
-    },
-)
-
 ResponseInspectionStatusCodeTypeDef = TypedDict(
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
     },
 )
@@ -1426,89 +1286,57 @@
 )
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
-AssociationConfigOutputTypeDef = TypedDict(
-    "AssociationConfigOutputTypeDef",
-    {
-        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
-    },
-    total=False,
-)
-
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
         "RequestBody": Mapping[
             Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
         ],
     },
     total=False,
 )
 
-RateLimitCookieOutputTypeDef = TypedDict(
-    "RateLimitCookieOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderOutputTypeDef = TypedDict(
-    "RateLimitHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitHeaderTypeDef = TypedDict(
     "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryArgumentOutputTypeDef = TypedDict(
-    "RateLimitQueryArgumentOutputTypeDef",
-    {
-        "Name": str,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringOutputTypeDef = TypedDict(
-    "RateLimitQueryStringOutputTypeDef",
+RateLimitQueryStringTypeDef = TypedDict(
+    "RateLimitQueryStringTypeDef",
     {
-        "TextTransformations": List[TextTransformationTypeDef],
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitQueryStringTypeDef = TypedDict(
-    "RateLimitQueryStringTypeDef",
+RateLimitUriPathTypeDef = TypedDict(
+    "RateLimitUriPathTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
 CaptchaConfigTypeDef = TypedDict(
     "CaptchaConfigTypeDef",
@@ -1648,23 +1476,14 @@
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
-CookiesOutputTypeDef = TypedDict(
-    "CookiesOutputTypeDef",
-    {
-        "MatchPattern": CookieMatchPatternOutputTypeDef,
-        "MatchScope": MapMatchScopeType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1844,48 +1663,21 @@
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomRequestHandlingOutputTypeDef = TypedDict(
-    "CustomRequestHandlingOutputTypeDef",
-    {
-        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
-    },
-)
-
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
-_RequiredCustomResponseOutputTypeDef = TypedDict(
-    "_RequiredCustomResponseOutputTypeDef",
-    {
-        "ResponseCode": int,
-    },
-)
-_OptionalCustomResponseOutputTypeDef = TypedDict(
-    "_OptionalCustomResponseOutputTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
-    },
-    total=False,
-)
-
-class CustomResponseOutputTypeDef(
-    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
-):
-    pass
-
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -1912,23 +1704,14 @@
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GeoMatchStatementOutputTypeDef = TypedDict(
-    "GeoMatchStatementOutputTypeDef",
-    {
-        "CountryCodes": List[CountryCodeType],
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
-    },
-    total=False,
-)
-
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
@@ -1961,23 +1744,14 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
-HeadersOutputTypeDef = TypedDict(
-    "HeadersOutputTypeDef",
-    {
-        "MatchPattern": HeaderMatchPatternOutputTypeDef,
-        "MatchScope": MapMatchScopeType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-)
-
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1998,33 +1772,14 @@
 )
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
-_RequiredJsonBodyOutputTypeDef = TypedDict(
-    "_RequiredJsonBodyOutputTypeDef",
-    {
-        "MatchPattern": JsonMatchPatternOutputTypeDef,
-        "MatchScope": JsonMatchScopeType,
-    },
-)
-_OptionalJsonBodyOutputTypeDef = TypedDict(
-    "_OptionalJsonBodyOutputTypeDef",
-    {
-        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
-        "OversizeHandling": OversizeHandlingType,
-    },
-    total=False,
-)
-
-class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
-    pass
-
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -2104,37 +1859,14 @@
     },
     total=False,
 )
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
-_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
-    "_RequiredRequestInspectionACFPOutputTypeDef",
-    {
-        "PayloadType": PayloadTypeType,
-    },
-)
-_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
-    "_OptionalRequestInspectionACFPOutputTypeDef",
-    {
-        "UsernameField": UsernameFieldTypeDef,
-        "PasswordField": PasswordFieldTypeDef,
-        "EmailField": EmailFieldTypeDef,
-        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
-        "AddressFields": List[AddressFieldTypeDef],
-    },
-    total=False,
-)
-
-class RequestInspectionACFPOutputTypeDef(
-    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
-):
-    pass
-
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -2174,25 +1906,14 @@
 
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
-ResponseInspectionOutputTypeDef = TypedDict(
-    "ResponseInspectionOutputTypeDef",
-    {
-        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
-        "Header": ResponseInspectionHeaderOutputTypeDef,
-        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
-        "Json": ResponseInspectionJsonOutputTypeDef,
-    },
-    total=False,
-)
-
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
@@ -2216,60 +1937,36 @@
         "Id": str,
         "LockToken": str,
         "VersionToExpire": str,
         "ExpiryTimestamp": TimestampTypeDef,
     },
 )
 
-AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
-RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
-    "RateBasedStatementCustomKeyOutputTypeDef",
-    {
-        "Header": RateLimitHeaderOutputTypeDef,
-        "Cookie": RateLimitCookieOutputTypeDef,
-        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
-        "QueryString": RateLimitQueryStringOutputTypeDef,
-        "HTTPMethod": Dict[str, Any],
-        "ForwardedIP": Dict[str, Any],
-        "IP": Dict[str, Any],
-        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
-    },
-    total=False,
-)
-
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
         "HTTPMethod": Mapping[str, Any],
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+        "UriPath": RateLimitUriPathTypeDef,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Behavior": FilterBehaviorType,
-        "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": Sequence[ConditionTypeDef],
+        "Conditions": List[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
@@ -2291,46 +1988,14 @@
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AllowActionOutputTypeDef = TypedDict(
-    "AllowActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-CaptchaActionOutputTypeDef = TypedDict(
-    "CaptchaActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-ChallengeActionOutputTypeDef = TypedDict(
-    "ChallengeActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
-CountActionOutputTypeDef = TypedDict(
-    "CountActionOutputTypeDef",
-    {
-        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
-    },
-    total=False,
-)
-
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
@@ -2355,22 +2020,14 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
-BlockActionOutputTypeDef = TypedDict(
-    "BlockActionOutputTypeDef",
-    {
-        "CustomResponse": CustomResponseOutputTypeDef,
-    },
-    total=False,
-)
-
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2399,32 +2056,14 @@
 )
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
-FieldToMatchOutputTypeDef = TypedDict(
-    "FieldToMatchOutputTypeDef",
-    {
-        "SingleHeader": SingleHeaderTypeDef,
-        "SingleQueryArgument": SingleQueryArgumentTypeDef,
-        "AllQueryArguments": Dict[str, Any],
-        "UriPath": Dict[str, Any],
-        "QueryString": Dict[str, Any],
-        "Body": BodyTypeDef,
-        "Method": Dict[str, Any],
-        "JsonBody": JsonBodyOutputTypeDef,
-        "Headers": HeadersOutputTypeDef,
-        "Cookies": CookiesOutputTypeDef,
-        "HeaderOrder": HeaderOrderTypeDef,
-    },
-    total=False,
-)
-
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2444,58 +2083,14 @@
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
-    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
-    {
-        "CreationPath": str,
-        "RegistrationPagePath": str,
-        "RequestInspection": RequestInspectionACFPOutputTypeDef,
-    },
-)
-_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
-    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
-    {
-        "ResponseInspection": ResponseInspectionOutputTypeDef,
-        "EnableRegexInPath": bool,
-    },
-    total=False,
-)
-
-class AWSManagedRulesACFPRuleSetOutputTypeDef(
-    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
-    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
-):
-    pass
-
-_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
-    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
-    {
-        "LoginPath": str,
-    },
-)
-_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
-    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
-    {
-        "RequestInspection": RequestInspectionTypeDef,
-        "ResponseInspection": ResponseInspectionOutputTypeDef,
-        "EnableRegexInPath": bool,
-    },
-    total=False,
-)
-
-class AWSManagedRulesATPRuleSetOutputTypeDef(
-    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
-):
-    pass
-
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
     },
@@ -2542,114 +2137,53 @@
         "RuleMetricName": str,
         "Scope": ScopeType,
         "TimeWindow": TimeWindowTypeDef,
         "MaxItems": int,
     },
 )
 
-TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
-_RequiredRateBasedStatementOutputTypeDef = TypedDict(
-    "_RequiredRateBasedStatementOutputTypeDef",
-    {
-        "Limit": int,
-        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
-    },
-)
-_OptionalRateBasedStatementOutputTypeDef = TypedDict(
-    "_OptionalRateBasedStatementOutputTypeDef",
-    {
-        "ScopeDownStatement": "StatementOutputTypeDef",
-        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
-        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
-    },
-    total=False,
-)
-
-class RateBasedStatementOutputTypeDef(
-    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
-):
-    pass
-
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
     },
     total=False,
 )
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
-LoggingFilterOutputTypeDef = TypedDict(
-    "LoggingFilterOutputTypeDef",
-    {
-        "Filters": List[FilterOutputTypeDef],
-        "DefaultBehavior": FilterBehaviorType,
-    },
-)
-
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
+        "Filters": List[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
-OverrideActionOutputTypeDef = TypedDict(
-    "OverrideActionOutputTypeDef",
-    {
-        "Count": CountActionOutputTypeDef,
-        "None": Dict[str, Any],
-    },
-    total=False,
-)
-
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
 )
 
-DefaultActionOutputTypeDef = TypedDict(
-    "DefaultActionOutputTypeDef",
-    {
-        "Block": BlockActionOutputTypeDef,
-        "Allow": AllowActionOutputTypeDef,
-    },
-    total=False,
-)
-
-RuleActionOutputTypeDef = TypedDict(
-    "RuleActionOutputTypeDef",
-    {
-        "Block": BlockActionOutputTypeDef,
-        "Allow": AllowActionOutputTypeDef,
-        "Count": CountActionOutputTypeDef,
-        "Captcha": CaptchaActionOutputTypeDef,
-        "Challenge": ChallengeActionOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -2668,85 +2202,19 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowOutputTypeDef,
+        "TimeWindow": TimeWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ByteMatchStatementOutputTypeDef = TypedDict(
-    "ByteMatchStatementOutputTypeDef",
-    {
-        "SearchString": bytes,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
-RegexMatchStatementOutputTypeDef = TypedDict(
-    "RegexMatchStatementOutputTypeDef",
-    {
-        "RegexString": str,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
-    "RegexPatternSetReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-SizeConstraintStatementOutputTypeDef = TypedDict(
-    "SizeConstraintStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
-_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
-    "_RequiredSqliMatchStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
-    "_OptionalSqliMatchStatementOutputTypeDef",
-    {
-        "SensitivityLevel": SensitivityLevelType,
-    },
-    total=False,
-)
-
-class SqliMatchStatementOutputTypeDef(
-    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
-):
-    pass
-
-XssMatchStatementOutputTypeDef = TypedDict(
-    "XssMatchStatementOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchOutputTypeDef,
-        "TextTransformations": List[TextTransformationTypeDef],
-    },
-)
-
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
         "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
@@ -2805,136 +2273,67 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-ManagedRuleGroupConfigOutputTypeDef = TypedDict(
-    "ManagedRuleGroupConfigOutputTypeDef",
-    {
-        "LoginPath": str,
-        "PayloadType": PayloadTypeType,
-        "UsernameField": UsernameFieldTypeDef,
-        "PasswordField": PasswordFieldTypeDef,
-        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
-        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
-        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
-    },
-    total=False,
-)
-
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
-_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationOutputTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchOutputTypeDef],
-        "ManagedByFirewallManager": bool,
-        "LoggingFilter": LoggingFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-class LoggingConfigurationOutputTypeDef(
-    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": Sequence[str],
+        "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": Sequence[FieldToMatchTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
-RuleActionOverrideOutputTypeDef = TypedDict(
-    "RuleActionOverrideOutputTypeDef",
-    {
-        "Name": str,
-        "ActionToUse": RuleActionOutputTypeDef,
-    },
-)
-
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
     {
         "Name": str,
-        "Priority": int,
-        "Statement": "StatementOutputTypeDef",
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
-    {
-        "Action": RuleActionOutputTypeDef,
-        "OverrideAction": OverrideActionOutputTypeDef,
-        "RuleLabels": List[LabelTypeDef],
-        "CaptchaConfig": CaptchaConfigTypeDef,
-        "ChallengeConfig": ChallengeConfigTypeDef,
+        "ActionToUse": RuleActionTypeDef,
     },
-    total=False,
 )
 
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
-    pass
-
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionOutputTypeDef,
+        "Action": RuleActionTypeDef,
     },
     total=False,
 )
 
-DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
-    {
-        "Name": str,
-        "ActionToUse": RuleActionTypeDef,
-    },
-)
-
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2954,127 +2353,39 @@
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
-    {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
-    "_RequiredManagedRuleGroupStatementOutputTypeDef",
-    {
-        "VendorName": str,
-        "Name": str,
-    },
-)
-_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
-    "_OptionalManagedRuleGroupStatementOutputTypeDef",
-    {
-        "Version": str,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-        "ScopeDownStatement": "StatementOutputTypeDef",
-        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
-        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
-    },
-    total=False,
-)
-
-class ManagedRuleGroupStatementOutputTypeDef(
-    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
-):
-    pass
-
-_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
-    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
-    {
-        "ARN": str,
-    },
-)
-_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
-    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
-    {
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
-    },
-    total=False,
-)
-
-class RuleGroupReferenceStatementOutputTypeDef(
-    _RequiredRuleGroupReferenceStatementOutputTypeDef,
-    _OptionalRuleGroupReferenceStatementOutputTypeDef,
-):
-    pass
-
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleOutputTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
@@ -3115,82 +2426,33 @@
 )
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
-        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
-        "XssMatchStatement": XssMatchStatementOutputTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
-        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
     {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3199,15 +2461,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
@@ -3224,15 +2486,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3240,29 +2502,55 @@
 )
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
@@ -3280,65 +2568,105 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
+    {
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+    },
+    total=False,
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionOutputTypeDef,
+        "OverrideAction": OverrideActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionOutputTypeDef,
+        "DefaultAction": DefaultActionTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigOutputTypeDef,
+        "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/SOURCES.txt` & `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

