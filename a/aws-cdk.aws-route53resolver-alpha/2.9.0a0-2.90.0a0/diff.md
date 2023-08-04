# Comparing `tmp/aws-cdk.aws-route53resolver-alpha-2.9.0a0.tar.gz` & `tmp/aws-cdk.aws-route53resolver-alpha-2.90.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-route53resolver/dist/python/aws-cdk.aws-route53resolver-alp", last modified: Wed Jan 26 11:22:07 2022, max compression
+gzip compressed data, was "aws-cdk.aws-route53resolver-alpha-2.90.0a0.tar", last modified: Fri Aug  4 19:20:37 2023, max compression
```

## Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0.tar` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5009 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4025 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1851 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/
--rw-r--r--   0 root         (0) root         (0)    62023 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      421 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39104 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/aws-route53resolver-alpha@2.9.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:07.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5009 2022-01-26 11:22:06.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      610 2022-01-26 11:22:06.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/
+-rw-r--r--   0 root         (0) root         (0)    73544 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43073 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/_jsii/aws-route53resolver-alpha@2.90.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:25.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:37.567486 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-08-04 19:20:37.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2023-08-04 19:20:37.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:37.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-04 19:20:37.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 19:20:37.000000 aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/LICENSE` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/PKG-INFO` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-route53resolver-alpha
-Version: 2.9.0a0
+Version: 2.90.0a0
 Summary: The CDK Construct Library for AWS::Route53Resolver
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 1
-Requires-Python: >=3.6
+Classifier: Framework :: AWS CDK :: 2
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Amazon Route53 Resolver Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -134,9 +134,7 @@
 
 
 rule_group.associate("Association",
     priority=101,
     vpc=my_vpc
 )
 ```
-
-
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/README.md` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/setup.py` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-route53resolver-alpha",
-    "version": "2.9.0.a0",
+    "version": "2.90.0.a0",
     "description": "The CDK Construct Library for AWS::Route53Resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,41 +22,43 @@
     },
     "packages": [
         "aws_cdk.aws_route53resolver_alpha",
         "aws_cdk.aws_route53resolver_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_route53resolver_alpha._jsii": [
-            "aws-route53resolver-alpha@2.9.0-alpha.0.jsii.tgz"
+            "aws-route53resolver-alpha@2.90.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_route53resolver_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": ">=3.6",
+    "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.9.0, <3.0.0",
+        "aws-cdk-lib==2.90.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.52.1, <2.0.0",
-        "publication>=0.0.3"
+        "jsii>=1.86.0, <2.0.0",
+        "publication>=0.0.3",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 1"
+        "Framework :: AWS CDK :: 2"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk/aws_route53resolver_alpha/__init__.py` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk/aws_route53resolver_alpha/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -119,20 +119,22 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
+from typeguard import check_type
+
 from ._jsii import *
 
-import aws_cdk
-import aws_cdk.aws_ec2
-import aws_cdk.aws_s3
-import constructs
+import aws_cdk as _aws_cdk_ceddda9d
+import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
+import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class DnsBlockResponse(
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="@aws-cdk/aws-route53resolver-alpha.DnsBlockResponse",
 ):
     '''(experimental) The way that you want DNS Firewall to block the request.
@@ -163,118 +165,122 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="noData") # type: ignore[misc]
+    @jsii.member(jsii_name="noData")
     @builtins.classmethod
     def no_data(cls) -> "DnsBlockResponse":
         '''(experimental) Respond indicating that the query was successful, but no response is available for it.
 
         :stability: experimental
         '''
         return typing.cast("DnsBlockResponse", jsii.sinvoke(cls, "noData", []))
 
-    @jsii.member(jsii_name="nxDomain") # type: ignore[misc]
+    @jsii.member(jsii_name="nxDomain")
     @builtins.classmethod
     def nx_domain(cls) -> "DnsBlockResponse":
         '''(experimental) Respond indicating that the domain name that's in the query doesn't exist.
 
         :stability: experimental
         '''
         return typing.cast("DnsBlockResponse", jsii.sinvoke(cls, "nxDomain", []))
 
-    @jsii.member(jsii_name="override") # type: ignore[misc]
+    @jsii.member(jsii_name="override")
     @builtins.classmethod
     def override(
         cls,
         domain: builtins.str,
-        ttl: typing.Optional[aws_cdk.Duration] = None,
+        ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     ) -> "DnsBlockResponse":
         '''(experimental) Provides a custom override response to the query.
 
         :param domain: The custom DNS record to send back in response to the query.
         :param ttl: The recommended amount of time for the DNS resolver or web browser to cache the provided override record.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__bcc6e5cbcbf161b026004146d290f4c2c5203dd60e43bb296ae451b7ea8afb50)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         return typing.cast("DnsBlockResponse", jsii.sinvoke(cls, "override", [domain, ttl]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideDnsType")
     @abc.abstractmethod
     def block_override_dns_type(self) -> typing.Optional[builtins.str]:
         '''(experimental) The DNS record's type.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideDomain")
     @abc.abstractmethod
     def block_override_domain(self) -> typing.Optional[builtins.str]:
         '''(experimental) The custom DNS record to send back in response to the query.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideTtl")
     @abc.abstractmethod
-    def block_override_ttl(self) -> typing.Optional[aws_cdk.Duration]:
+    def block_override_ttl(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) The recommended amount of time for the DNS resolver or web browser to cache the provided override record.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockResponse")
     @abc.abstractmethod
     def block_response(self) -> typing.Optional[builtins.str]:
         '''(experimental) The way that you want DNS Firewall to block the request.
 
         :stability: experimental
         '''
         ...
 
 
 class _DnsBlockResponseProxy(DnsBlockResponse):
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideDnsType")
     def block_override_dns_type(self) -> typing.Optional[builtins.str]:
         '''(experimental) The DNS record's type.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "blockOverrideDnsType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideDomain")
     def block_override_domain(self) -> typing.Optional[builtins.str]:
         '''(experimental) The custom DNS record to send back in response to the query.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "blockOverrideDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockOverrideTtl")
-    def block_override_ttl(self) -> typing.Optional[aws_cdk.Duration]:
+    def block_override_ttl(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
         '''(experimental) The recommended amount of time for the DNS resolver or web browser to cache the provided override record.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[aws_cdk.Duration], jsii.get(self, "blockOverrideTtl"))
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], jsii.get(self, "blockOverrideTtl"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockResponse")
     def block_response(self) -> typing.Optional[builtins.str]:
         '''(experimental) The way that you want DNS Firewall to block the request.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "blockResponse"))
@@ -310,15 +316,19 @@
             import aws_cdk.aws_route53resolver_alpha as route53resolver_alpha
             
             domains_config = route53resolver_alpha.DomainsConfig(
                 domain_file_url="domainFileUrl",
                 domains=["domains"]
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {}
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__efcc739bead6cd1e2f6028bbf509537b88cdaab217e4ad29abcb83010af732aa)
+            check_type(argname="argument domain_file_url", value=domain_file_url, expected_type=type_hints["domain_file_url"])
+            check_type(argname="argument domains", value=domains, expected_type=type_hints["domains"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if domain_file_url is not None:
             self._values["domain_file_url"] = domain_file_url
         if domains is not None:
             self._values["domains"] = domains
 
     @builtins.property
     def domain_file_url(self) -> typing.Optional[builtins.str]:
@@ -387,15 +397,19 @@
                 domains=route53resolver.FirewallDomains.from_s3_url("s3://bucket/prefix/object")
             )
             
             asset_list = route53resolver.FirewallDomainList(self, "AssetList",
                 domains=route53resolver.FirewallDomains.from_asset("/path/to/domains.txt")
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e2694ecc77bbdf59285a53d044c17b801083d48fd6d9cf26c5798be8ef83cfd4)
+            check_type(argname="argument domains", value=domains, expected_type=type_hints["domains"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "domains": domains,
         }
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def domains(self) -> "FirewallDomains":
@@ -456,93 +470,109 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="fromAsset") # type: ignore[misc]
+    @jsii.member(jsii_name="fromAsset")
     @builtins.classmethod
     def from_asset(cls, asset_path: builtins.str) -> "FirewallDomains":
         '''(experimental) Firewall domains created from a local disk path to a text file.
 
         The file must be a text file (``.txt`` extension) and must contain a single
         domain per line. It will be uploaded to S3.
 
         :param asset_path: path to the text file.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a7b0d1079af5d8eb8466e6719de93c31cc9a02bfc3b4b058593e609db394d240)
+            check_type(argname="argument asset_path", value=asset_path, expected_type=type_hints["asset_path"])
         return typing.cast("FirewallDomains", jsii.sinvoke(cls, "fromAsset", [asset_path]))
 
-    @jsii.member(jsii_name="fromList") # type: ignore[misc]
+    @jsii.member(jsii_name="fromList")
     @builtins.classmethod
     def from_list(cls, list: typing.Sequence[builtins.str]) -> "FirewallDomains":
         '''(experimental) Firewall domains created from a list of domains.
 
         :param list: the list of domains.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4db439b64de98348184f5457d37416fdf39df7bfa653f43e5546f736c932c7ba)
+            check_type(argname="argument list", value=list, expected_type=type_hints["list"])
         return typing.cast("FirewallDomains", jsii.sinvoke(cls, "fromList", [list]))
 
-    @jsii.member(jsii_name="fromS3") # type: ignore[misc]
+    @jsii.member(jsii_name="fromS3")
     @builtins.classmethod
     def from_s3(
         cls,
-        bucket: aws_cdk.aws_s3.IBucket,
+        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
         key: builtins.str,
     ) -> "FirewallDomains":
         '''(experimental) Firewall domains created from a file stored in Amazon S3.
 
         The file must be a text file and must contain a single domain per line.
         The content type of the S3 object must be ``plain/text``.
 
         :param bucket: S3 bucket.
         :param key: S3 key.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9123f4606e1c6eda8fc3b706939d87b0209c2bea457af92c0af2a946a6684d64)
+            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
+            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast("FirewallDomains", jsii.sinvoke(cls, "fromS3", [bucket, key]))
 
-    @jsii.member(jsii_name="fromS3Url") # type: ignore[misc]
+    @jsii.member(jsii_name="fromS3Url")
     @builtins.classmethod
     def from_s3_url(cls, url: builtins.str) -> "FirewallDomains":
         '''(experimental) Firewall domains created from the URL of a file stored in Amazon S3.
 
         The file must be a text file and must contain a single domain per line.
         The content type of the S3 object must be ``plain/text``.
 
         :param url: S3 bucket url (s3://bucket/prefix/objet).
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9f74514d1763b172a7f7f23feabbb8360b780c1b88c0e33c8dd934f2542a42db)
+            check_type(argname="argument url", value=url, expected_type=type_hints["url"])
         return typing.cast("FirewallDomains", jsii.sinvoke(cls, "fromS3Url", [url]))
 
-    @jsii.member(jsii_name="bind") # type: ignore[misc]
+    @jsii.member(jsii_name="bind")
     @abc.abstractmethod
-    def bind(self, scope: constructs.Construct) -> DomainsConfig:
+    def bind(self, scope: _constructs_77d1e7e8.Construct) -> DomainsConfig:
         '''(experimental) Binds the domains to a domain list.
 
         :param scope: -
 
         :stability: experimental
         '''
         ...
 
 
 class _FirewallDomainsProxy(FirewallDomains):
     @jsii.member(jsii_name="bind")
-    def bind(self, scope: constructs.Construct) -> DomainsConfig:
+    def bind(self, scope: _constructs_77d1e7e8.Construct) -> DomainsConfig:
         '''(experimental) Binds the domains to a domain list.
 
         :param scope: -
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__beee843294402bd0b4634b78a18a987c0d888a0afb182d42637c4bf1d18c0908)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
         return typing.cast(DomainsConfig, jsii.invoke(self, "bind", [scope]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, FirewallDomains).__jsii_proxy_class__ = lambda : _FirewallDomainsProxy
 
 
 @jsii.data_type(
@@ -587,15 +617,20 @@
             rule_group.add_rule(
                 priority=20,
                 firewall_domain_list=my_block_list,
                 # block and override DNS response with a custom domain
                 action=route53resolver.FirewallRuleAction.block(route53resolver.DnsBlockResponse.override("amazon.com"))
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c842a13b2d3ff276f74958de9ce814eafca72f45f15296caa8cf78d6ad8c39a5)
+            check_type(argname="argument action", value=action, expected_type=type_hints["action"])
+            check_type(argname="argument firewall_domain_list", value=firewall_domain_list, expected_type=type_hints["firewall_domain_list"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "action": action,
             "firewall_domain_list": firewall_domain_list,
             "priority": priority,
         }
 
     @builtins.property
     def action(self) -> "FirewallRuleAction":
@@ -668,92 +703,95 @@
 
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
-    @jsii.member(jsii_name="alert") # type: ignore[misc]
+    @jsii.member(jsii_name="alert")
     @builtins.classmethod
     def alert(cls) -> "FirewallRuleAction":
         '''(experimental) Permit the request to go through but send an alert to the logs.
 
         :stability: experimental
         '''
         return typing.cast("FirewallRuleAction", jsii.sinvoke(cls, "alert", []))
 
-    @jsii.member(jsii_name="allow") # type: ignore[misc]
+    @jsii.member(jsii_name="allow")
     @builtins.classmethod
     def allow(cls) -> "FirewallRuleAction":
         '''(experimental) Permit the request to go through.
 
         :stability: experimental
         '''
         return typing.cast("FirewallRuleAction", jsii.sinvoke(cls, "allow", []))
 
-    @jsii.member(jsii_name="block") # type: ignore[misc]
+    @jsii.member(jsii_name="block")
     @builtins.classmethod
     def block(
         cls,
         response: typing.Optional[DnsBlockResponse] = None,
     ) -> "FirewallRuleAction":
         '''(experimental) Disallow the request.
 
         :param response: The way that you want DNS Firewall to block the request.
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__908212340f1ac128d44306136d4c2b8737eeff37eab2b68c781cfb8d7345f036)
+            check_type(argname="argument response", value=response, expected_type=type_hints["response"])
         return typing.cast("FirewallRuleAction", jsii.sinvoke(cls, "block", [response]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="action")
     @abc.abstractmethod
     def action(self) -> builtins.str:
         '''(experimental) The action that DNS Firewall should take on a DNS query when it matches one of the domains in the rule's domain list.
 
         :stability: experimental
         '''
         ...
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockResponse")
     @abc.abstractmethod
     def block_response(self) -> typing.Optional[DnsBlockResponse]:
         '''(experimental) The way that you want DNS Firewall to block the request.
 
         :stability: experimental
         '''
         ...
 
 
 class _FirewallRuleActionProxy(FirewallRuleAction):
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="action")
     def action(self) -> builtins.str:
         '''(experimental) The action that DNS Firewall should take on a DNS query when it matches one of the domains in the rule's domain list.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "action"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="blockResponse")
     def block_response(self) -> typing.Optional[DnsBlockResponse]:
         '''(experimental) The way that you want DNS Firewall to block the request.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[DnsBlockResponse], jsii.get(self, "blockResponse"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, FirewallRuleAction).__jsii_proxy_class__ = lambda : _FirewallRuleActionProxy
 
 
 class FirewallRuleGroupAssociation(
-    aws_cdk.Resource,
+    _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-route53resolver-alpha.FirewallRuleGroupAssociation",
 ):
     '''(experimental) A Firewall Rule Group Association.
 
     :stability: experimental
     :exampleMetadata: fixture=_generated
@@ -777,118 +815,122 @@
             mutation_protection=False,
             name="name"
         )
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         firewall_rule_group: "IFirewallRuleGroup",
         priority: jsii.Number,
-        vpc: aws_cdk.aws_ec2.IVpc,
+        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         mutation_protection: typing.Optional[builtins.bool] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param firewall_rule_group: (experimental) The firewall rule group which must be associated.
         :param priority: (experimental) The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters VPC traffic starting from rule group with the lowest numeric priority setting. This value must be greater than 100 and less than 9,000
         :param vpc: (experimental) The VPC that to associate with the rule group.
         :param mutation_protection: (experimental) If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections. Default: true
         :param name: (experimental) The name of the association. Default: - a CloudFormation generated name
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__66db44623853cec6127559e80b1ff37cd188ae6bb06e46d5500ca10c786695ec)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirewallRuleGroupAssociationProps(
             firewall_rule_group=firewall_rule_group,
             priority=priority,
             vpc=vpc,
             mutation_protection=mutation_protection,
             name=name,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationArn")
     def firewall_rule_group_association_arn(self) -> builtins.str:
         '''(experimental) The ARN (Amazon Resource Name) of the association.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationCreationTime")
     def firewall_rule_group_association_creation_time(self) -> builtins.str:
         '''(experimental) The date and time that the association was created.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationCreationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationCreatorRequestId")
     def firewall_rule_group_association_creator_request_id(self) -> builtins.str:
         '''(experimental) The creator request ID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationCreatorRequestId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationId")
     def firewall_rule_group_association_id(self) -> builtins.str:
         '''(experimental) The ID of the association.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationManagedOwnerName")
     def firewall_rule_group_association_managed_owner_name(self) -> builtins.str:
         '''(experimental) The owner of the association, used only for lists that are not managed by you.
 
         If you use AWS Firewall Manager to manage your firewallls from DNS Firewall,
         then this reports Firewall Manager as the managed owner.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationManagedOwnerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationModificationTime")
     def firewall_rule_group_association_modification_time(self) -> builtins.str:
         '''(experimental) The date and time that the association was last modified.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationModificationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationStatus")
     def firewall_rule_group_association_status(self) -> builtins.str:
         '''(experimental) The status of the association.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupAssociationStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupAssociationStatusMessage")
     def firewall_rule_group_association_status_message(self) -> builtins.str:
         '''(experimental) Additional information about the status of the association.
 
         :stability: experimental
         :attribute: true
         '''
@@ -906,15 +948,15 @@
     },
 )
 class FirewallRuleGroupAssociationOptions:
     def __init__(
         self,
         *,
         priority: jsii.Number,
-        vpc: aws_cdk.aws_ec2.IVpc,
+        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         mutation_protection: typing.Optional[builtins.bool] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Options for a Firewall Rule Group Association.
 
         :param priority: (experimental) The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters VPC traffic starting from rule group with the lowest numeric priority setting. This value must be greater than 100 and less than 9,000
         :param vpc: (experimental) The VPC that to associate with the rule group.
@@ -933,15 +975,21 @@
             
             
             rule_group.associate("Association",
                 priority=101,
                 vpc=my_vpc
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d760432d87440f1d9d763a89518f2699a8f5ebc2f80e4eee0cad66fb9d945d0e)
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
+            check_type(argname="argument mutation_protection", value=mutation_protection, expected_type=type_hints["mutation_protection"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "priority": priority,
             "vpc": vpc,
         }
         if mutation_protection is not None:
             self._values["mutation_protection"] = mutation_protection
         if name is not None:
             self._values["name"] = name
@@ -958,22 +1006,22 @@
         :stability: experimental
         '''
         result = self._values.get("priority")
         assert result is not None, "Required property 'priority' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC that to associate with the rule group.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
 
     @builtins.property
     def mutation_protection(self) -> typing.Optional[builtins.bool]:
         '''(experimental) If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections.
 
         :default: true
 
@@ -1017,15 +1065,15 @@
     },
 )
 class FirewallRuleGroupAssociationProps(FirewallRuleGroupAssociationOptions):
     def __init__(
         self,
         *,
         priority: jsii.Number,
-        vpc: aws_cdk.aws_ec2.IVpc,
+        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         mutation_protection: typing.Optional[builtins.bool] = None,
         name: typing.Optional[builtins.str] = None,
         firewall_rule_group: "IFirewallRuleGroup",
     ) -> None:
         '''(experimental) Properties for a Firewall Rule Group Association.
 
         :param priority: (experimental) The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters VPC traffic starting from rule group with the lowest numeric priority setting. This value must be greater than 100 and less than 9,000
@@ -1053,15 +1101,22 @@
                 vpc=vpc,
             
                 # the properties below are optional
                 mutation_protection=False,
                 name="name"
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__83da411f10ecd4b598d0ba8241ed0a5eb15f93d3bedcf56bea32403113edff28)
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
+            check_type(argname="argument mutation_protection", value=mutation_protection, expected_type=type_hints["mutation_protection"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument firewall_rule_group", value=firewall_rule_group, expected_type=type_hints["firewall_rule_group"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "priority": priority,
             "vpc": vpc,
             "firewall_rule_group": firewall_rule_group,
         }
         if mutation_protection is not None:
             self._values["mutation_protection"] = mutation_protection
         if name is not None:
@@ -1079,22 +1134,22 @@
         :stability: experimental
         '''
         result = self._values.get("priority")
         assert result is not None, "Required property 'priority' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
-    def vpc(self) -> aws_cdk.aws_ec2.IVpc:
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
         '''(experimental) The VPC that to associate with the rule group.
 
         :stability: experimental
         '''
         result = self._values.get("vpc")
         assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(aws_cdk.aws_ec2.IVpc, result)
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
 
     @builtins.property
     def mutation_protection(self) -> typing.Optional[builtins.bool]:
         '''(experimental) If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections.
 
         :default: true
 
@@ -1142,15 +1197,15 @@
     name_mapping={"name": "name", "rules": "rules"},
 )
 class FirewallRuleGroupProps:
     def __init__(
         self,
         *,
         name: typing.Optional[builtins.str] = None,
-        rules: typing.Optional[typing.Sequence[FirewallRule]] = None,
+        rules: typing.Optional[typing.Sequence[typing.Union[FirewallRule, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''(experimental) Properties for a Firewall Rule Group.
 
         :param name: (experimental) The name of the rule group. Default: - a CloudFormation generated name
         :param rules: (experimental) A list of rules for this group. Default: - no rules
 
         :stability: experimental
@@ -1166,15 +1221,19 @@
                     firewall_domain_list=my_block_list,
                     # block and reply with NODATA
                     action=route53resolver.FirewallRuleAction.block()
                 )
                 ]
             )
         '''
-        self._values: typing.Dict[str, typing.Any] = {}
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7bcc990fe1d7f82a8c07b96a7a276e0306150596cdae07e9a310ee5702d9e9dd)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument rules", value=rules, expected_type=type_hints["rules"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if name is not None:
             self._values["name"] = name
         if rules is not None:
             self._values["rules"] = rules
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
@@ -1207,84 +1266,84 @@
     def __repr__(self) -> str:
         return "FirewallRuleGroupProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-route53resolver-alpha.IFirewallDomainList")
-class IFirewallDomainList(aws_cdk.IResource, typing_extensions.Protocol):
+class IFirewallDomainList(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
     '''(experimental) A Firewall Domain List.
 
     :stability: experimental
     '''
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListId")
     def firewall_domain_list_id(self) -> builtins.str:
         '''(experimental) The ID of the domain list.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IFirewallDomainListProxy(
-    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
+    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
 ):
     '''(experimental) A Firewall Domain List.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-route53resolver-alpha.IFirewallDomainList"
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListId")
     def firewall_domain_list_id(self) -> builtins.str:
         '''(experimental) The ID of the domain list.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListId"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IFirewallDomainList).__jsii_proxy_class__ = lambda : _IFirewallDomainListProxy
 
 
 @jsii.interface(jsii_type="@aws-cdk/aws-route53resolver-alpha.IFirewallRuleGroup")
-class IFirewallRuleGroup(aws_cdk.IResource, typing_extensions.Protocol):
+class IFirewallRuleGroup(_aws_cdk_ceddda9d.IResource, typing_extensions.Protocol):
     '''(experimental) A Firewall Rule Group.
 
     :stability: experimental
     '''
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupId")
     def firewall_rule_group_id(self) -> builtins.str:
         '''(experimental) The ID of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         ...
 
 
 class _IFirewallRuleGroupProxy(
-    jsii.proxy_for(aws_cdk.IResource) # type: ignore[misc]
+    jsii.proxy_for(_aws_cdk_ceddda9d.IResource), # type: ignore[misc]
 ):
     '''(experimental) A Firewall Rule Group.
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-cdk/aws-route53resolver-alpha.IFirewallRuleGroup"
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupId")
     def firewall_rule_group_id(self) -> builtins.str:
         '''(experimental) The ID of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
@@ -1292,15 +1351,15 @@
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IFirewallRuleGroup).__jsii_proxy_class__ = lambda : _IFirewallRuleGroupProxy
 
 
 @jsii.implements(IFirewallDomainList)
 class FirewallDomainList(
-    aws_cdk.Resource,
+    _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-route53resolver-alpha.FirewallDomainList",
 ):
     '''(experimental) A Firewall Domain List.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -1318,146 +1377,155 @@
         asset_list = route53resolver.FirewallDomainList(self, "AssetList",
             domains=route53resolver.FirewallDomains.from_asset("/path/to/domains.txt")
         )
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         domains: FirewallDomains,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param domains: (experimental) A list of domains.
         :param name: (experimental) A name for the domain list. Default: - a CloudFormation generated name
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d88ae2f1abdd515eaaf6c8c66d5625be7fdc658b36001fd0e165ea83b038320a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirewallDomainListProps(domains=domains, name=name)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromFirewallDomainListId") # type: ignore[misc]
+    @jsii.member(jsii_name="fromFirewallDomainListId")
     @builtins.classmethod
     def from_firewall_domain_list_id(
         cls,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         firewall_domain_list_id: builtins.str,
     ) -> IFirewallDomainList:
         '''(experimental) Import an existing Firewall Rule Group.
 
         :param scope: -
         :param id: -
         :param firewall_domain_list_id: -
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9fac64f1151d9c654325fa60b63a3266f027fcfdd0f27cfc7dd25dca3626062d)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument firewall_domain_list_id", value=firewall_domain_list_id, expected_type=type_hints["firewall_domain_list_id"])
         return typing.cast(IFirewallDomainList, jsii.sinvoke(cls, "fromFirewallDomainListId", [scope, id, firewall_domain_list_id]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListArn")
     def firewall_domain_list_arn(self) -> builtins.str:
         '''(experimental) The ARN (Amazon Resource Name) of the domain list.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListCreationTime")
     def firewall_domain_list_creation_time(self) -> builtins.str:
         '''(experimental) The date and time that the domain list was created.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListCreationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListCreatorRequestId")
     def firewall_domain_list_creator_request_id(self) -> builtins.str:
         '''(experimental) The creator request ID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListCreatorRequestId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListDomainCount")
     def firewall_domain_list_domain_count(self) -> jsii.Number:
         '''(experimental) The number of domains in the list.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(jsii.Number, jsii.get(self, "firewallDomainListDomainCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListId")
     def firewall_domain_list_id(self) -> builtins.str:
         '''(experimental) The ID of the domain list.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListManagedOwnerName")
     def firewall_domain_list_managed_owner_name(self) -> builtins.str:
         '''(experimental) The owner of the list, used only for lists that are not managed by you.
 
         For example, the managed domain list ``AWSManagedDomainsMalwareDomainList``
         has the managed owner name ``Route 53 Resolver DNS Firewall``.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListManagedOwnerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListModificationTime")
     def firewall_domain_list_modification_time(self) -> builtins.str:
         '''(experimental) The date and time that the domain list was last modified.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListModificationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListStatus")
     def firewall_domain_list_status(self) -> builtins.str:
         '''(experimental) The status of the domain list.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallDomainListStatusMessage")
     def firewall_domain_list_status_message(self) -> builtins.str:
         '''(experimental) Additional information about the status of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallDomainListStatusMessage"))
 
 
 @jsii.implements(IFirewallRuleGroup)
 class FirewallRuleGroup(
-    aws_cdk.Resource,
+    _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-cdk/aws-route53resolver-alpha.FirewallRuleGroup",
 ):
     '''(experimental) A Firewall Rule Group.
 
     :stability: experimental
     :exampleMetadata: infused
@@ -1475,48 +1543,57 @@
             )
             ]
         )
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: typing.Optional[builtins.str] = None,
-        rules: typing.Optional[typing.Sequence[FirewallRule]] = None,
+        rules: typing.Optional[typing.Sequence[typing.Union[FirewallRule, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param name: (experimental) The name of the rule group. Default: - a CloudFormation generated name
         :param rules: (experimental) A list of rules for this group. Default: - no rules
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1cb24fa06a6d2f6631fd2f617858f3d92eba8ac1220751022ff38d3f87a6db20)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirewallRuleGroupProps(name=name, rules=rules)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="fromFirewallRuleGroupId") # type: ignore[misc]
+    @jsii.member(jsii_name="fromFirewallRuleGroupId")
     @builtins.classmethod
     def from_firewall_rule_group_id(
         cls,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         firewall_rule_group_id: builtins.str,
     ) -> IFirewallRuleGroup:
         '''(experimental) Import an existing Firewall Rule Group.
 
         :param scope: -
         :param id: -
         :param firewall_rule_group_id: -
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6af1f0d9981b2568b1050e7796f1a1b81df83547efa007299f4de89a58871c08)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument firewall_rule_group_id", value=firewall_rule_group_id, expected_type=type_hints["firewall_rule_group_id"])
         return typing.cast(IFirewallRuleGroup, jsii.sinvoke(cls, "fromFirewallRuleGroupId", [scope, id, firewall_rule_group_id]))
 
     @jsii.member(jsii_name="addRule")
     def add_rule(
         self,
         *,
         action: FirewallRuleAction,
@@ -1539,127 +1616,130 @@
 
     @jsii.member(jsii_name="associate")
     def associate(
         self,
         id: builtins.str,
         *,
         priority: jsii.Number,
-        vpc: aws_cdk.aws_ec2.IVpc,
+        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
         mutation_protection: typing.Optional[builtins.bool] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> FirewallRuleGroupAssociation:
         '''(experimental) Associates this Firewall Rule Group with a VPC.
 
         :param id: -
         :param priority: (experimental) The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters VPC traffic starting from rule group with the lowest numeric priority setting. This value must be greater than 100 and less than 9,000
         :param vpc: (experimental) The VPC that to associate with the rule group.
         :param mutation_protection: (experimental) If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections. Default: true
         :param name: (experimental) The name of the association. Default: - a CloudFormation generated name
 
         :stability: experimental
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2c7f8452576eb937895dbebdfe9c7ae375ecabfafd5e215cbfec8b69ad2074d2)
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirewallRuleGroupAssociationOptions(
             priority=priority,
             vpc=vpc,
             mutation_protection=mutation_protection,
             name=name,
         )
 
         return typing.cast(FirewallRuleGroupAssociation, jsii.invoke(self, "associate", [id, props]))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupArn")
     def firewall_rule_group_arn(self) -> builtins.str:
         '''(experimental) The ARN (Amazon Resource Name) of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupCreationTime")
     def firewall_rule_group_creation_time(self) -> builtins.str:
         '''(experimental) The date and time that the rule group was created.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupCreationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupCreatorRequestId")
     def firewall_rule_group_creator_request_id(self) -> builtins.str:
         '''(experimental) The creator request ID.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupCreatorRequestId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupId")
     def firewall_rule_group_id(self) -> builtins.str:
         '''(experimental) The ID of the rule group.
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupModificationTime")
     def firewall_rule_group_modification_time(self) -> builtins.str:
         '''(experimental) The date and time that the rule group was last modified.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupModificationTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupOwnerId")
     def firewall_rule_group_owner_id(self) -> builtins.str:
         '''(experimental) The AWS account ID for the account that created the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupOwnerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupRuleCount")
     def firewall_rule_group_rule_count(self) -> jsii.Number:
         '''(experimental) The number of rules in the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(jsii.Number, jsii.get(self, "firewallRuleGroupRuleCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupShareStatus")
     def firewall_rule_group_share_status(self) -> builtins.str:
         '''(experimental) Whether the rule group is shared with other AWS accounts, or was shared with the current account by another AWS account.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupShareStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupStatus")
     def firewall_rule_group_status(self) -> builtins.str:
         '''(experimental) The status of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
         return typing.cast(builtins.str, jsii.get(self, "firewallRuleGroupStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="firewallRuleGroupStatusMessage")
     def firewall_rule_group_status_message(self) -> builtins.str:
         '''(experimental) Additional information about the status of the rule group.
 
         :stability: experimental
         :attribute: true
         '''
@@ -1680,7 +1760,165 @@
     "FirewallRuleGroupAssociationProps",
     "FirewallRuleGroupProps",
     "IFirewallDomainList",
     "IFirewallRuleGroup",
 ]
 
 publication.publish()
+
+def _typecheckingstub__bcc6e5cbcbf161b026004146d290f4c2c5203dd60e43bb296ae451b7ea8afb50(
+    domain: builtins.str,
+    ttl: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__efcc739bead6cd1e2f6028bbf509537b88cdaab217e4ad29abcb83010af732aa(
+    *,
+    domain_file_url: typing.Optional[builtins.str] = None,
+    domains: typing.Optional[typing.Sequence[builtins.str]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e2694ecc77bbdf59285a53d044c17b801083d48fd6d9cf26c5798be8ef83cfd4(
+    *,
+    domains: FirewallDomains,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a7b0d1079af5d8eb8466e6719de93c31cc9a02bfc3b4b058593e609db394d240(
+    asset_path: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4db439b64de98348184f5457d37416fdf39df7bfa653f43e5546f736c932c7ba(
+    list: typing.Sequence[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9123f4606e1c6eda8fc3b706939d87b0209c2bea457af92c0af2a946a6684d64(
+    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    key: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9f74514d1763b172a7f7f23feabbb8360b780c1b88c0e33c8dd934f2542a42db(
+    url: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__beee843294402bd0b4634b78a18a987c0d888a0afb182d42637c4bf1d18c0908(
+    scope: _constructs_77d1e7e8.Construct,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c842a13b2d3ff276f74958de9ce814eafca72f45f15296caa8cf78d6ad8c39a5(
+    *,
+    action: FirewallRuleAction,
+    firewall_domain_list: IFirewallDomainList,
+    priority: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__908212340f1ac128d44306136d4c2b8737eeff37eab2b68c781cfb8d7345f036(
+    response: typing.Optional[DnsBlockResponse] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__66db44623853cec6127559e80b1ff37cd188ae6bb06e46d5500ca10c786695ec(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    firewall_rule_group: IFirewallRuleGroup,
+    priority: jsii.Number,
+    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+    mutation_protection: typing.Optional[builtins.bool] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d760432d87440f1d9d763a89518f2699a8f5ebc2f80e4eee0cad66fb9d945d0e(
+    *,
+    priority: jsii.Number,
+    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+    mutation_protection: typing.Optional[builtins.bool] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__83da411f10ecd4b598d0ba8241ed0a5eb15f93d3bedcf56bea32403113edff28(
+    *,
+    priority: jsii.Number,
+    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+    mutation_protection: typing.Optional[builtins.bool] = None,
+    name: typing.Optional[builtins.str] = None,
+    firewall_rule_group: IFirewallRuleGroup,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7bcc990fe1d7f82a8c07b96a7a276e0306150596cdae07e9a310ee5702d9e9dd(
+    *,
+    name: typing.Optional[builtins.str] = None,
+    rules: typing.Optional[typing.Sequence[typing.Union[FirewallRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d88ae2f1abdd515eaaf6c8c66d5625be7fdc658b36001fd0e165ea83b038320a(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    domains: FirewallDomains,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9fac64f1151d9c654325fa60b63a3266f027fcfdd0f27cfc7dd25dca3626062d(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    firewall_domain_list_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1cb24fa06a6d2f6631fd2f617858f3d92eba8ac1220751022ff38d3f87a6db20(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    name: typing.Optional[builtins.str] = None,
+    rules: typing.Optional[typing.Sequence[typing.Union[FirewallRule, typing.Dict[builtins.str, typing.Any]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6af1f0d9981b2568b1050e7796f1a1b81df83547efa007299f4de89a58871c08(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    firewall_rule_group_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2c7f8452576eb937895dbebdfe9c7ae375ecabfafd5e215cbfec8b69ad2074d2(
+    id: builtins.str,
+    *,
+    priority: jsii.Number,
+    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
+    mutation_protection: typing.Optional[builtins.bool] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-route53resolver-alpha
-Version: 2.9.0a0
+Version: 2.90.0a0
 Summary: The CDK Construct Library for AWS::Route53Resolver
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 1
-Requires-Python: >=3.6
+Classifier: Framework :: AWS CDK :: 2
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Amazon Route53 Resolver Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
@@ -134,9 +134,7 @@
 
 
 rule_group.associate("Association",
     priority=101,
     vpc=my_vpc
 )
 ```
-
-
```

### Comparing `aws-cdk.aws-route53resolver-alpha-2.9.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-route53resolver-alpha-2.90.0a0/src/aws_cdk.aws_route53resolver_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_route53resolver_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_route53resolver_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_route53resolver_alpha.egg-info/requires.txt
 src/aws_cdk.aws_route53resolver_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_route53resolver_alpha/__init__.py
 src/aws_cdk/aws_route53resolver_alpha/py.typed
 src/aws_cdk/aws_route53resolver_alpha/_jsii/__init__.py
-src/aws_cdk/aws_route53resolver_alpha/_jsii/aws-route53resolver-alpha@2.9.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_route53resolver_alpha/_jsii/aws-route53resolver-alpha@2.90.0-alpha.0.jsii.tgz
```

