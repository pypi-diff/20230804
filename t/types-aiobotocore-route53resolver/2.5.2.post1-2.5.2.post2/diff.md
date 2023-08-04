# Comparing `tmp/types-aiobotocore-route53resolver-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53resolver-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53resolver-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53resolver-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53resolver-2.5.2.post1.tar` & `types-aiobotocore-route53resolver-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.121474 types-aiobotocore-route53resolver-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:10.000000 types-aiobotocore-route53resolver-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-08-02 14:52:55.121474 types-aiobotocore-route53resolver-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-08-02 14:48:10.000000 types-aiobotocore-route53resolver-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.121474 types-aiobotocore-route53resolver-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:48:10.000000 types-aiobotocore-route53resolver-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.121474 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 14:48:10.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58137 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:11.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56931 2023-08-02 14:48:15.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56890 2023-08-02 14:48:12.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:10.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.121474 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-08-02 14:52:54.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:55.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:54.000000 types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16142 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14592 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2128 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4569 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4568 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      975 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    62209 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    62116 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14396 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14394 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21614 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21596 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61169 2023-08-04 13:51:21.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61124 2023-08-04 13:51:21.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16142 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/LICENSE` & `types-aiobotocore-route53resolver-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/setup.py` & `types-aiobotocore-route53resolver-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53resolver",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__init__.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         Client,
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -33,14 +34,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -52,14 +54,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -74,14 +77,15 @@
     "Client",
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__init__.pyi` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         Client,
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -33,14 +34,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -52,14 +54,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -73,14 +76,15 @@
     "Client",
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/__main__.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53Resolver 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
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

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/client.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -55,33 +56,36 @@
     AssociateFirewallRuleGroupResponseTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     AssociateResolverQueryLogConfigResponseTypeDef,
     AssociateResolverRuleResponseTypeDef,
     CreateFirewallDomainListResponseTypeDef,
     CreateFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteFirewallDomainListResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
     DisassociateResolverQueryLogConfigResponseTypeDef,
     DisassociateResolverRuleResponseTypeDef,
     FilterTypeDef,
     GetFirewallConfigResponseTypeDef,
     GetFirewallDomainListResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
     GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     GetResolverEndpointResponseTypeDef,
     GetResolverQueryLogConfigAssociationResponseTypeDef,
     GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     GetResolverRuleAssociationResponseTypeDef,
@@ -92,14 +96,15 @@
     IpAddressUpdateTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -112,14 +117,15 @@
     TagTypeDef,
     TargetAddressTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     UpdateResolverEndpointResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -150,14 +156,15 @@
     InvalidRequestException: Type[BotocoreClientError]
     InvalidTagException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class Route53ResolverClient(AioBaseClient):
     """
@@ -280,24 +287,43 @@
         Creates an empty DNS Firewall rule group for filtering DNS network traffic in a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_firewall_rule_group)
         """
 
+    async def create_outpost_resolver(
+        self,
+        *,
+        CreatorRequestId: str,
+        Name: str,
+        PreferredInstanceType: str,
+        OutpostArn: str,
+        InstanceCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateOutpostResolverResponseTypeDef:
+        """
+        Creates an Route 53 Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_outpost_resolver)
+        """
+
     async def create_resolver_endpoint(
         self,
         *,
         CreatorRequestId: str,
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ResolverEndpointType: ResolverEndpointTypeType = ...
+        ResolverEndpointType: ResolverEndpointTypeType = ...,
+        OutpostArn: str = ...,
+        PreferredInstanceType: str = ...
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_resolver_endpoint)
         """
@@ -364,14 +390,22 @@
         """
         Deletes the specified firewall rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#delete_firewall_rule_group)
         """
 
+    async def delete_outpost_resolver(self, *, Id: str) -> DeleteOutpostResolverResponseTypeDef:
+        """
+        Deletes a Resolver on the Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#delete_outpost_resolver)
+        """
+
     async def delete_resolver_endpoint(
         self, *, ResolverEndpointId: str
     ) -> DeleteResolverEndpointResponseTypeDef:
         """
         Deletes a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_endpoint)
@@ -500,14 +534,23 @@
         Returns the Identity and Access Management (Amazon Web Services IAM) policy for
         sharing the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_firewall_rule_group_policy)
         """
 
+    async def get_outpost_resolver(self, *, Id: str) -> GetOutpostResolverResponseTypeDef:
+        """
+        Gets information about a specified Resolver on the Outpost, such as its instance
+        count and type, name, and the current status of the Resolver.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_outpost_resolver)
+        """
+
     async def get_resolver_config(self, *, ResourceId: str) -> GetResolverConfigResponseTypeDef:
         """
         Retrieves the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_resolver_config)
@@ -680,14 +723,25 @@
         Retrieves the firewall rules that you have defined for the specified firewall
         rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_firewall_rules)
         """
 
+    async def list_outpost_resolvers(
+        self, *, OutpostArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListOutpostResolversResponseTypeDef:
+        """
+        Lists all the Resolvers on Outposts that were created using the current Amazon
+        Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_outpost_resolvers)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_outpost_resolvers)
+        """
+
     async def list_resolver_configs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListResolverConfigsResponseTypeDef:
         """
         Retrieves the Resolver configurations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_configs)
@@ -899,14 +953,30 @@
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule_group_association)
         """
 
+    async def update_outpost_resolver(
+        self,
+        *,
+        Id: str,
+        Name: str = ...,
+        InstanceCount: int = ...,
+        PreferredInstanceType: str = ...
+    ) -> UpdateOutpostResolverResponseTypeDef:
+        """
+        You can use `UpdateOutpostResolver` to update the instance count, type, or name
+        of a Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_outpost_resolver)
+        """
+
     async def update_resolver_config(
         self, *, ResourceId: str, AutodefinedReverseFlag: AutodefinedReverseFlagType
     ) -> UpdateResolverConfigResponseTypeDef:
         """
         Updates the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
@@ -1002,14 +1072,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_outpost_resolvers"]
+    ) -> ListOutpostResolversPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_resolver_configs"]
     ) -> ListResolverConfigsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
         """
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/client.pyi` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -55,33 +56,36 @@
     AssociateFirewallRuleGroupResponseTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     AssociateResolverQueryLogConfigResponseTypeDef,
     AssociateResolverRuleResponseTypeDef,
     CreateFirewallDomainListResponseTypeDef,
     CreateFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteFirewallDomainListResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
     DisassociateResolverQueryLogConfigResponseTypeDef,
     DisassociateResolverRuleResponseTypeDef,
     FilterTypeDef,
     GetFirewallConfigResponseTypeDef,
     GetFirewallDomainListResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
     GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     GetResolverEndpointResponseTypeDef,
     GetResolverQueryLogConfigAssociationResponseTypeDef,
     GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     GetResolverRuleAssociationResponseTypeDef,
@@ -92,14 +96,15 @@
     IpAddressUpdateTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -112,14 +117,15 @@
     TagTypeDef,
     TargetAddressTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     UpdateResolverEndpointResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -147,14 +153,15 @@
     InvalidRequestException: Type[BotocoreClientError]
     InvalidTagException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class Route53ResolverClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client)
@@ -266,24 +273,42 @@
         """
         Creates an empty DNS Firewall rule group for filtering DNS network traffic in a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_firewall_rule_group)
         """
+    async def create_outpost_resolver(
+        self,
+        *,
+        CreatorRequestId: str,
+        Name: str,
+        PreferredInstanceType: str,
+        OutpostArn: str,
+        InstanceCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateOutpostResolverResponseTypeDef:
+        """
+        Creates an Route 53 Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_outpost_resolver)
+        """
     async def create_resolver_endpoint(
         self,
         *,
         CreatorRequestId: str,
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ResolverEndpointType: ResolverEndpointTypeType = ...
+        ResolverEndpointType: ResolverEndpointTypeType = ...,
+        OutpostArn: str = ...,
+        PreferredInstanceType: str = ...
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#create_resolver_endpoint)
         """
@@ -344,14 +369,21 @@
     ) -> DeleteFirewallRuleGroupResponseTypeDef:
         """
         Deletes the specified firewall rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#delete_firewall_rule_group)
         """
+    async def delete_outpost_resolver(self, *, Id: str) -> DeleteOutpostResolverResponseTypeDef:
+        """
+        Deletes a Resolver on the Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#delete_outpost_resolver)
+        """
     async def delete_resolver_endpoint(
         self, *, ResolverEndpointId: str
     ) -> DeleteResolverEndpointResponseTypeDef:
         """
         Deletes a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_endpoint)
@@ -467,14 +499,22 @@
         """
         Returns the Identity and Access Management (Amazon Web Services IAM) policy for
         sharing the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_firewall_rule_group_policy)
         """
+    async def get_outpost_resolver(self, *, Id: str) -> GetOutpostResolverResponseTypeDef:
+        """
+        Gets information about a specified Resolver on the Outpost, such as its instance
+        count and type, name, and the current status of the Resolver.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_outpost_resolver)
+        """
     async def get_resolver_config(self, *, ResourceId: str) -> GetResolverConfigResponseTypeDef:
         """
         Retrieves the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_resolver_config)
@@ -631,14 +671,24 @@
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_firewall_rules)
         """
+    async def list_outpost_resolvers(
+        self, *, OutpostArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListOutpostResolversResponseTypeDef:
+        """
+        Lists all the Resolvers on Outposts that were created using the current Amazon
+        Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_outpost_resolvers)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#list_outpost_resolvers)
+        """
     async def list_resolver_configs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListResolverConfigsResponseTypeDef:
         """
         Retrieves the Resolver configurations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_configs)
@@ -832,14 +882,29 @@
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_firewall_rule_group_association)
         """
+    async def update_outpost_resolver(
+        self,
+        *,
+        Id: str,
+        Name: str = ...,
+        InstanceCount: int = ...,
+        PreferredInstanceType: str = ...
+    ) -> UpdateOutpostResolverResponseTypeDef:
+        """
+        You can use `UpdateOutpostResolver` to update the instance count, type, or name
+        of a Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#update_outpost_resolver)
+        """
     async def update_resolver_config(
         self, *, ResourceId: str, AutodefinedReverseFlag: AutodefinedReverseFlagType
     ) -> UpdateResolverConfigResponseTypeDef:
         """
         Updates the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
@@ -925,14 +990,22 @@
     ) -> ListFirewallRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_outpost_resolvers"]
+    ) -> ListOutpostResolversPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_resolver_configs"]
     ) -> ListResolverConfigsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/client/#get_paginator)
         """
     @overload
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/literals.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,24 +33,26 @@
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
     "ListFirewallDomainsPaginatorName",
     "ListFirewallRuleGroupAssociationsPaginatorName",
     "ListFirewallRuleGroupsPaginatorName",
     "ListFirewallRulesPaginatorName",
+    "ListOutpostResolversPaginatorName",
     "ListResolverConfigsPaginatorName",
     "ListResolverDnssecConfigsPaginatorName",
     "ListResolverEndpointIpAddressesPaginatorName",
     "ListResolverEndpointsPaginatorName",
     "ListResolverQueryLogConfigAssociationsPaginatorName",
     "ListResolverQueryLogConfigsPaginatorName",
     "ListResolverRuleAssociationsPaginatorName",
     "ListResolverRulesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MutationProtectionStatusType",
+    "OutpostResolverStatusType",
     "ResolverAutodefinedReverseStatusType",
     "ResolverDNSSECValidationStatusType",
     "ResolverEndpointDirectionType",
     "ResolverEndpointStatusType",
     "ResolverEndpointTypeType",
     "ResolverQueryLogConfigAssociationErrorType",
     "ResolverQueryLogConfigAssociationStatusType",
@@ -88,34 +90,45 @@
     "DELETE_FAILED_FAS_EXPIRED",
     "DELETING",
     "DETACHING",
     "FAILED_CREATION",
     "FAILED_RESOURCE_GONE",
     "REMAP_ATTACHING",
     "REMAP_DETACHING",
+    "UPDATE_FAILED",
     "UPDATING",
 ]
 ListFirewallConfigsPaginatorName = Literal["list_firewall_configs"]
 ListFirewallDomainListsPaginatorName = Literal["list_firewall_domain_lists"]
 ListFirewallDomainsPaginatorName = Literal["list_firewall_domains"]
 ListFirewallRuleGroupAssociationsPaginatorName = Literal["list_firewall_rule_group_associations"]
 ListFirewallRuleGroupsPaginatorName = Literal["list_firewall_rule_groups"]
 ListFirewallRulesPaginatorName = Literal["list_firewall_rules"]
+ListOutpostResolversPaginatorName = Literal["list_outpost_resolvers"]
 ListResolverConfigsPaginatorName = Literal["list_resolver_configs"]
 ListResolverDnssecConfigsPaginatorName = Literal["list_resolver_dnssec_configs"]
 ListResolverEndpointIpAddressesPaginatorName = Literal["list_resolver_endpoint_ip_addresses"]
 ListResolverEndpointsPaginatorName = Literal["list_resolver_endpoints"]
 ListResolverQueryLogConfigAssociationsPaginatorName = Literal[
     "list_resolver_query_log_config_associations"
 ]
 ListResolverQueryLogConfigsPaginatorName = Literal["list_resolver_query_log_configs"]
 ListResolverRuleAssociationsPaginatorName = Literal["list_resolver_rule_associations"]
 ListResolverRulesPaginatorName = Literal["list_resolver_rules"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MutationProtectionStatusType = Literal["DISABLED", "ENABLED"]
+OutpostResolverStatusType = Literal[
+    "ACTION_NEEDED",
+    "CREATING",
+    "DELETING",
+    "FAILED_CREATION",
+    "FAILED_DELETION",
+    "OPERATIONAL",
+    "UPDATING",
+]
 ResolverAutodefinedReverseStatusType = Literal[
     "DISABLED",
     "DISABLING",
     "ENABLED",
     "ENABLING",
     "UPDATING_TO_USE_LOCAL_RESOURCE_SETTING",
     "USE_LOCAL_RESOURCE_SETTING",
@@ -160,14 +173,15 @@
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
@@ -263,14 +277,15 @@
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
@@ -349,26 +364,28 @@
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
@@ -515,14 +532,15 @@
 PaginatorName = Literal[
     "list_firewall_configs",
     "list_firewall_domain_lists",
     "list_firewall_domains",
     "list_firewall_rule_group_associations",
     "list_firewall_rule_groups",
     "list_firewall_rules",
+    "list_outpost_resolvers",
     "list_resolver_configs",
     "list_resolver_dnssec_configs",
     "list_resolver_endpoint_ip_addresses",
     "list_resolver_endpoints",
     "list_resolver_query_log_config_associations",
     "list_resolver_query_log_configs",
     "list_resolver_rule_associations",
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/literals.pyi` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,24 +32,26 @@
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
     "ListFirewallDomainsPaginatorName",
     "ListFirewallRuleGroupAssociationsPaginatorName",
     "ListFirewallRuleGroupsPaginatorName",
     "ListFirewallRulesPaginatorName",
+    "ListOutpostResolversPaginatorName",
     "ListResolverConfigsPaginatorName",
     "ListResolverDnssecConfigsPaginatorName",
     "ListResolverEndpointIpAddressesPaginatorName",
     "ListResolverEndpointsPaginatorName",
     "ListResolverQueryLogConfigAssociationsPaginatorName",
     "ListResolverQueryLogConfigsPaginatorName",
     "ListResolverRuleAssociationsPaginatorName",
     "ListResolverRulesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MutationProtectionStatusType",
+    "OutpostResolverStatusType",
     "ResolverAutodefinedReverseStatusType",
     "ResolverDNSSECValidationStatusType",
     "ResolverEndpointDirectionType",
     "ResolverEndpointStatusType",
     "ResolverEndpointTypeType",
     "ResolverQueryLogConfigAssociationErrorType",
     "ResolverQueryLogConfigAssociationStatusType",
@@ -86,34 +88,45 @@
     "DELETE_FAILED_FAS_EXPIRED",
     "DELETING",
     "DETACHING",
     "FAILED_CREATION",
     "FAILED_RESOURCE_GONE",
     "REMAP_ATTACHING",
     "REMAP_DETACHING",
+    "UPDATE_FAILED",
     "UPDATING",
 ]
 ListFirewallConfigsPaginatorName = Literal["list_firewall_configs"]
 ListFirewallDomainListsPaginatorName = Literal["list_firewall_domain_lists"]
 ListFirewallDomainsPaginatorName = Literal["list_firewall_domains"]
 ListFirewallRuleGroupAssociationsPaginatorName = Literal["list_firewall_rule_group_associations"]
 ListFirewallRuleGroupsPaginatorName = Literal["list_firewall_rule_groups"]
 ListFirewallRulesPaginatorName = Literal["list_firewall_rules"]
+ListOutpostResolversPaginatorName = Literal["list_outpost_resolvers"]
 ListResolverConfigsPaginatorName = Literal["list_resolver_configs"]
 ListResolverDnssecConfigsPaginatorName = Literal["list_resolver_dnssec_configs"]
 ListResolverEndpointIpAddressesPaginatorName = Literal["list_resolver_endpoint_ip_addresses"]
 ListResolverEndpointsPaginatorName = Literal["list_resolver_endpoints"]
 ListResolverQueryLogConfigAssociationsPaginatorName = Literal[
     "list_resolver_query_log_config_associations"
 ]
 ListResolverQueryLogConfigsPaginatorName = Literal["list_resolver_query_log_configs"]
 ListResolverRuleAssociationsPaginatorName = Literal["list_resolver_rule_associations"]
 ListResolverRulesPaginatorName = Literal["list_resolver_rules"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MutationProtectionStatusType = Literal["DISABLED", "ENABLED"]
+OutpostResolverStatusType = Literal[
+    "ACTION_NEEDED",
+    "CREATING",
+    "DELETING",
+    "FAILED_CREATION",
+    "FAILED_DELETION",
+    "OPERATIONAL",
+    "UPDATING",
+]
 ResolverAutodefinedReverseStatusType = Literal[
     "DISABLED",
     "DISABLING",
     "ENABLED",
     "ENABLING",
     "UPDATING_TO_USE_LOCAL_RESOURCE_SETTING",
     "USE_LOCAL_RESOURCE_SETTING",
@@ -158,14 +171,15 @@
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
@@ -261,14 +275,15 @@
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
@@ -347,26 +362,28 @@
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
@@ -513,14 +530,15 @@
 PaginatorName = Literal[
     "list_firewall_configs",
     "list_firewall_domain_lists",
     "list_firewall_domains",
     "list_firewall_rule_group_associations",
     "list_firewall_rule_groups",
     "list_firewall_rules",
+    "list_outpost_resolvers",
     "list_resolver_configs",
     "list_resolver_dnssec_configs",
     "list_resolver_endpoint_ip_addresses",
     "list_resolver_endpoints",
     "list_resolver_query_log_config_associations",
     "list_resolver_query_log_configs",
     "list_resolver_rule_associations",
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/paginator.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from types_aiobotocore_route53resolver.paginator import (
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -33,14 +34,15 @@
 
         list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
         list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
         list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
         list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
         list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
         list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+        list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
         list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
         list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
         list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
         list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
         list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
         list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
         list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -58,14 +60,15 @@
     FilterTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -77,14 +80,15 @@
 __all__ = (
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
@@ -200,14 +204,29 @@
     ) -> AsyncIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 
+class ListOutpostResolversPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listoutpostresolverspaginator)
+    """
+
+    def paginate(
+        self, *, OutpostArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListOutpostResolversResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listoutpostresolverspaginator)
+        """
+
+
 class ListResolverConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/paginator.pyi` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from types_aiobotocore_route53resolver.paginator import (
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -33,14 +34,15 @@
 
         list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
         list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
         list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
         list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
         list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
         list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+        list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
         list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
         list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
         list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
         list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
         list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
         list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
         list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -58,14 +60,15 @@
     FilterTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -77,14 +80,15 @@
 __all__ = (
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
@@ -191,14 +195,28 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
+class ListOutpostResolversPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listoutpostresolverspaginator)
+    """
+
+    def paginate(
+        self, *, OutpostArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListOutpostResolversResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listoutpostresolverspaginator)
+        """
+
 class ListResolverConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/type_defs.py` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FirewallDomainListStatusType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -61,20 +62,22 @@
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
     "FirewallRuleGroupTypeDef",
     "CreateFirewallRuleRequestRequestTypeDef",
     "FirewallRuleTypeDef",
+    "OutpostResolverTypeDef",
     "IpAddressRequestTypeDef",
     "ResolverQueryLogConfigTypeDef",
     "TargetAddressTypeDef",
     "DeleteFirewallDomainListRequestRequestTypeDef",
     "DeleteFirewallRuleGroupRequestRequestTypeDef",
     "DeleteFirewallRuleRequestRequestTypeDef",
+    "DeleteOutpostResolverRequestRequestTypeDef",
     "DeleteResolverEndpointRequestRequestTypeDef",
     "DeleteResolverQueryLogConfigRequestRequestTypeDef",
     "DeleteResolverRuleRequestRequestTypeDef",
     "DisassociateFirewallRuleGroupRequestRequestTypeDef",
     "DisassociateResolverQueryLogConfigRequestRequestTypeDef",
     "DisassociateResolverRuleRequestRequestTypeDef",
     "FilterTypeDef",
@@ -82,14 +85,15 @@
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
+    "GetOutpostResolverRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
@@ -102,31 +106,34 @@
     "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
+    "ListOutpostResolversRequestRequestTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
+    "UpdateOutpostResolverRequestRequestTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
+    "CreateOutpostResolverRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetResolverQueryLogConfigPolicyResponseTypeDef",
@@ -163,14 +170,19 @@
     "CreateFirewallRuleGroupResponseTypeDef",
     "DeleteFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupResponseTypeDef",
     "CreateFirewallRuleResponseTypeDef",
     "DeleteFirewallRuleResponseTypeDef",
     "ListFirewallRulesResponseTypeDef",
     "UpdateFirewallRuleResponseTypeDef",
+    "CreateOutpostResolverResponseTypeDef",
+    "DeleteOutpostResolverResponseTypeDef",
+    "GetOutpostResolverResponseTypeDef",
+    "ListOutpostResolversResponseTypeDef",
+    "UpdateOutpostResolverResponseTypeDef",
     "CreateResolverEndpointRequestRequestTypeDef",
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
@@ -195,14 +207,15 @@
     "ListResolverEndpointIpAddressesResponseTypeDef",
     "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
     "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
     "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
@@ -279,14 +292,16 @@
         "IpAddressCount": int,
         "HostVPCId": str,
         "Status": ResolverEndpointStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
@@ -425,14 +440,32 @@
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
+OutpostResolverTypeDef = TypedDict(
+    "OutpostResolverTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": str,
+        "ModificationTime": str,
+        "CreatorRequestId": str,
+        "Id": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+        "Name": str,
+        "Status": OutpostResolverStatusType,
+        "StatusMessage": str,
+        "OutpostArn": str,
+    },
+    total=False,
+)
+
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
 )
 _OptionalIpAddressRequestTypeDef = TypedDict(
@@ -494,14 +527,21 @@
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
 
+DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
+    "DeleteOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 DeleteResolverEndpointRequestRequestTypeDef = TypedDict(
     "DeleteResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 
@@ -618,14 +658,21 @@
 GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 
+GetOutpostResolverRequestRequestTypeDef = TypedDict(
+    "GetOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 GetResolverConfigRequestRequestTypeDef = TypedDict(
     "GetResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -824,14 +871,24 @@
 
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
 
+ListOutpostResolversRequestRequestTypeDef = TypedDict(
+    "ListOutpostResolversRequestRequestTypeDef",
+    {
+        "OutpostArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -989,14 +1046,38 @@
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
 
+_RequiredUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+    },
+    total=False,
+)
+
+
+class UpdateOutpostResolverRequestRequestTypeDef(
+    _RequiredUpdateOutpostResolverRequestRequestTypeDef,
+    _OptionalUpdateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateResolverConfigRequestRequestTypeDef = TypedDict(
     "UpdateResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
         "AutodefinedReverseFlag": AutodefinedReverseFlagType,
     },
 )
@@ -1078,14 +1159,40 @@
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Name": str,
+        "PreferredInstanceType": str,
+        "OutpostArn": str,
+    },
+)
+_OptionalCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "InstanceCount": int,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateOutpostResolverRequestRequestTypeDef(
+    _RequiredCreateOutpostResolverRequestRequestTypeDef,
+    _OptionalCreateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1463,14 +1570,55 @@
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateOutpostResolverResponseTypeDef = TypedDict(
+    "CreateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOutpostResolverResponseTypeDef = TypedDict(
+    "DeleteOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOutpostResolverResponseTypeDef = TypedDict(
+    "GetOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutpostResolversResponseTypeDef = TypedDict(
+    "ListOutpostResolversResponseTypeDef",
+    {
+        "OutpostResolvers": List[OutpostResolverTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOutpostResolverResponseTypeDef = TypedDict(
+    "UpdateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "SecurityGroupIds": Sequence[str],
         "Direction": ResolverEndpointDirectionType,
         "IpAddresses": Sequence[IpAddressRequestTypeDef],
@@ -1478,14 +1626,16 @@
 )
 _OptionalCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResolverEndpointRequestRequestTypeDef",
     {
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
@@ -1834,14 +1984,23 @@
 class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
     _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
 ):
     pass
 
 
+ListOutpostResolversRequestListOutpostResolversPaginateTypeDef = TypedDict(
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    {
+        "OutpostArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
     "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver/type_defs.pyi` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FirewallDomainListStatusType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -60,20 +61,22 @@
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
     "FirewallRuleGroupTypeDef",
     "CreateFirewallRuleRequestRequestTypeDef",
     "FirewallRuleTypeDef",
+    "OutpostResolverTypeDef",
     "IpAddressRequestTypeDef",
     "ResolverQueryLogConfigTypeDef",
     "TargetAddressTypeDef",
     "DeleteFirewallDomainListRequestRequestTypeDef",
     "DeleteFirewallRuleGroupRequestRequestTypeDef",
     "DeleteFirewallRuleRequestRequestTypeDef",
+    "DeleteOutpostResolverRequestRequestTypeDef",
     "DeleteResolverEndpointRequestRequestTypeDef",
     "DeleteResolverQueryLogConfigRequestRequestTypeDef",
     "DeleteResolverRuleRequestRequestTypeDef",
     "DisassociateFirewallRuleGroupRequestRequestTypeDef",
     "DisassociateResolverQueryLogConfigRequestRequestTypeDef",
     "DisassociateResolverRuleRequestRequestTypeDef",
     "FilterTypeDef",
@@ -81,14 +84,15 @@
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
+    "GetOutpostResolverRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
@@ -101,31 +105,34 @@
     "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
+    "ListOutpostResolversRequestRequestTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
+    "UpdateOutpostResolverRequestRequestTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
+    "CreateOutpostResolverRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetResolverQueryLogConfigPolicyResponseTypeDef",
@@ -162,14 +169,19 @@
     "CreateFirewallRuleGroupResponseTypeDef",
     "DeleteFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupResponseTypeDef",
     "CreateFirewallRuleResponseTypeDef",
     "DeleteFirewallRuleResponseTypeDef",
     "ListFirewallRulesResponseTypeDef",
     "UpdateFirewallRuleResponseTypeDef",
+    "CreateOutpostResolverResponseTypeDef",
+    "DeleteOutpostResolverResponseTypeDef",
+    "GetOutpostResolverResponseTypeDef",
+    "ListOutpostResolversResponseTypeDef",
+    "UpdateOutpostResolverResponseTypeDef",
     "CreateResolverEndpointRequestRequestTypeDef",
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
@@ -194,14 +206,15 @@
     "ListResolverEndpointIpAddressesResponseTypeDef",
     "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
     "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
     "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
@@ -278,14 +291,16 @@
         "IpAddressCount": int,
         "HostVPCId": str,
         "Status": ResolverEndpointStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
@@ -420,14 +435,32 @@
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
+OutpostResolverTypeDef = TypedDict(
+    "OutpostResolverTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": str,
+        "ModificationTime": str,
+        "CreatorRequestId": str,
+        "Id": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+        "Name": str,
+        "Status": OutpostResolverStatusType,
+        "StatusMessage": str,
+        "OutpostArn": str,
+    },
+    total=False,
+)
+
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
 )
 _OptionalIpAddressRequestTypeDef = TypedDict(
@@ -487,14 +520,21 @@
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
 
+DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
+    "DeleteOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 DeleteResolverEndpointRequestRequestTypeDef = TypedDict(
     "DeleteResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 
@@ -611,14 +651,21 @@
 GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 
+GetOutpostResolverRequestRequestTypeDef = TypedDict(
+    "GetOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 GetResolverConfigRequestRequestTypeDef = TypedDict(
     "GetResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -813,14 +860,24 @@
 )
 
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
+ListOutpostResolversRequestRequestTypeDef = TypedDict(
+    "ListOutpostResolversRequestRequestTypeDef",
+    {
+        "OutpostArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -970,14 +1027,36 @@
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
 
+_RequiredUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+    },
+    total=False,
+)
+
+class UpdateOutpostResolverRequestRequestTypeDef(
+    _RequiredUpdateOutpostResolverRequestRequestTypeDef,
+    _OptionalUpdateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
 UpdateResolverConfigRequestRequestTypeDef = TypedDict(
     "UpdateResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
         "AutodefinedReverseFlag": AutodefinedReverseFlagType,
     },
 )
@@ -1053,14 +1132,38 @@
 
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Name": str,
+        "PreferredInstanceType": str,
+        "OutpostArn": str,
+    },
+)
+_OptionalCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "InstanceCount": int,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateOutpostResolverRequestRequestTypeDef(
+    _RequiredCreateOutpostResolverRequestRequestTypeDef,
+    _OptionalCreateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1436,14 +1539,55 @@
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateOutpostResolverResponseTypeDef = TypedDict(
+    "CreateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOutpostResolverResponseTypeDef = TypedDict(
+    "DeleteOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOutpostResolverResponseTypeDef = TypedDict(
+    "GetOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutpostResolversResponseTypeDef = TypedDict(
+    "ListOutpostResolversResponseTypeDef",
+    {
+        "OutpostResolvers": List[OutpostResolverTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOutpostResolverResponseTypeDef = TypedDict(
+    "UpdateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "SecurityGroupIds": Sequence[str],
         "Direction": ResolverEndpointDirectionType,
         "IpAddresses": Sequence[IpAddressRequestTypeDef],
@@ -1451,14 +1595,16 @@
 )
 _OptionalCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResolverEndpointRequestRequestTypeDef",
     {
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
     _OptionalCreateResolverEndpointRequestRequestTypeDef,
@@ -1799,14 +1945,23 @@
 
 class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
     _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
 ):
     pass
 
+ListOutpostResolversRequestListOutpostResolversPaginateTypeDef = TypedDict(
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    {
+        "OutpostArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
     "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post1/types_aiobotocore_route53resolver.egg-info/SOURCES.txt` & `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

