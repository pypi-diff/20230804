# Comparing `tmp/types-aiobotocore-sesv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sesv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sesv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-sesv2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-sesv2-2.5.2.post1.tar` & `types-aiobotocore-sesv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.537456 types-aiobotocore-sesv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-08-02 14:53:01.533456 types-aiobotocore-sesv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.537456 types-aiobotocore-sesv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.529456 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59893 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59798 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71044 2023-08-02 14:49:44.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70974 2023-08-02 14:49:44.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.533456 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.606643 types-aiobotocore-sesv2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12088 2023-08-04 13:59:26.606643 types-aiobotocore-sesv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10578 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.606643 types-aiobotocore-sesv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.596643 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      426 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      425 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59863 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59768 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11881 2023-08-04 13:53:35.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11879 2023-08-04 13:53:35.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    69244 2023-08-04 13:53:36.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    69174 2023-08-04 13:53:36.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:34.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.606643 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12088 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      700 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:26.000000 types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/LICENSE` & `types-aiobotocore-sesv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/setup.py` & `types-aiobotocore-sesv2-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sesv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__main__.py` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SESV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SESV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.py` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -79,20 +79,20 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsUnionTypeDef,
+    ReputationOptionsTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsUnionTypeDef,
+    SuppressionOptionsTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -172,18 +172,18 @@
 
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
+        ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
@@ -939,15 +939,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.pyi` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -79,20 +79,20 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsUnionTypeDef,
+    ReputationOptionsTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsUnionTypeDef,
+    SuppressionOptionsTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
     TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
@@ -165,18 +165,18 @@
         """
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
+        ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
@@ -864,15 +864,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.py` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
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
@@ -247,14 +248,15 @@
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
@@ -333,26 +335,28 @@
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

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.pyi` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
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
@@ -245,14 +246,15 @@
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
@@ -331,26 +333,28 @@
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

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.py` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,28 +107,25 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
-    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsOutputTypeDef",
-    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
@@ -200,15 +197,14 @@
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
@@ -228,55 +224,51 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
-    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
-    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
+    "EventDestinationTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionUnionTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -729,28 +721,19 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionOutputTypeDef",
-    {
-        "Global": bool,
-        "TrackedIsps": List[str],
-    },
-    total=False,
-)
-
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": Sequence[str],
+        "TrackedIsps": List[str],
     },
     total=False,
 )
 
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
@@ -827,31 +810,14 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ReputationOptionsOutputTypeDef = TypedDict(
-    "ReputationOptionsOutputTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": datetime,
-    },
-    total=False,
-)
-
-SuppressionOptionsOutputTypeDef = TypedDict(
-    "SuppressionOptionsOutputTypeDef",
-    {
-        "SuppressedReasons": List[SuppressionListReasonType],
-    },
-    total=False,
-)
-
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
@@ -1726,21 +1692,14 @@
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CloudWatchDestinationOutputTypeDef = TypedDict(
-    "CloudWatchDestinationOutputTypeDef",
-    {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
-    },
-)
-
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
@@ -2083,44 +2042,33 @@
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
-    {
-        "Domain": str,
-        "SubscriptionStartDate": datetime,
-        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": TimestampTypeDef,
+        "SubscriptionStartDate": datetime,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2250,60 +2198,59 @@
 BatchGetMetricDataRequestRequestTypeDef = TypedDict(
     "BatchGetMetricDataRequestRequestTypeDef",
     {
         "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
     },
 )
 
-ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
 
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2320,23 +2267,42 @@
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
-    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
-]
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
+
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -2397,18 +2363,18 @@
 
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
@@ -2526,22 +2492,14 @@
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2552,36 +2510,22 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
-
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.pyi` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,28 +106,25 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
-    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsOutputTypeDef",
-    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
@@ -199,15 +196,14 @@
     "SendEmailResponseTypeDef",
     "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
@@ -227,55 +223,51 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
-    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
-    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
+    "EventDestinationTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionUnionTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -722,28 +714,19 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionOutputTypeDef",
-    {
-        "Global": bool,
-        "TrackedIsps": List[str],
-    },
-    total=False,
-)
-
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": Sequence[str],
+        "TrackedIsps": List[str],
     },
     total=False,
 )
 
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
@@ -820,31 +803,14 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ReputationOptionsOutputTypeDef = TypedDict(
-    "ReputationOptionsOutputTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": datetime,
-    },
-    total=False,
-)
-
-SuppressionOptionsOutputTypeDef = TypedDict(
-    "SuppressionOptionsOutputTypeDef",
-    {
-        "SuppressedReasons": List[SuppressionListReasonType],
-    },
-    total=False,
-)
-
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
@@ -1691,21 +1657,14 @@
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CloudWatchDestinationOutputTypeDef = TypedDict(
-    "CloudWatchDestinationOutputTypeDef",
-    {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
-    },
-)
-
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
@@ -2034,44 +1993,33 @@
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
-    {
-        "Domain": str,
-        "SubscriptionStartDate": datetime,
-        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": TimestampTypeDef,
+        "SubscriptionStartDate": datetime,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2197,58 +2145,57 @@
 BatchGetMetricDataRequestRequestTypeDef = TypedDict(
     "BatchGetMetricDataRequestRequestTypeDef",
     {
         "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
     },
 )
 
-ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2265,23 +2212,40 @@
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
-    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
-]
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+    },
+    total=False,
+)
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
@@ -2340,18 +2304,18 @@
 
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
@@ -2463,22 +2427,14 @@
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2489,34 +2445,22 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/SOURCES.txt` & `types-aiobotocore-sesv2-2.5.2.post2/types_aiobotocore_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

