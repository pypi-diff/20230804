# Comparing `tmp/types-aiobotocore-network-firewall-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-network-firewall-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-network-firewall-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-network-firewall-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-network-firewall-2.5.2.post1.tar` & `types-aiobotocore-network-firewall-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20704 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.297512 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34132 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34082 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-08-02 14:43:59.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55815 2023-08-02 14:44:02.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55749 2023-08-02 14:43:59.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:58.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.301512 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20704 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:43.000000 types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.496643 types-aiobotocore-network-firewall-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14086 2023-08-04 13:59:19.496643 types-aiobotocore-network-firewall-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12533 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.496643 types-aiobotocore-network-firewall-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2134 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.486643 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1672 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1671 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      977 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34077 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34027 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11115 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11113 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7191 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7184 2023-08-04 13:45:33.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47471 2023-08-04 13:45:34.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47415 2023-08-04 13:45:34.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:31.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.496643 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14086 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:19.000000 types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/LICENSE` & `types-aiobotocore-network-firewall-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/setup.py` & `types-aiobotocore-network-firewall-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-network-firewall",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NetworkFirewall 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__init__.pyi` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/__main__.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.NetworkFirewall 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyUnionTypeDef,
+    FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
-    RuleGroupUnionTypeDef,
+    LoggingConfigurationTypeDef,
+    RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationUnionTypeDef,
+    TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -189,15 +189,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
         """
 
     async def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyUnionTypeDef,
+        FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -208,15 +208,15 @@
 
     async def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupUnionTypeDef = ...,
+        RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -228,15 +228,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_rule_group)
         """
 
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -519,15 +519,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
 
     async def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyUnionTypeDef,
+        FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -554,30 +554,30 @@
         """
 
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
 
     async def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupUnionTypeDef = ...,
+        RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -604,15 +604,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
         """
 
     async def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/client.pyi` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyUnionTypeDef,
+    FirewallPolicyTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
-    RuleGroupUnionTypeDef,
+    LoggingConfigurationTypeDef,
+    RuleGroupTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationUnionTypeDef,
+    TLSInspectionConfigurationTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -179,15 +179,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_firewall)
         """
     async def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: FirewallPolicyUnionTypeDef,
+        FirewallPolicy: FirewallPolicyTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -197,15 +197,15 @@
         """
     async def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: RuleGroupUnionTypeDef = ...,
+        RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -216,15 +216,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#create_rule_group)
         """
     async def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -481,15 +481,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_encryption_configuration)
         """
     async def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: FirewallPolicyUnionTypeDef,
+        FirewallPolicy: FirewallPolicyTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -514,29 +514,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_firewall_policy_change_protection)
         """
     async def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
+        LoggingConfiguration: LoggingConfigurationTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_logging_configuration)
         """
     async def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: RuleGroupUnionTypeDef = ...,
+        RuleGroup: RuleGroupTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -561,15 +561,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_network_firewall/client/#update_subnet_change_protection)
         """
     async def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
+        TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
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
@@ -215,14 +216,15 @@
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
@@ -301,26 +303,28 @@
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
@@ -474,21 +478,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/literals.pyi` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -213,14 +214,15 @@
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
@@ -299,26 +301,28 @@
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
@@ -472,21 +476,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/paginator.pyi` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.py` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_network_firewall.type_defs import AddressTypeDef
 
     data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
@@ -74,37 +73,31 @@
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
-    "IPSetOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
     "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
     "ListFirewallsRequestRequestTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
-    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
     "PerObjectStatusTypeDef",
-    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
-    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
     "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
@@ -125,91 +118,69 @@
     "CreateFirewallRequestRequestTypeDef",
     "FirewallPolicyResponseTypeDef",
     "FirewallTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
-    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
-    "PolicyVariablesOutputTypeDef",
-    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
     "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "ServerCertificateScopeOutputTypeDef",
     "ServerCertificateScopeTypeDef",
-    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
-    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
-    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
-    "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
-    "ServerCertificateConfigurationOutputTypeDef",
+    "UpdateLoggingConfigurationResponseTypeDef",
     "ServerCertificateConfigurationTypeDef",
-    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
-    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
-    "TLSInspectionConfigurationOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
-    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
-    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
-    "TLSInspectionConfigurationUnionTypeDef",
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
-    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
-    "FirewallPolicyUnionTypeDef",
+    "DescribeFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
-    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
-    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
-    "RuleGroupUnionTypeDef",
+    "DescribeRuleGroupResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -228,22 +199,20 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
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
@@ -261,19 +230,17 @@
     "_OptionalSubnetMappingTypeDef",
     {
         "IPAddressType": IPAddressTypeType,
     },
     total=False,
 )
 
-
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -299,21 +266,19 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
-
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -461,22 +426,20 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
-
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -516,21 +479,14 @@
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
-IPSetOutputTypeDef = TypedDict(
-    "IPSetOutputTypeDef",
-    {
-        "Definition": List[str],
-    },
-)
-
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -621,105 +577,63 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
-LogDestinationConfigOutputTypeDef = TypedDict(
-    "LogDestinationConfigOutputTypeDef",
-    {
-        "LogType": LogTypeType,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
-    },
-)
-
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Mapping[str, str],
+        "LogDestination": Dict[str, str],
     },
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
-_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
-    "_RequiredTCPFlagFieldOutputTypeDef",
-    {
-        "Flags": List[TCPFlagType],
-    },
-)
-_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
-    "_OptionalTCPFlagFieldOutputTypeDef",
-    {
-        "Masks": List[TCPFlagType],
-    },
-    total=False,
-)
-
-
-class TCPFlagFieldOutputTypeDef(
-    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
-):
-    pass
-
-
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
     "_OptionalTCPFlagFieldTypeDef",
     {
         "Masks": Sequence[TCPFlagType],
     },
     total=False,
 )
 
-
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
-
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
 )
 
-PortSetOutputTypeDef = TypedDict(
-    "PortSetOutputTypeDef",
-    {
-        "Definition": List[str],
-    },
-    total=False,
-)
-
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -728,61 +642,31 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-_RequiredRuleOptionOutputTypeDef = TypedDict(
-    "_RequiredRuleOptionOutputTypeDef",
-    {
-        "Keyword": str,
-    },
-)
-_OptionalRuleOptionOutputTypeDef = TypedDict(
-    "_OptionalRuleOptionOutputTypeDef",
-    {
-        "Settings": List[str],
-    },
-    total=False,
-)
-
-
-class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
-    pass
-
-
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
     "_OptionalRuleOptionTypeDef",
     {
         "Settings": Sequence[str],
     },
     total=False,
 )
 
-
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
-
-RulesSourceListOutputTypeDef = TypedDict(
-    "RulesSourceListOutputTypeDef",
-    {
-        "Targets": List[str],
-        "TargetTypes": List[TargetTypeType],
-        "GeneratedRulesType": GeneratedRulesTypeType,
-    },
-)
-
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
@@ -835,22 +719,20 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
@@ -870,22 +752,20 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -894,22 +774,20 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateFirewallPolicyResponseTypeDef = TypedDict(
     "AssociateFirewallPolicyResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "UpdateToken": str,
@@ -981,21 +859,19 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
-
 class AssociateSubnetsRequestRequestTypeDef(
     _RequiredAssociateSubnetsRequestRequestTypeDef, _OptionalAssociateSubnetsRequestRequestTypeDef
 ):
     pass
 
-
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
@@ -1064,21 +940,19 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredFirewallPolicyResponseTypeDef = TypedDict(
     "_RequiredFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
     },
@@ -1094,21 +968,19 @@
         "NumberOfAssociations": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-
 class FirewallPolicyResponseTypeDef(
     _RequiredFirewallPolicyResponseTypeDef, _OptionalFirewallPolicyResponseTypeDef
 ):
     pass
 
-
 _RequiredFirewallTypeDef = TypedDict(
     "_RequiredFirewallTypeDef",
     {
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "FirewallId": str,
@@ -1125,19 +997,17 @@
         "Description": str,
         "Tags": List[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1173,42 +1043,33 @@
         "SourceMetadata": SourceMetadataTypeDef,
         "SnsTopic": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-
 class RuleGroupResponseTypeDef(
     _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
 ):
     pass
 
-
 DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
     "DescribeRuleGroupMetadataResponseTypeDef",
     {
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PublishMetricActionOutputTypeDef = TypedDict(
-    "PublishMetricActionOutputTypeDef",
-    {
-        "Dimensions": List[DimensionTypeDef],
-    },
-)
-
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
     },
 )
 
@@ -1226,30 +1087,14 @@
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyVariablesOutputTypeDef = TypedDict(
-    "PolicyVariablesOutputTypeDef",
-    {
-        "RuleVariables": Dict[str, IPSetOutputTypeDef],
-    },
-    total=False,
-)
-
-ReferenceSetsOutputTypeDef = TypedDict(
-    "ReferenceSetsOutputTypeDef",
-    {
-        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
-    },
-    total=False,
-)
-
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
@@ -1308,22 +1153,20 @@
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
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1334,65 +1177,33 @@
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
-    {
-        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
-    },
-)
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
-    },
-)
-
-ServerCertificateScopeOutputTypeDef = TypedDict(
-    "ServerCertificateScopeOutputTypeDef",
-    {
-        "Sources": List[AddressTypeDef],
-        "Destinations": List[AddressTypeDef],
-        "SourcePorts": List[PortRangeTypeDef],
-        "DestinationPorts": List[PortRangeTypeDef],
-        "Protocols": List[int],
+        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
     },
-    total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
-MatchAttributesOutputTypeDef = TypedDict(
-    "MatchAttributesOutputTypeDef",
-    {
-        "Sources": List[AddressTypeDef],
-        "Destinations": List[AddressTypeDef],
-        "SourcePorts": List[PortRangeTypeDef],
-        "DestinationPorts": List[PortRangeTypeDef],
-        "Protocols": List[int],
-        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
-    },
-    total=False,
-)
-
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1407,41 +1218,23 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
-RuleVariablesOutputTypeDef = TypedDict(
-    "RuleVariablesOutputTypeDef",
-    {
-        "IPSets": Dict[str, IPSetOutputTypeDef],
-        "PortSets": Dict[str, PortSetOutputTypeDef],
-    },
-    total=False,
-)
-
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
-StatefulRuleOutputTypeDef = TypedDict(
-    "StatefulRuleOutputTypeDef",
-    {
-        "Action": StatefulActionType,
-        "Header": HeaderTypeDef,
-        "RuleOptions": List[RuleOptionOutputTypeDef],
-    },
-)
-
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
@@ -1458,21 +1251,19 @@
     {
         "Priority": int,
         "Override": StatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
-
 class StatefulRuleGroupReferenceTypeDef(
     _RequiredStatefulRuleGroupReferenceTypeDef, _OptionalStatefulRuleGroupReferenceTypeDef
 ):
     pass
 
-
 _RequiredTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_RequiredTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfigurationId": str,
     },
@@ -1487,22 +1278,20 @@
         "NumberOfAssociations": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
-
 class TLSInspectionConfigurationResponseTypeDef(
     _RequiredTLSInspectionConfigurationResponseTypeDef,
     _OptionalTLSInspectionConfigurationResponseTypeDef,
 ):
     pass
 
-
 CapacityUsageSummaryTypeDef = TypedDict(
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
@@ -1555,88 +1344,60 @@
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionDefinitionOutputTypeDef = TypedDict(
-    "ActionDefinitionOutputTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
     },
     total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-ServerCertificateConfigurationOutputTypeDef = TypedDict(
-    "ServerCertificateConfigurationOutputTypeDef",
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
     {
-        "ServerCertificates": List[ServerCertificateTypeDef],
-        "Scopes": List[ServerCertificateScopeOutputTypeDef],
+        "FirewallArn": str,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionOutputTypeDef = TypedDict(
-    "RuleDefinitionOutputTypeDef",
-    {
-        "MatchAttributes": MatchAttributesOutputTypeDef,
-        "Actions": List[str],
-    },
-)
-
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
@@ -1679,59 +1440,33 @@
     {
         "SyncStates": Dict[str, SyncStateTypeDef],
         "CapacityUsageSummary": CapacityUsageSummaryTypeDef,
     },
     total=False,
 )
 
-
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
-
-CustomActionOutputTypeDef = TypedDict(
-    "CustomActionOutputTypeDef",
-    {
-        "ActionName": str,
-        "ActionDefinition": ActionDefinitionOutputTypeDef,
-    },
-)
-
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
-TLSInspectionConfigurationOutputTypeDef = TypedDict(
-    "TLSInspectionConfigurationOutputTypeDef",
-    {
-        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
-StatelessRuleOutputTypeDef = TypedDict(
-    "StatelessRuleOutputTypeDef",
-    {
-        "RuleDefinition": RuleDefinitionOutputTypeDef,
-        "Priority": int,
-    },
-)
-
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
@@ -1760,42 +1495,14 @@
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFirewallPolicyOutputTypeDef = TypedDict(
-    "_RequiredFirewallPolicyOutputTypeDef",
-    {
-        "StatelessDefaultActions": List[str],
-        "StatelessFragmentDefaultActions": List[str],
-    },
-)
-_OptionalFirewallPolicyOutputTypeDef = TypedDict(
-    "_OptionalFirewallPolicyOutputTypeDef",
-    {
-        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
-        "StatelessCustomActions": List[CustomActionOutputTypeDef],
-        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
-        "StatefulDefaultActions": List[str],
-        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
-        "TLSInspectionConfigurationArn": str,
-        "PolicyVariables": PolicyVariablesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FirewallPolicyOutputTypeDef(
-    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
 )
@@ -1809,29 +1516,17 @@
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
         "TLSInspectionConfigurationArn": str,
         "PolicyVariables": PolicyVariablesTypeDef,
     },
     total=False,
 )
 
-
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
-
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -1841,25 +1536,30 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-TLSInspectionConfigurationUnionTypeDef = Union[
-    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-]
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1870,75 +1570,39 @@
         "TLSInspectionConfigurationName": str,
         "Description": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "StatelessRules": List[StatelessRuleOutputTypeDef],
-    },
-)
-_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "CustomActions": List[CustomActionOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class StatelessRulesAndCustomActionsOutputTypeDef(
-    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
-    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
-):
-    pass
-
-
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_OptionalStatelessRulesAndCustomActionsTypeDef",
     {
         "CustomActions": Sequence[CustomActionTypeDef],
     },
     total=False,
 )
 
-
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
-
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1949,23 +1613,30 @@
         "Tags": Sequence[TagTypeDef],
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1977,65 +1648,31 @@
         "Description": str,
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-RulesSourceOutputTypeDef = TypedDict(
-    "RulesSourceOutputTypeDef",
-    {
-        "RulesString": str,
-        "RulesSourceList": RulesSourceListOutputTypeDef,
-        "StatefulRules": List[StatefulRuleOutputTypeDef],
-        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
-    },
-    total=False,
-)
-
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleGroupOutputTypeDef = TypedDict(
-    "_RequiredRuleGroupOutputTypeDef",
-    {
-        "RulesSource": RulesSourceOutputTypeDef,
-    },
-)
-_OptionalRuleGroupOutputTypeDef = TypedDict(
-    "_OptionalRuleGroupOutputTypeDef",
-    {
-        "RuleVariables": RuleVariablesOutputTypeDef,
-        "ReferenceSets": ReferenceSetsOutputTypeDef,
-        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
-    pass
-
-
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -2044,29 +1681,17 @@
         "RuleVariables": RuleVariablesTypeDef,
         "ReferenceSets": ReferenceSetsTypeDef,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
-
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupOutputTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
     },
@@ -2081,22 +1706,29 @@
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "SourceMetadata": SourceMetadataTypeDef,
     },
     total=False,
 )
 
-
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
@@ -2111,12 +1743,11 @@
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "SourceMetadata": SourceMetadataTypeDef,
     },
     total=False,
 )
 
-
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall/type_defs.pyi` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_network_firewall.type_defs import AddressTypeDef
 
     data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -43,14 +43,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
@@ -73,37 +74,31 @@
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
     "HeaderTypeDef",
-    "IPSetOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
     "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
     "ListFirewallsRequestRequestTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
     "PortRangeTypeDef",
-    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
     "PerObjectStatusTypeDef",
-    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
-    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
     "ServerCertificateTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
@@ -124,91 +119,69 @@
     "CreateFirewallRequestRequestTypeDef",
     "FirewallPolicyResponseTypeDef",
     "FirewallTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
-    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
-    "PolicyVariablesOutputTypeDef",
-    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
     "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "ServerCertificateScopeOutputTypeDef",
     "ServerCertificateScopeTypeDef",
-    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
-    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
-    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
-    "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
-    "ServerCertificateConfigurationOutputTypeDef",
+    "UpdateLoggingConfigurationResponseTypeDef",
     "ServerCertificateConfigurationTypeDef",
-    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
-    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
-    "TLSInspectionConfigurationOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
-    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
-    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
-    "TLSInspectionConfigurationUnionTypeDef",
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
-    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
-    "FirewallPolicyUnionTypeDef",
+    "DescribeFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
-    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
-    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
-    "RuleGroupUnionTypeDef",
+    "DescribeRuleGroupResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -227,20 +200,22 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
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
@@ -258,17 +233,19 @@
     "_OptionalSubnetMappingTypeDef",
     {
         "IPAddressType": IPAddressTypeType,
     },
     total=False,
 )
 
+
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -294,19 +271,21 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
+
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -454,20 +433,22 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
+
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -507,21 +488,14 @@
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
-IPSetOutputTypeDef = TypedDict(
-    "IPSetOutputTypeDef",
-    {
-        "Definition": List[str],
-    },
-)
-
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -612,99 +586,67 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-LogDestinationConfigOutputTypeDef = TypedDict(
-    "LogDestinationConfigOutputTypeDef",
-    {
-        "LogType": LogTypeType,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
-    },
-)
 
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Mapping[str, str],
+        "LogDestination": Dict[str, str],
     },
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
-_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
-    "_RequiredTCPFlagFieldOutputTypeDef",
-    {
-        "Flags": List[TCPFlagType],
-    },
-)
-_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
-    "_OptionalTCPFlagFieldOutputTypeDef",
-    {
-        "Masks": List[TCPFlagType],
-    },
-    total=False,
-)
-
-class TCPFlagFieldOutputTypeDef(
-    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
-):
-    pass
-
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
     "_OptionalTCPFlagFieldTypeDef",
     {
         "Masks": Sequence[TCPFlagType],
     },
     total=False,
 )
 
+
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
+
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
 )
 
-PortSetOutputTypeDef = TypedDict(
-    "PortSetOutputTypeDef",
-    {
-        "Definition": List[str],
-    },
-    total=False,
-)
-
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -713,56 +655,32 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-_RequiredRuleOptionOutputTypeDef = TypedDict(
-    "_RequiredRuleOptionOutputTypeDef",
-    {
-        "Keyword": str,
-    },
-)
-_OptionalRuleOptionOutputTypeDef = TypedDict(
-    "_OptionalRuleOptionOutputTypeDef",
-    {
-        "Settings": List[str],
-    },
-    total=False,
-)
-
-class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
-    pass
-
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
     "_OptionalRuleOptionTypeDef",
     {
         "Settings": Sequence[str],
     },
     total=False,
 )
 
+
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
-RulesSourceListOutputTypeDef = TypedDict(
-    "RulesSourceListOutputTypeDef",
-    {
-        "Targets": List[str],
-        "TargetTypes": List[TargetTypeType],
-        "GeneratedRulesType": GeneratedRulesTypeType,
-    },
-)
 
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
@@ -816,20 +734,22 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
@@ -849,20 +769,22 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -871,20 +793,22 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateFirewallPolicyResponseTypeDef = TypedDict(
     "AssociateFirewallPolicyResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "UpdateToken": str,
@@ -956,19 +880,21 @@
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
     },
     total=False,
 )
 
+
 class AssociateSubnetsRequestRequestTypeDef(
     _RequiredAssociateSubnetsRequestRequestTypeDef, _OptionalAssociateSubnetsRequestRequestTypeDef
 ):
     pass
 
+
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
@@ -1037,19 +963,21 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredFirewallPolicyResponseTypeDef = TypedDict(
     "_RequiredFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
     },
@@ -1065,19 +993,21 @@
         "NumberOfAssociations": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+
 class FirewallPolicyResponseTypeDef(
     _RequiredFirewallPolicyResponseTypeDef, _OptionalFirewallPolicyResponseTypeDef
 ):
     pass
 
+
 _RequiredFirewallTypeDef = TypedDict(
     "_RequiredFirewallTypeDef",
     {
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": List[SubnetMappingTypeDef],
         "FirewallId": str,
@@ -1094,17 +1024,19 @@
         "Description": str,
         "Tags": List[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1140,40 +1072,35 @@
         "SourceMetadata": SourceMetadataTypeDef,
         "SnsTopic": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+
 class RuleGroupResponseTypeDef(
     _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
 ):
     pass
 
+
 DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
     "DescribeRuleGroupMetadataResponseTypeDef",
     {
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PublishMetricActionOutputTypeDef = TypedDict(
-    "PublishMetricActionOutputTypeDef",
-    {
-        "Dimensions": List[DimensionTypeDef],
-    },
-)
-
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
     },
 )
 
@@ -1191,30 +1118,14 @@
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyVariablesOutputTypeDef = TypedDict(
-    "PolicyVariablesOutputTypeDef",
-    {
-        "RuleVariables": Dict[str, IPSetOutputTypeDef],
-    },
-    total=False,
-)
-
-ReferenceSetsOutputTypeDef = TypedDict(
-    "ReferenceSetsOutputTypeDef",
-    {
-        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
-    },
-    total=False,
-)
-
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
@@ -1273,20 +1184,22 @@
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
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1297,65 +1210,33 @@
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
-    {
-        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
-    },
-)
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
+        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
     },
 )
 
-ServerCertificateScopeOutputTypeDef = TypedDict(
-    "ServerCertificateScopeOutputTypeDef",
-    {
-        "Sources": List[AddressTypeDef],
-        "Destinations": List[AddressTypeDef],
-        "SourcePorts": List[PortRangeTypeDef],
-        "DestinationPorts": List[PortRangeTypeDef],
-        "Protocols": List[int],
-    },
-    total=False,
-)
-
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
-MatchAttributesOutputTypeDef = TypedDict(
-    "MatchAttributesOutputTypeDef",
-    {
-        "Sources": List[AddressTypeDef],
-        "Destinations": List[AddressTypeDef],
-        "SourcePorts": List[PortRangeTypeDef],
-        "DestinationPorts": List[PortRangeTypeDef],
-        "Protocols": List[int],
-        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
-    },
-    total=False,
-)
-
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1370,41 +1251,23 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
-RuleVariablesOutputTypeDef = TypedDict(
-    "RuleVariablesOutputTypeDef",
-    {
-        "IPSets": Dict[str, IPSetOutputTypeDef],
-        "PortSets": Dict[str, PortSetOutputTypeDef],
-    },
-    total=False,
-)
-
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
-StatefulRuleOutputTypeDef = TypedDict(
-    "StatefulRuleOutputTypeDef",
-    {
-        "Action": StatefulActionType,
-        "Header": HeaderTypeDef,
-        "RuleOptions": List[RuleOptionOutputTypeDef],
-    },
-)
-
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
@@ -1421,19 +1284,21 @@
     {
         "Priority": int,
         "Override": StatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
+
 class StatefulRuleGroupReferenceTypeDef(
     _RequiredStatefulRuleGroupReferenceTypeDef, _OptionalStatefulRuleGroupReferenceTypeDef
 ):
     pass
 
+
 _RequiredTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_RequiredTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfigurationId": str,
     },
@@ -1448,20 +1313,22 @@
         "NumberOfAssociations": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
+
 class TLSInspectionConfigurationResponseTypeDef(
     _RequiredTLSInspectionConfigurationResponseTypeDef,
     _OptionalTLSInspectionConfigurationResponseTypeDef,
 ):
     pass
 
+
 CapacityUsageSummaryTypeDef = TypedDict(
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
@@ -1514,88 +1381,60 @@
     {
         "UpdateToken": str,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionDefinitionOutputTypeDef = TypedDict(
-    "ActionDefinitionOutputTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionDefinitionTypeDef = TypedDict(
     "ActionDefinitionTypeDef",
     {
         "PublishMetricAction": PublishMetricActionTypeDef,
     },
     total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-ServerCertificateConfigurationOutputTypeDef = TypedDict(
-    "ServerCertificateConfigurationOutputTypeDef",
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
     {
-        "ServerCertificates": List[ServerCertificateTypeDef],
-        "Scopes": List[ServerCertificateScopeOutputTypeDef],
+        "FirewallArn": str,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionOutputTypeDef = TypedDict(
-    "RuleDefinitionOutputTypeDef",
-    {
-        "MatchAttributes": MatchAttributesOutputTypeDef,
-        "Actions": List[str],
-    },
-)
-
 RuleDefinitionTypeDef = TypedDict(
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
@@ -1638,57 +1477,35 @@
     {
         "SyncStates": Dict[str, SyncStateTypeDef],
         "CapacityUsageSummary": CapacityUsageSummaryTypeDef,
     },
     total=False,
 )
 
+
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
-CustomActionOutputTypeDef = TypedDict(
-    "CustomActionOutputTypeDef",
-    {
-        "ActionName": str,
-        "ActionDefinition": ActionDefinitionOutputTypeDef,
-    },
-)
 
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
-TLSInspectionConfigurationOutputTypeDef = TypedDict(
-    "TLSInspectionConfigurationOutputTypeDef",
-    {
-        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
-StatelessRuleOutputTypeDef = TypedDict(
-    "StatelessRuleOutputTypeDef",
-    {
-        "RuleDefinition": RuleDefinitionOutputTypeDef,
-        "Priority": int,
-    },
-)
-
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
@@ -1717,40 +1534,14 @@
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFirewallPolicyOutputTypeDef = TypedDict(
-    "_RequiredFirewallPolicyOutputTypeDef",
-    {
-        "StatelessDefaultActions": List[str],
-        "StatelessFragmentDefaultActions": List[str],
-    },
-)
-_OptionalFirewallPolicyOutputTypeDef = TypedDict(
-    "_OptionalFirewallPolicyOutputTypeDef",
-    {
-        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
-        "StatelessCustomActions": List[CustomActionOutputTypeDef],
-        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
-        "StatefulDefaultActions": List[str],
-        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
-        "TLSInspectionConfigurationArn": str,
-        "PolicyVariables": PolicyVariablesOutputTypeDef,
-    },
-    total=False,
-)
-
-class FirewallPolicyOutputTypeDef(
-    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
-):
-    pass
-
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
 )
@@ -1764,26 +1555,18 @@
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
         "TLSInspectionConfigurationArn": str,
         "PolicyVariables": PolicyVariablesTypeDef,
     },
     total=False,
 )
 
+
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
@@ -1794,23 +1577,32 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-TLSInspectionConfigurationUnionTypeDef = Union[
-    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-]
+
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1821,39 +1613,21 @@
         "TLSInspectionConfigurationName": str,
         "Description": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "StatelessRules": List[StatelessRuleOutputTypeDef],
-    },
-)
-_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "CustomActions": List[CustomActionOutputTypeDef],
-    },
-    total=False,
-)
-
-class StatelessRulesAndCustomActionsOutputTypeDef(
-    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
-    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
-):
-    pass
 
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
@@ -1861,28 +1635,20 @@
     "_OptionalStatelessRulesAndCustomActionsTypeDef",
     {
         "CustomActions": Sequence[CustomActionTypeDef],
     },
     total=False,
 )
 
+
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
@@ -1894,21 +1660,32 @@
         "Tags": Sequence[TagTypeDef],
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
+
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1920,61 +1697,33 @@
         "Description": str,
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-RulesSourceOutputTypeDef = TypedDict(
-    "RulesSourceOutputTypeDef",
-    {
-        "RulesString": str,
-        "RulesSourceList": RulesSourceListOutputTypeDef,
-        "StatefulRules": List[StatefulRuleOutputTypeDef],
-        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
-    },
-    total=False,
-)
 
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleGroupOutputTypeDef = TypedDict(
-    "_RequiredRuleGroupOutputTypeDef",
-    {
-        "RulesSource": RulesSourceOutputTypeDef,
-    },
-)
-_OptionalRuleGroupOutputTypeDef = TypedDict(
-    "_OptionalRuleGroupOutputTypeDef",
-    {
-        "RuleVariables": RuleVariablesOutputTypeDef,
-        "ReferenceSets": ReferenceSetsOutputTypeDef,
-        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
-    },
-    total=False,
-)
-
-class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
-    pass
-
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -1983,26 +1732,18 @@
         "RuleVariables": RuleVariablesTypeDef,
         "ReferenceSets": ReferenceSetsTypeDef,
         "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupOutputTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
@@ -2018,20 +1759,31 @@
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "SourceMetadata": SourceMetadataTypeDef,
     },
     total=False,
 )
 
+
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
-RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
+
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
@@ -2046,11 +1798,12 @@
         "DryRun": bool,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "SourceMetadata": SourceMetadataTypeDef,
     },
     total=False,
 )
 
+
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-network-firewall-2.5.2.post1/types_aiobotocore_network_firewall.egg-info/SOURCES.txt` & `types-aiobotocore-network-firewall-2.5.2.post2/types_aiobotocore_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

