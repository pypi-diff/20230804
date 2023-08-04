# Comparing `tmp/types-aiobotocore-opensearch-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-opensearch-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opensearch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-opensearch-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-opensearch-2.5.2.post1.tar` & `types-aiobotocore-opensearch-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43489 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43426 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68915 2023-08-02 14:44:20.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68858 2023-08-02 14:44:20.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.036643 types-aiobotocore-opensearch-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12422 2023-08-04 13:59:20.036643 types-aiobotocore-opensearch-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10885 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.036643 types-aiobotocore-opensearch-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.036643 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      501 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      500 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43479 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43416 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15467 2023-08-04 13:45:59.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15465 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    68099 2023-08-04 13:46:02.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    68042 2023-08-04 13:45:59.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:58.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.036643 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12422 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      785 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:19.000000 types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/LICENSE` & `types-aiobotocore-opensearch-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/setup.py` & `types-aiobotocore-opensearch-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opensearch",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__main__.py` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.OpenSearchService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.py` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsUnionTypeDef,
+    AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -747,15 +747,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.pyi` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsUnionTypeDef,
+    AutoTuneOptionsTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -690,15 +690,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.py` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,15 @@
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
@@ -371,14 +372,15 @@
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
@@ -457,26 +459,28 @@
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
@@ -637,14 +641,15 @@
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

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.pyi` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,15 @@
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
@@ -369,14 +370,15 @@
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
@@ -455,26 +457,28 @@
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
@@ -635,14 +639,15 @@
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

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.py` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,14 @@
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
@@ -220,15 +219,14 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
-    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -253,15 +251,14 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
-    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -1498,24 +1495,14 @@
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
-    {
-        "StartAt": datetime,
-        "Duration": DurationTypeDef,
-        "CronExpressionForRecurrence": str,
-    },
-    total=False,
-)
-
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -2052,25 +2039,14 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsExtraOutputTypeDef = TypedDict(
-    "AutoTuneOptionsExtraOutputTypeDef",
-    {
-        "DesiredState": AutoTuneDesiredStateType,
-        "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
-        "UseOffPeakWindow": bool,
-    },
-    total=False,
-)
-
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2078,15 +2054,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2380,21 +2356,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsExtraOutputTypeDef,
+        "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.pyi` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,14 @@
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
@@ -219,15 +218,14 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
-    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -252,15 +250,14 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
-    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -1457,24 +1454,14 @@
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
-    {
-        "StartAt": datetime,
-        "Duration": DurationTypeDef,
-        "CronExpressionForRecurrence": str,
-    },
-    total=False,
-)
-
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -2003,25 +1990,14 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsExtraOutputTypeDef = TypedDict(
-    "AutoTuneOptionsExtraOutputTypeDef",
-    {
-        "DesiredState": AutoTuneDesiredStateType,
-        "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
-        "UseOffPeakWindow": bool,
-    },
-    total=False,
-)
-
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2029,15 +2005,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2329,21 +2305,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsExtraOutputTypeDef,
+        "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/SOURCES.txt` & `types-aiobotocore-opensearch-2.5.2.post2/types_aiobotocore_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

