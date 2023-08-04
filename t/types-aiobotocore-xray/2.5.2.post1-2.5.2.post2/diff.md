# Comparing `tmp/types-aiobotocore-xray-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-xray-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-xray-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-xray-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-xray-2.5.2.post1.tar` & `types-aiobotocore-xray-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.413423 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27732 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-08-02 14:51:31.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44087 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.413423 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12653 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2027 2023-08-04 13:56:30.000000 types-aiobotocore-xray-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2635 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2634 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      920 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27722 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27673 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10047 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10045 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12648 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12636 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43285 2023-08-04 13:56:32.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43236 2023-08-04 13:56:32.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-xray-2.5.2.post1/LICENSE` & `types-aiobotocore-xray-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post1/setup.py` & `types-aiobotocore-xray-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-xray",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.pyi` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__main__.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.XRay 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.XRay 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleUnionTypeDef,
+    SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
     TimestampTypeDef,
     UpdateGroupResultTypeDef,
@@ -155,15 +155,15 @@
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
 
     async def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_sampling_rule)
         """
```

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.pyi` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleUnionTypeDef,
+    SamplingRuleTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
     TimestampTypeDef,
     UpdateGroupResultTypeDef,
@@ -146,15 +146,15 @@
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
     async def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_sampling_rule)
         """
```

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -261,26 +263,28 @@
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
@@ -453,14 +457,15 @@
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

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.pyi` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -173,14 +174,15 @@
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
@@ -259,26 +261,28 @@
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
@@ -451,14 +455,15 @@
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

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.pyi` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.py` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
     "PaginatorConfigTypeDef",
@@ -75,15 +74,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
-    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
@@ -96,14 +94,15 @@
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
+    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
@@ -119,37 +118,35 @@
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
-    "SamplingRuleRecordTypeDef",
-    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "CreateSamplingRuleResultTypeDef",
+    "DeleteSamplingRuleResultTypeDef",
+    "GetSamplingRulesResultTypeDef",
+    "UpdateSamplingRuleResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
-    "CreateSamplingRuleResultTypeDef",
-    "DeleteSamplingRuleResultTypeDef",
-    "GetSamplingRulesResultTypeDef",
-    "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -232,21 +229,19 @@
     "_OptionalBatchGetTracesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
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
@@ -292,19 +287,17 @@
         "RuleName": str,
         "RuleARN": str,
         "Attributes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SamplingRuleTypeDef(_RequiredSamplingRuleTypeDef, _OptionalSamplingRuleTypeDef):
     pass
 
-
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
@@ -320,22 +313,20 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -425,21 +416,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
-
 TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
@@ -504,21 +493,19 @@
     "_OptionalGetTraceGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTraceGraphRequestRequestTypeDef(
     _RequiredGetTraceGraphRequestRequestTypeDef, _OptionalGetTraceGraphRequestRequestTypeDef
 ):
     pass
 
-
 SamplingStrategyTypeDef = TypedDict(
     "SamplingStrategyTypeDef",
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
@@ -591,44 +578,40 @@
     "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
         "NextToken": str,
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
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalPutEncryptionConfigRequestRequestTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
-
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -637,21 +620,19 @@
     {
         "PolicyRevisionId": str,
         "BypassPolicyLockoutCheck": bool,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -679,46 +660,14 @@
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
-_RequiredSamplingRuleOutputTypeDef = TypedDict(
-    "_RequiredSamplingRuleOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Priority": int,
-        "FixedRate": float,
-        "ReservoirSize": int,
-        "ServiceName": str,
-        "ServiceType": str,
-        "Host": str,
-        "HTTPMethod": str,
-        "URLPath": str,
-        "Version": int,
-    },
-)
-_OptionalSamplingRuleOutputTypeDef = TypedDict(
-    "_OptionalSamplingRuleOutputTypeDef",
-    {
-        "RuleName": str,
-        "RuleARN": str,
-        "Attributes": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class SamplingRuleOutputTypeDef(
-    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
-):
-    pass
-
-
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -787,22 +736,20 @@
     "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
     _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
 ):
     pass
 
-
 GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
     "GetGroupsRequestGetGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -833,22 +780,20 @@
     "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
     _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
 ):
     pass
 
-
 ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -863,22 +808,20 @@
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
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -920,21 +863,19 @@
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -958,21 +899,29 @@
     "_OptionalCreateSamplingRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
 
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
@@ -1042,22 +991,20 @@
     "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInsightImpactGraphRequestRequestTypeDef(
     _RequiredGetInsightImpactGraphRequestRequestTypeDef,
     _OptionalGetInsightImpactGraphRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1069,22 +1016,20 @@
         "GroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1094,22 +1039,20 @@
         "GroupName": str,
         "GroupARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
     _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1119,21 +1062,19 @@
         "GroupName": str,
         "GroupARN": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1146,22 +1087,20 @@
         "Period": int,
         "ForecastStatistics": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1174,22 +1113,20 @@
         "Period": int,
         "ForecastStatistics": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
     "_RequiredSamplingStatisticsDocumentTypeDef",
     {
         "RuleName": str,
         "ClientID": str,
         "Timestamp": TimestampTypeDef,
         "RequestCount": int,
@@ -1200,21 +1137,19 @@
     "_OptionalSamplingStatisticsDocumentTypeDef",
     {
         "BorrowCount": int,
     },
     total=False,
 )
 
-
 class SamplingStatisticsDocumentTypeDef(
     _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
 ):
     pass
 
-
 _RequiredTelemetryRecordTypeDef = TypedDict(
     "_RequiredTelemetryRecordTypeDef",
     {
         "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalTelemetryRecordTypeDef = TypedDict(
@@ -1225,19 +1160,17 @@
         "SegmentsSpilloverCount": int,
         "SegmentsRejectedCount": int,
         "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
     },
     total=False,
 )
 
-
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
-
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1268,22 +1201,20 @@
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1295,21 +1226,19 @@
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
-
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1353,25 +1282,14 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleOutputTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
-
-SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1466,14 +1384,47 @@
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1542,22 +1493,20 @@
         "EC2InstanceId": str,
         "Hostname": str,
         "ResourceARN": str,
     },
     total=False,
 )
 
-
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
-
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
@@ -1573,47 +1522,14 @@
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.pyi` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
     "PaginatorConfigTypeDef",
@@ -74,15 +75,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
-    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
     "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
@@ -95,14 +95,15 @@
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
+    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
     "GetInsightImpactGraphRequestRequestTypeDef",
@@ -118,37 +119,35 @@
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
-    "SamplingRuleRecordTypeDef",
-    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
+    "CreateSamplingRuleResultTypeDef",
+    "DeleteSamplingRuleResultTypeDef",
+    "GetSamplingRulesResultTypeDef",
+    "UpdateSamplingRuleResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
     "GetSamplingTargetsRequestRequestTypeDef",
     "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
-    "CreateSamplingRuleResultTypeDef",
-    "DeleteSamplingRuleResultTypeDef",
-    "GetSamplingRulesResultTypeDef",
-    "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -231,19 +230,21 @@
     "_OptionalBatchGetTracesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
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
@@ -289,17 +290,19 @@
         "RuleName": str,
         "RuleARN": str,
         "Attributes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SamplingRuleTypeDef(_RequiredSamplingRuleTypeDef, _OptionalSamplingRuleTypeDef):
     pass
 
+
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
@@ -315,20 +318,22 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -418,19 +423,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
+
 TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
@@ -495,19 +502,21 @@
     "_OptionalGetTraceGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTraceGraphRequestRequestTypeDef(
     _RequiredGetTraceGraphRequestRequestTypeDef, _OptionalGetTraceGraphRequestRequestTypeDef
 ):
     pass
 
+
 SamplingStrategyTypeDef = TypedDict(
     "SamplingStrategyTypeDef",
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
@@ -580,40 +589,44 @@
     "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalPutEncryptionConfigRequestRequestTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
+
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -622,19 +635,21 @@
     {
         "PolicyRevisionId": str,
         "BypassPolicyLockoutCheck": bool,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -662,44 +677,14 @@
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
-_RequiredSamplingRuleOutputTypeDef = TypedDict(
-    "_RequiredSamplingRuleOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "Priority": int,
-        "FixedRate": float,
-        "ReservoirSize": int,
-        "ServiceName": str,
-        "ServiceType": str,
-        "Host": str,
-        "HTTPMethod": str,
-        "URLPath": str,
-        "Version": int,
-    },
-)
-_OptionalSamplingRuleOutputTypeDef = TypedDict(
-    "_OptionalSamplingRuleOutputTypeDef",
-    {
-        "RuleName": str,
-        "RuleARN": str,
-        "Attributes": Dict[str, str],
-    },
-    total=False,
-)
-
-class SamplingRuleOutputTypeDef(
-    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
-):
-    pass
-
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -768,20 +753,22 @@
     "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
     _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
     _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
 ):
     pass
 
+
 GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
     "GetGroupsRequestGetGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -812,20 +799,22 @@
     "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
     _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
 ):
     pass
 
+
 ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
     "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -840,20 +829,22 @@
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
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -895,19 +886,21 @@
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -931,20 +924,32 @@
     "_OptionalCreateSamplingRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
+
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
+
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
         "TotalCount": int,
@@ -1013,20 +1018,22 @@
     "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInsightImpactGraphRequestRequestTypeDef(
     _RequiredGetInsightImpactGraphRequestRequestTypeDef,
     _OptionalGetInsightImpactGraphRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1038,20 +1045,22 @@
         "GroupName": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInsightSummariesRequestRequestTypeDef(
     _RequiredGetInsightSummariesRequestRequestTypeDef,
     _OptionalGetInsightSummariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1061,20 +1070,22 @@
         "GroupName": str,
         "GroupARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
     _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
     _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceGraphRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1084,19 +1095,21 @@
         "GroupName": str,
         "GroupARN": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetServiceGraphRequestRequestTypeDef(
     _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1109,20 +1122,22 @@
         "Period": int,
         "ForecastStatistics": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1135,20 +1150,22 @@
         "Period": int,
         "ForecastStatistics": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
     _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
     _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
     "_RequiredSamplingStatisticsDocumentTypeDef",
     {
         "RuleName": str,
         "ClientID": str,
         "Timestamp": TimestampTypeDef,
         "RequestCount": int,
@@ -1159,19 +1176,21 @@
     "_OptionalSamplingStatisticsDocumentTypeDef",
     {
         "BorrowCount": int,
     },
     total=False,
 )
 
+
 class SamplingStatisticsDocumentTypeDef(
     _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
 ):
     pass
 
+
 _RequiredTelemetryRecordTypeDef = TypedDict(
     "_RequiredTelemetryRecordTypeDef",
     {
         "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalTelemetryRecordTypeDef = TypedDict(
@@ -1182,17 +1201,19 @@
         "SegmentsSpilloverCount": int,
         "SegmentsRejectedCount": int,
         "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
     },
     total=False,
 )
 
+
 class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
     pass
 
+
 GetSamplingStatisticSummariesResultTypeDef = TypedDict(
     "GetSamplingStatisticSummariesResultTypeDef",
     {
         "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1223,20 +1244,22 @@
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
@@ -1248,19 +1271,21 @@
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
+
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1304,25 +1329,14 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleOutputTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
-
-SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1417,14 +1431,47 @@
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
         "StartTime": datetime,
         "EndTime": datetime,
         "SummaryStatistics": EdgeStatisticsTypeDef,
@@ -1493,20 +1540,22 @@
         "EC2InstanceId": str,
         "Hostname": str,
         "ResourceARN": str,
     },
     total=False,
 )
 
+
 class PutTelemetryRecordsRequestRequestTypeDef(
     _RequiredPutTelemetryRecordsRequestRequestTypeDef,
     _OptionalPutTelemetryRecordsRequestRequestTypeDef,
 ):
     pass
 
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
@@ -1522,47 +1571,14 @@
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/SOURCES.txt` & `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

