# Comparing `tmp/types-aiobotocore-elbv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elbv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elbv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-elbv2-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:52 2023, max compression
```

## Comparing `types-aiobotocore-elbv2-2.5.2.post1.tar` & `types-aiobotocore-elbv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35935 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43710 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-08-02 14:38:22.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-02 14:38:21.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.649589 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:16.000000 types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.636150 types-aiobotocore-elbv2-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-08-04 12:00:52.632150 types-aiobotocore-elbv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:52.636150 types-aiobotocore-elbv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-04 11:45:49.000000 types-aiobotocore-elbv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.628150 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35950 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38622 2023-08-04 11:45:51.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38581 2023-08-04 11:45:51.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-04 11:45:50.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.632150 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:00:52.000000 types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/LICENSE` & `types-aiobotocore-elbv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/setup.py` & `types-aiobotocore-elbv2-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elbv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__init__.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/__main__.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
+    ActionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -59,15 +59,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionUnionTypeDef,
+    RuleConditionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -194,15 +194,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#close)
         """
 
     async def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionUnionTypeDef],
+        DefaultActions: Sequence[ActionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -235,17 +235,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
         """
 
     async def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionUnionTypeDef],
+        Conditions: Sequence[RuleConditionTypeDef],
         Priority: int,
-        Actions: Sequence[ActionUnionTypeDef],
+        Actions: Sequence[ActionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
@@ -478,15 +478,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
+        DefaultActions: Sequence[ActionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
@@ -503,16 +503,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_load_balancer_attributes)
         """
 
     async def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
-        Actions: Sequence[ActionUnionTypeDef] = ...
+        Conditions: Sequence[RuleConditionTypeDef] = ...,
+        Actions: Sequence[ActionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/client.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     DescribeListenersPaginator,
     DescribeLoadBalancersPaginator,
     DescribeRulesPaginator,
     DescribeSSLPoliciesPaginator,
     DescribeTargetGroupsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
+    ActionTypeDef,
     AddListenerCertificatesOutputTypeDef,
     CertificateTypeDef,
     CreateListenerOutputTypeDef,
     CreateLoadBalancerOutputTypeDef,
     CreateRuleOutputTypeDef,
     CreateTargetGroupOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
@@ -59,15 +59,15 @@
     LoadBalancerAttributeTypeDef,
     MatcherTypeDef,
     ModifyListenerOutputTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     ModifyRuleOutputTypeDef,
     ModifyTargetGroupAttributesOutputTypeDef,
     ModifyTargetGroupOutputTypeDef,
-    RuleConditionUnionTypeDef,
+    RuleConditionTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeOutputTypeDef,
     SetRulePrioritiesOutputTypeDef,
     SetSecurityGroupsOutputTypeDef,
     SetSubnetsOutputTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
@@ -185,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#close)
         """
     async def create_listener(
         self,
         *,
         LoadBalancerArn: str,
-        DefaultActions: Sequence[ActionUnionTypeDef],
+        DefaultActions: Sequence[ActionTypeDef],
         Protocol: ProtocolEnumType = ...,
         Port: int = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateListenerOutputTypeDef:
@@ -224,17 +224,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_load_balancer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_load_balancer)
         """
     async def create_rule(
         self,
         *,
         ListenerArn: str,
-        Conditions: Sequence[RuleConditionUnionTypeDef],
+        Conditions: Sequence[RuleConditionTypeDef],
         Priority: int,
-        Actions: Sequence[ActionUnionTypeDef],
+        Actions: Sequence[ActionTypeDef],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateRuleOutputTypeDef:
         """
         Creates a rule for the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#create_rule)
@@ -448,15 +448,15 @@
         self,
         *,
         ListenerArn: str,
         Port: int = ...,
         Protocol: ProtocolEnumType = ...,
         SslPolicy: str = ...,
         Certificates: Sequence[CertificateTypeDef] = ...,
-        DefaultActions: Sequence[ActionUnionTypeDef] = ...,
+        DefaultActions: Sequence[ActionTypeDef] = ...,
         AlpnPolicy: Sequence[str] = ...
     ) -> ModifyListenerOutputTypeDef:
         """
         Replaces the specified properties of the specified listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_listener)
@@ -471,16 +471,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_load_balancer_attributes)
         """
     async def modify_rule(
         self,
         *,
         RuleArn: str,
-        Conditions: Sequence[RuleConditionUnionTypeDef] = ...,
-        Actions: Sequence[ActionUnionTypeDef] = ...
+        Conditions: Sequence[RuleConditionTypeDef] = ...,
+        Actions: Sequence[ActionTypeDef] = ...
     ) -> ModifyRuleOutputTypeDef:
         """
         Replaces the specified properties of the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Client.modify_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/client/#modify_rule)
         """
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/literals.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/paginator.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
+    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
 
-    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
+    data: AuthenticateCognitoActionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -34,20 +34,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AuthenticateCognitoActionConfigOutputTypeDef",
-    "AuthenticateOidcActionConfigOutputTypeDef",
-    "FixedResponseActionConfigTypeDef",
-    "RedirectActionConfigTypeDef",
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
+    "FixedResponseActionConfigTypeDef",
+    "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
@@ -69,26 +67,21 @@
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
-    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
-    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
-    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
-    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
     "RemoveListenerCertificatesInputRequestTypeDef",
@@ -123,107 +116,99 @@
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
-    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
-    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
     "TargetHealthDescriptionTypeDef",
     "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
-    "ActionUnionTypeDef",
+    "ModifyListenerInputRequestTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
     "RuleTypeDef",
-    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
-    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
 )
 
-_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
+_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
 )
-_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
+_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigTypeDef",
     {
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Dict[str, str],
+        "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
 
-class AuthenticateCognitoActionConfigOutputTypeDef(
-    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
-    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
+class AuthenticateCognitoActionConfigTypeDef(
+    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
 
-_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
+_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
     },
 )
-_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
+_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigTypeDef",
     {
         "ClientSecret": str,
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Dict[str, str],
+        "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
 
-class AuthenticateOidcActionConfigOutputTypeDef(
-    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
-    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
+class AuthenticateOidcActionConfigTypeDef(
+    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
 
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
@@ -267,72 +252,14 @@
 
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
 
-_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigTypeDef",
-    {
-        "UserPoolArn": str,
-        "UserPoolClientId": str,
-        "UserPoolDomain": str,
-    },
-)
-_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigTypeDef",
-    {
-        "SessionCookieName": str,
-        "Scope": str,
-        "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
-        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
-    },
-    total=False,
-)
-
-
-class AuthenticateCognitoActionConfigTypeDef(
-    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
-):
-    pass
-
-
-_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigTypeDef",
-    {
-        "Issuer": str,
-        "AuthorizationEndpoint": str,
-        "TokenEndpoint": str,
-        "UserInfoEndpoint": str,
-        "ClientId": str,
-    },
-)
-_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigTypeDef",
-    {
-        "ClientSecret": str,
-        "SessionCookieName": str,
-        "Scope": str,
-        "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
-        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
-        "UseExistingClientSecret": bool,
-    },
-    total=False,
-)
-
-
-class AuthenticateOidcActionConfigTypeDef(
-    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
-):
-    pass
-
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
@@ -627,56 +554,31 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
-HostHeaderConditionConfigOutputTypeDef = TypedDict(
-    "HostHeaderConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-HttpHeaderConditionConfigOutputTypeDef = TypedDict(
-    "HttpHeaderConditionConfigOutputTypeDef",
-    {
-        "HttpHeaderName": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
-    "HttpRequestMethodConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -686,22 +588,14 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-PathPatternConditionConfigOutputTypeDef = TypedDict(
-    "PathPatternConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -719,22 +613,14 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-SourceIpConditionConfigOutputTypeDef = TypedDict(
-    "SourceIpConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -1257,40 +1143,23 @@
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ForwardActionConfigOutputTypeDef = TypedDict(
-    "ForwardActionConfigOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTupleTypeDef],
-        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
-    },
-    total=False,
-)
-
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
-QueryStringConditionConfigOutputTypeDef = TypedDict(
-    "QueryStringConditionConfigOutputTypeDef",
-    {
-        "Values": List[QueryStringKeyValuePairTypeDef],
-    },
-    total=False,
-)
-
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1379,39 +1248,14 @@
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActionOutputTypeDef = TypedDict(
-    "_RequiredActionOutputTypeDef",
-    {
-        "Type": ActionTypeEnumType,
-    },
-)
-_OptionalActionOutputTypeDef = TypedDict(
-    "_OptionalActionOutputTypeDef",
-    {
-        "TargetGroupArn": str,
-        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
-        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
-        "Order": int,
-        "RedirectConfig": RedirectActionConfigTypeDef,
-        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
-        "ForwardConfig": ForwardActionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
-    pass
-
-
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
 _OptionalActionTypeDef = TypedDict(
@@ -1429,29 +1273,14 @@
 )
 
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
 
-RuleConditionOutputTypeDef = TypedDict(
-    "RuleConditionOutputTypeDef",
-    {
-        "Field": str,
-        "Values": List[str],
-        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
-        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
-        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
-        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
-        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
-        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1484,73 +1313,19 @@
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionOutputTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
-
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionOutputTypeDef],
-        "Actions": List[ActionOutputTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
-
-RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionUnionTypeDef],
+        "DefaultActions": Sequence[ActionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1565,80 +1340,62 @@
 
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
 
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionUnionTypeDef],
+        "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
 
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
-        "Actions": Sequence[ActionUnionTypeDef],
+        "Actions": Sequence[ActionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1657,18 +1414,89 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionUnionTypeDef],
-        "Actions": Sequence[ActionUnionTypeDef],
+        "Conditions": Sequence[RuleConditionTypeDef],
+        "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
+
+
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionTypeDef],
+        "Actions": List[ActionTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/type_defs.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for elbv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigOutputTypeDef
+    from types_aiobotocore_elbv2.type_defs import AuthenticateCognitoActionConfigTypeDef
 
-    data: AuthenticateCognitoActionConfigOutputTypeDef = ...
+    data: AuthenticateCognitoActionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionTypeEnumType,
     AuthenticateCognitoActionConditionalBehaviorEnumType,
     AuthenticateOidcActionConditionalBehaviorEnumType,
     IpAddressTypeType,
     LoadBalancerSchemeEnumType,
@@ -33,20 +33,18 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AuthenticateCognitoActionConfigOutputTypeDef",
-    "AuthenticateOidcActionConfigOutputTypeDef",
-    "FixedResponseActionConfigTypeDef",
-    "RedirectActionConfigTypeDef",
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
+    "FixedResponseActionConfigTypeDef",
+    "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
@@ -68,26 +66,21 @@
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
-    "HostHeaderConditionConfigOutputTypeDef",
     "HostHeaderConditionConfigTypeDef",
-    "HttpHeaderConditionConfigOutputTypeDef",
     "HttpHeaderConditionConfigTypeDef",
-    "HttpRequestMethodConditionConfigOutputTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
-    "PathPatternConditionConfigOutputTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "SourceIpConditionConfigOutputTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
     "RemoveListenerCertificatesInputRequestTypeDef",
@@ -122,104 +115,96 @@
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
     "DescribeTargetHealthInputTargetDeregisteredWaitTypeDef",
     "DescribeTargetHealthInputTargetInServiceWaitTypeDef",
     "DescribeTargetGroupAttributesOutputTypeDef",
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     "ModifyTargetGroupAttributesOutputTypeDef",
-    "ForwardActionConfigOutputTypeDef",
     "ForwardActionConfigTypeDef",
-    "QueryStringConditionConfigOutputTypeDef",
     "QueryStringConditionConfigTypeDef",
     "SetRulePrioritiesInputRequestTypeDef",
     "TargetHealthDescriptionTypeDef",
     "DescribeTagsOutputTypeDef",
     "LoadBalancerTypeDef",
     "SetSubnetsOutputTypeDef",
     "DescribeSSLPoliciesOutputTypeDef",
     "CreateTargetGroupOutputTypeDef",
     "DescribeTargetGroupsOutputTypeDef",
     "ModifyTargetGroupOutputTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "RuleConditionOutputTypeDef",
     "RuleConditionTypeDef",
     "DescribeTargetHealthOutputTypeDef",
     "CreateLoadBalancerOutputTypeDef",
     "DescribeLoadBalancersOutputTypeDef",
+    "CreateListenerInputRequestTypeDef",
     "ListenerTypeDef",
-    "ActionUnionTypeDef",
+    "ModifyListenerInputRequestTypeDef",
+    "CreateRuleInputRequestTypeDef",
+    "ModifyRuleInputRequestTypeDef",
     "RuleTypeDef",
-    "RuleConditionUnionTypeDef",
     "CreateListenerOutputTypeDef",
     "DescribeListenersOutputTypeDef",
     "ModifyListenerOutputTypeDef",
-    "CreateListenerInputRequestTypeDef",
-    "ModifyListenerInputRequestTypeDef",
     "CreateRuleOutputTypeDef",
     "DescribeRulesOutputTypeDef",
     "ModifyRuleOutputTypeDef",
     "SetRulePrioritiesOutputTypeDef",
-    "CreateRuleInputRequestTypeDef",
-    "ModifyRuleInputRequestTypeDef",
 )
 
-_RequiredAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigOutputTypeDef",
+_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateCognitoActionConfigTypeDef",
     {
         "UserPoolArn": str,
         "UserPoolClientId": str,
         "UserPoolDomain": str,
     },
 )
-_OptionalAuthenticateCognitoActionConfigOutputTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigOutputTypeDef",
+_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateCognitoActionConfigTypeDef",
     {
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Dict[str, str],
+        "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
-class AuthenticateCognitoActionConfigOutputTypeDef(
-    _RequiredAuthenticateCognitoActionConfigOutputTypeDef,
-    _OptionalAuthenticateCognitoActionConfigOutputTypeDef,
+class AuthenticateCognitoActionConfigTypeDef(
+    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
-_RequiredAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigOutputTypeDef",
+_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
     },
 )
-_OptionalAuthenticateOidcActionConfigOutputTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigOutputTypeDef",
+_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
+    "_OptionalAuthenticateOidcActionConfigTypeDef",
     {
         "ClientSecret": str,
         "SessionCookieName": str,
         "Scope": str,
         "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Dict[str, str],
+        "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
-class AuthenticateOidcActionConfigOutputTypeDef(
-    _RequiredAuthenticateOidcActionConfigOutputTypeDef,
-    _OptionalAuthenticateOidcActionConfigOutputTypeDef,
+class AuthenticateOidcActionConfigTypeDef(
+    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
@@ -258,68 +243,14 @@
 )
 
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
-_RequiredAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateCognitoActionConfigTypeDef",
-    {
-        "UserPoolArn": str,
-        "UserPoolClientId": str,
-        "UserPoolDomain": str,
-    },
-)
-_OptionalAuthenticateCognitoActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateCognitoActionConfigTypeDef",
-    {
-        "SessionCookieName": str,
-        "Scope": str,
-        "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
-        "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
-    },
-    total=False,
-)
-
-class AuthenticateCognitoActionConfigTypeDef(
-    _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
-):
-    pass
-
-_RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_RequiredAuthenticateOidcActionConfigTypeDef",
-    {
-        "Issuer": str,
-        "AuthorizationEndpoint": str,
-        "TokenEndpoint": str,
-        "UserInfoEndpoint": str,
-        "ClientId": str,
-    },
-)
-_OptionalAuthenticateOidcActionConfigTypeDef = TypedDict(
-    "_OptionalAuthenticateOidcActionConfigTypeDef",
-    {
-        "ClientSecret": str,
-        "SessionCookieName": str,
-        "Scope": str,
-        "SessionTimeout": int,
-        "AuthenticationRequestExtraParams": Mapping[str, str],
-        "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
-        "UseExistingClientSecret": bool,
-    },
-    total=False,
-)
-
-class AuthenticateOidcActionConfigTypeDef(
-    _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
-):
-    pass
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
@@ -608,56 +539,31 @@
     {
         "TargetGroupArn": str,
         "Weight": int,
     },
     total=False,
 )
 
-HostHeaderConditionConfigOutputTypeDef = TypedDict(
-    "HostHeaderConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HostHeaderConditionConfigTypeDef = TypedDict(
     "HostHeaderConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-HttpHeaderConditionConfigOutputTypeDef = TypedDict(
-    "HttpHeaderConditionConfigOutputTypeDef",
-    {
-        "HttpHeaderName": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HttpHeaderConditionConfigTypeDef = TypedDict(
     "HttpHeaderConditionConfigTypeDef",
     {
         "HttpHeaderName": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-HttpRequestMethodConditionConfigOutputTypeDef = TypedDict(
-    "HttpRequestMethodConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 HttpRequestMethodConditionConfigTypeDef = TypedDict(
     "HttpRequestMethodConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -667,22 +573,14 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
     },
     total=False,
 )
 
-PathPatternConditionConfigOutputTypeDef = TypedDict(
-    "PathPatternConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -700,22 +598,14 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
-SourceIpConditionConfigOutputTypeDef = TypedDict(
-    "SourceIpConditionConfigOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-    total=False,
-)
-
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -1222,40 +1112,23 @@
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ForwardActionConfigOutputTypeDef = TypedDict(
-    "ForwardActionConfigOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTupleTypeDef],
-        "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
-    },
-    total=False,
-)
-
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
         "TargetGroupStickinessConfig": TargetGroupStickinessConfigTypeDef,
     },
     total=False,
 )
 
-QueryStringConditionConfigOutputTypeDef = TypedDict(
-    "QueryStringConditionConfigOutputTypeDef",
-    {
-        "Values": List[QueryStringKeyValuePairTypeDef],
-    },
-    total=False,
-)
-
 QueryStringConditionConfigTypeDef = TypedDict(
     "QueryStringConditionConfigTypeDef",
     {
         "Values": Sequence[QueryStringKeyValuePairTypeDef],
     },
     total=False,
 )
@@ -1344,37 +1217,14 @@
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActionOutputTypeDef = TypedDict(
-    "_RequiredActionOutputTypeDef",
-    {
-        "Type": ActionTypeEnumType,
-    },
-)
-_OptionalActionOutputTypeDef = TypedDict(
-    "_OptionalActionOutputTypeDef",
-    {
-        "TargetGroupArn": str,
-        "AuthenticateOidcConfig": AuthenticateOidcActionConfigOutputTypeDef,
-        "AuthenticateCognitoConfig": AuthenticateCognitoActionConfigOutputTypeDef,
-        "Order": int,
-        "RedirectConfig": RedirectActionConfigTypeDef,
-        "FixedResponseConfig": FixedResponseActionConfigTypeDef,
-        "ForwardConfig": ForwardActionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class ActionOutputTypeDef(_RequiredActionOutputTypeDef, _OptionalActionOutputTypeDef):
-    pass
-
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
     },
 )
 _OptionalActionTypeDef = TypedDict(
@@ -1390,29 +1240,14 @@
     },
     total=False,
 )
 
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
-RuleConditionOutputTypeDef = TypedDict(
-    "RuleConditionOutputTypeDef",
-    {
-        "Field": str,
-        "Values": List[str],
-        "HostHeaderConfig": HostHeaderConditionConfigOutputTypeDef,
-        "PathPatternConfig": PathPatternConditionConfigOutputTypeDef,
-        "HttpHeaderConfig": HttpHeaderConditionConfigOutputTypeDef,
-        "QueryStringConfig": QueryStringConditionConfigOutputTypeDef,
-        "HttpRequestMethodConfig": HttpRequestMethodConditionConfigOutputTypeDef,
-        "SourceIpConfig": SourceIpConditionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1445,73 +1280,19 @@
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "LoadBalancerArn": str,
-        "Port": int,
-        "Protocol": ProtocolEnumType,
-        "Certificates": List[CertificateTypeDef],
-        "SslPolicy": str,
-        "DefaultActions": List[ActionOutputTypeDef],
-        "AlpnPolicy": List[str],
-    },
-    total=False,
-)
-
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
-    {
-        "RuleArn": str,
-        "Priority": str,
-        "Conditions": List[RuleConditionOutputTypeDef],
-        "Actions": List[ActionOutputTypeDef],
-        "IsDefault": bool,
-    },
-    total=False,
-)
-
-RuleConditionUnionTypeDef = Union[RuleConditionTypeDef, RuleConditionOutputTypeDef]
-CreateListenerOutputTypeDef = TypedDict(
-    "CreateListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeListenersOutputTypeDef = TypedDict(
-    "DescribeListenersOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyListenerOutputTypeDef = TypedDict(
-    "ModifyListenerOutputTypeDef",
-    {
-        "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
-        "DefaultActions": Sequence[ActionUnionTypeDef],
+        "DefaultActions": Sequence[ActionTypeDef],
     },
 )
 _OptionalCreateListenerInputRequestTypeDef = TypedDict(
     "_OptionalCreateListenerInputRequestTypeDef",
     {
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -1524,78 +1305,60 @@
 )
 
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "LoadBalancerArn": str,
+        "Port": int,
+        "Protocol": ProtocolEnumType,
+        "Certificates": List[CertificateTypeDef],
+        "SslPolicy": str,
+        "DefaultActions": List[ActionTypeDef],
+        "AlpnPolicy": List[str],
+    },
+    total=False,
+)
+
 _RequiredModifyListenerInputRequestTypeDef = TypedDict(
     "_RequiredModifyListenerInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalModifyListenerInputRequestTypeDef = TypedDict(
     "_OptionalModifyListenerInputRequestTypeDef",
     {
         "Port": int,
         "Protocol": ProtocolEnumType,
         "SslPolicy": str,
         "Certificates": Sequence[CertificateTypeDef],
-        "DefaultActions": Sequence[ActionUnionTypeDef],
+        "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
-CreateRuleOutputTypeDef = TypedDict(
-    "CreateRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRulesOutputTypeDef = TypedDict(
-    "DescribeRulesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyRuleOutputTypeDef = TypedDict(
-    "ModifyRuleOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRulePrioritiesOutputTypeDef = TypedDict(
-    "SetRulePrioritiesOutputTypeDef",
-    {
-        "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
-        "Conditions": Sequence[RuleConditionUnionTypeDef],
+        "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
-        "Actions": Sequence[ActionUnionTypeDef],
+        "Actions": Sequence[ActionTypeDef],
     },
 )
 _OptionalCreateRuleInputRequestTypeDef = TypedDict(
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -1612,17 +1375,87 @@
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
     "_OptionalModifyRuleInputRequestTypeDef",
     {
-        "Conditions": Sequence[RuleConditionUnionTypeDef],
-        "Actions": Sequence[ActionUnionTypeDef],
+        "Conditions": Sequence[RuleConditionTypeDef],
+        "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
+
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
+    {
+        "RuleArn": str,
+        "Priority": str,
+        "Conditions": List[RuleConditionTypeDef],
+        "Actions": List[ActionTypeDef],
+        "IsDefault": bool,
+    },
+    total=False,
+)
+
+CreateListenerOutputTypeDef = TypedDict(
+    "CreateListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeListenersOutputTypeDef = TypedDict(
+    "DescribeListenersOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyListenerOutputTypeDef = TypedDict(
+    "ModifyListenerOutputTypeDef",
+    {
+        "Listeners": List[ListenerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRuleOutputTypeDef = TypedDict(
+    "CreateRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRulesOutputTypeDef = TypedDict(
+    "DescribeRulesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyRuleOutputTypeDef = TypedDict(
+    "ModifyRuleOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRulePrioritiesOutputTypeDef = TypedDict(
+    "SetRulePrioritiesOutputTypeDef",
+    {
+        "Rules": List[RuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.py` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2/waiter.pyi` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post1/types_aiobotocore_elbv2.egg-info/SOURCES.txt` & `types-aiobotocore-elbv2-2.5.2.post2/types_aiobotocore_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

