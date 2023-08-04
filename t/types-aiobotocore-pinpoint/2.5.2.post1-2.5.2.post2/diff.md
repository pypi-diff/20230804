# Comparing `tmp/types-aiobotocore-pinpoint-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-pinpoint-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-pinpoint-2.5.2.post1.tar` & `types-aiobotocore-pinpoint-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.069497 types-aiobotocore-pinpoint-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30318 2023-08-02 14:52:48.069497 types-aiobotocore-pinpoint-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28796 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:48.069497 types-aiobotocore-pinpoint-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.061497 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83867 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83737 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   169709 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   169484 2023-08-02 14:44:52.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:50.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.069497 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30318 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.246643 types-aiobotocore-pinpoint-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12231 2023-08-04 13:59:21.246643 types-aiobotocore-pinpoint-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10709 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.246643 types-aiobotocore-pinpoint-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.246643 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      450 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      449 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83857 2023-08-04 13:46:47.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83727 2023-08-04 13:46:47.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10918 2023-08-04 13:46:48.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10916 2023-08-04 13:46:47.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   159810 2023-08-04 13:46:53.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   159595 2023-08-04 13:46:50.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:45.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.246643 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12231 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/LICENSE` & `types-aiobotocore-pinpoint-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/setup.py` & `types-aiobotocore-pinpoint-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Pinpoint 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/__main__.py` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Pinpoint 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Pinpoint 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
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

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/client.py` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelUnionTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1284,15 +1284,15 @@
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_users_messages)
         """
 
     async def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
+        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#tag_resource)
```

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/client.pyi` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     SendMessagesResponseTypeDef,
     SendOTPMessageRequestParametersTypeDef,
     SendOTPMessageResponseTypeDef,
     SendUsersMessageRequestTypeDef,
     SendUsersMessagesResponseTypeDef,
     SMSChannelRequestTypeDef,
     SMSTemplateRequestTypeDef,
-    TagsModelUnionTypeDef,
+    TagsModelTypeDef,
     TemplateActiveVersionRequestTypeDef,
     TimestampTypeDef,
     UpdateAdmChannelResponseTypeDef,
     UpdateApnsChannelResponseTypeDef,
     UpdateApnsSandboxChannelResponseTypeDef,
     UpdateApnsVoipChannelResponseTypeDef,
     UpdateApnsVoipSandboxChannelResponseTypeDef,
@@ -1182,15 +1182,15 @@
         """
         Creates and sends a message to a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_users_messages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#send_users_messages)
         """
     async def tag_resource(
-        self, *, ResourceArn: str, TagsModel: TagsModelUnionTypeDef
+        self, *, ResourceArn: str, TagsModel: TagsModelTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds one or more tags (keys and values) to an application, campaign, message
         template, or segment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint/client/#tag_resource)
```

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/literals.py` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -252,14 +253,15 @@
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
@@ -338,26 +340,28 @@
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

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/literals.pyi` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
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
@@ -250,14 +251,15 @@
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
@@ -336,26 +338,28 @@
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

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/type_defs.py` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,28 +70,28 @@
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
+    "JourneyTimeframeCapTypeDef",
     "CampaignHookTypeDef",
     "CampaignLimitsTypeDef",
     "QuietTimeTypeDef",
-    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
     "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
     "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationOutputTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
@@ -99,15 +99,14 @@
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
     "JourneyCustomMessageTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
@@ -145,18 +144,16 @@
     "JourneyEmailMessageTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
-    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
-    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
@@ -213,23 +210,21 @@
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
-    "JourneyLimitsTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelOutputTypeDef",
+    "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
@@ -240,15 +235,14 @@
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
-    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
@@ -257,20 +251,19 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "ApplicationSettingsResourceTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
+    "ApplicationSettingsJourneyLimitsTypeDef",
+    "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "RawEmailTypeDef",
     "ChannelsResponseTypeDef",
-    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
@@ -308,15 +301,14 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
-    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
     "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
@@ -345,19 +337,17 @@
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
+    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
-    "EndpointResponseTypeDef",
-    "EventDimensionsOutputTypeDef",
-    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
@@ -374,148 +364,129 @@
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
-    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
-    "GetApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
+    "ApplicationSettingsResourceTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
     "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
-    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "CampaignEventFilterOutputTypeDef",
-    "EventConditionOutputTypeDef",
-    "EventFilterOutputTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
-    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
+    "GetApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
-    "ScheduleOutputTypeDef",
-    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
-    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageOutputTypeDef",
     "CampaignInAppMessageTypeDef",
     "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
-    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
-    "SegmentGroupOutputTypeDef",
-    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationOutputTypeDef",
     "MessageConfigurationTypeDef",
     "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
     "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
-    "SegmentGroupListOutputTypeDef",
-    "ConditionOutputTypeDef",
-    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
     "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
-    "ConditionalSplitActivityOutputTypeDef",
-    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
     "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
-    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -944,14 +915,23 @@
 
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
 
+JourneyTimeframeCapTypeDef = TypedDict(
+    "JourneyTimeframeCapTypeDef",
+    {
+        "Cap": int,
+        "Days": int,
+    },
+    total=False,
+)
+
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -975,35 +955,14 @@
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
-_RequiredAttributeDimensionOutputTypeDef = TypedDict(
-    "_RequiredAttributeDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-_OptionalAttributeDimensionOutputTypeDef = TypedDict(
-    "_OptionalAttributeDimensionOutputTypeDef",
-    {
-        "AttributeType": AttributeTypeType,
-    },
-    total=False,
-)
-
-
-class AttributeDimensionOutputTypeDef(
-    _RequiredAttributeDimensionOutputTypeDef, _OptionalAttributeDimensionOutputTypeDef
-):
-    pass
-
-
 _RequiredAttributeDimensionTypeDef = TypedDict(
     "_RequiredAttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalAttributeDimensionTypeDef = TypedDict(
@@ -1140,32 +1099,31 @@
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationOutputTypeDef",
+_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationTypeDef",
     {
         "DeliveryUri": str,
     },
 )
-_OptionalCustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationOutputTypeDef",
+_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationTypeDef",
     {
-        "EndpointTypes": List[EndpointTypesElementType],
+        "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
 
-class CustomDeliveryConfigurationOutputTypeDef(
-    _RequiredCustomDeliveryConfigurationOutputTypeDef,
-    _OptionalCustomDeliveryConfigurationOutputTypeDef,
+class CustomDeliveryConfigurationTypeDef(
+    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
 
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
@@ -1407,35 +1365,14 @@
         "tags": Mapping[str, str],
         "TemplateDescription": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationTypeDef",
-    {
-        "DeliveryUri": str,
-    },
-)
-_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationTypeDef",
-    {
-        "EndpointTypes": Sequence[EndpointTypesElementType],
-    },
-    total=False,
-)
-
-
-class CustomDeliveryConfigurationTypeDef(
-    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
-):
-    pass
-
-
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
@@ -1673,25 +1610,27 @@
         "ApplicationId": str,
     },
 )
 
 _RequiredGCMChannelResponseTypeDef = TypedDict(
     "_RequiredGCMChannelResponseTypeDef",
     {
-        "Credential": str,
         "Platform": str,
     },
 )
 _OptionalGCMChannelResponseTypeDef = TypedDict(
     "_OptionalGCMChannelResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
+        "Credential": str,
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
         "HasCredential": bool,
+        "HasFcmServiceCredentials": bool,
         "Id": str,
         "IsArchived": bool,
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
@@ -1904,14 +1843,15 @@
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
         "IconReference": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
+        "PreferredAuthenticationMethod": str,
         "Priority": str,
         "RawContent": str,
         "RestrictedPackageName": str,
         "SilentPush": bool,
         "SmallImageIconUrl": str,
         "Sound": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2041,15 +1981,15 @@
     },
     total=False,
 )
 
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": Mapping[str, Sequence[str]],
+        "UserAttributes": Dict[str, List[str]],
         "UserId": str,
     },
     total=False,
 )
 
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
@@ -2081,23 +2021,14 @@
 
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
 
-EndpointUserOutputTypeDef = TypedDict(
-    "EndpointUserOutputTypeDef",
-    {
-        "UserAttributes": Dict[str, List[str]],
-        "UserId": str,
-    },
-    total=False,
-)
-
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2110,35 +2041,14 @@
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
 
-_RequiredSetDimensionOutputTypeDef = TypedDict(
-    "_RequiredSetDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-_OptionalSetDimensionOutputTypeDef = TypedDict(
-    "_OptionalSetDimensionOutputTypeDef",
-    {
-        "DimensionType": DimensionTypeType,
-    },
-    total=False,
-)
-
-
-class SetDimensionOutputTypeDef(
-    _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
-):
-    pass
-
-
 _RequiredSetDimensionTypeDef = TypedDict(
     "_RequiredSetDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalSetDimensionTypeDef = TypedDict(
@@ -2203,35 +2113,25 @@
 
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
 
-_RequiredGCMChannelRequestTypeDef = TypedDict(
-    "_RequiredGCMChannelRequestTypeDef",
+GCMChannelRequestTypeDef = TypedDict(
+    "GCMChannelRequestTypeDef",
     {
         "ApiKey": str,
-    },
-)
-_OptionalGCMChannelRequestTypeDef = TypedDict(
-    "_OptionalGCMChannelRequestTypeDef",
-    {
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
+        "ServiceJson": str,
     },
     total=False,
 )
 
-
-class GCMChannelRequestTypeDef(
-    _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
-):
-    pass
-
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -3056,43 +2956,22 @@
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
-JourneyLimitsTypeDef = TypedDict(
-    "JourneyLimitsTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
 
-JourneyScheduleOutputTypeDef = TypedDict(
-    "JourneyScheduleOutputTypeDef",
-    {
-        "EndTime": datetime,
-        "StartTime": datetime,
-        "Timezone": str,
-    },
-    total=False,
-)
-
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
     {
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
@@ -3144,16 +3023,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagsModelOutputTypeDef = TypedDict(
-    "TagsModelOutputTypeDef",
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 
 _RequiredListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateVersionsRequestRequestTypeDef",
@@ -3408,21 +3287,14 @@
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
 )
 
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-)
-
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
@@ -3615,46 +3487,33 @@
     {
         "Item": List[ApplicationResponseTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+ApplicationSettingsJourneyLimitsTypeDef = TypedDict(
+    "ApplicationSettingsJourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "DailyCap": int,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
-
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+JourneyLimitsTypeDef = TypedDict(
+    "JourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
 UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
@@ -3674,26 +3533,14 @@
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-ClosedDaysOutputTypeDef = TypedDict(
-    "ClosedDaysOutputTypeDef",
-    {
-        "EMAIL": List[ClosedDaysRuleTypeDef],
-        "SMS": List[ClosedDaysRuleTypeDef],
-        "PUSH": List[ClosedDaysRuleTypeDef],
-        "VOICE": List[ClosedDaysRuleTypeDef],
-        "CUSTOM": List[ClosedDaysRuleTypeDef],
-    },
-    total=False,
-)
-
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
         "EMAIL": Sequence[ClosedDaysRuleTypeDef],
         "SMS": Sequence[ClosedDaysRuleTypeDef],
         "PUSH": Sequence[ClosedDaysRuleTypeDef],
         "VOICE": Sequence[ClosedDaysRuleTypeDef],
@@ -4109,27 +3956,14 @@
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-CustomMessageActivityOutputTypeDef = TypedDict(
-    "CustomMessageActivityOutputTypeDef",
-    {
-        "DeliveryUri": str,
-        "EndpointTypes": List[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -4474,14 +4308,36 @@
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserTypeDef,
     },
     total=False,
 )
 
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
+    {
+        "Address": str,
+        "ApplicationId": str,
+        "Attributes": Dict[str, List[str]],
+        "ChannelType": ChannelTypeType,
+        "CohortId": str,
+        "CreationDate": str,
+        "Demographic": EndpointDemographicTypeDef,
+        "EffectiveDate": str,
+        "EndpointStatus": str,
+        "Id": str,
+        "Location": EndpointLocationTypeDef,
+        "Metrics": Dict[str, float],
+        "OptOut": str,
+        "RequestId": str,
+        "User": EndpointUserTypeDef,
+    },
+    total=False,
+)
+
 PublicEndpointTypeDef = TypedDict(
     "PublicEndpointTypeDef",
     {
         "Address": str,
         "Attributes": Mapping[str, Sequence[str]],
         "ChannelType": ChannelTypeType,
         "Demographic": EndpointDemographicTypeDef,
@@ -4514,59 +4370,14 @@
 
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
 
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
-    {
-        "Address": str,
-        "ApplicationId": str,
-        "Attributes": Dict[str, List[str]],
-        "ChannelType": ChannelTypeType,
-        "CohortId": str,
-        "CreationDate": str,
-        "Demographic": EndpointDemographicTypeDef,
-        "EffectiveDate": str,
-        "EndpointStatus": str,
-        "Id": str,
-        "Location": EndpointLocationTypeDef,
-        "Metrics": Dict[str, float],
-        "OptOut": str,
-        "RequestId": str,
-        "User": EndpointUserOutputTypeDef,
-    },
-    total=False,
-)
-
-EventDimensionsOutputTypeDef = TypedDict(
-    "EventDimensionsOutputTypeDef",
-    {
-        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "EventType": SetDimensionOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-SegmentDemographicsOutputTypeDef = TypedDict(
-    "SegmentDemographicsOutputTypeDef",
-    {
-        "AppVersion": SetDimensionOutputTypeDef,
-        "Channel": SetDimensionOutputTypeDef,
-        "DeviceType": SetDimensionOutputTypeDef,
-        "Make": SetDimensionOutputTypeDef,
-        "Model": SetDimensionOutputTypeDef,
-        "Platform": SetDimensionOutputTypeDef,
-    },
-    total=False,
-)
-
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4917,19 +4728,27 @@
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelOutputTypeDef,
+        "TagsModel": TagsModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
+
 _RequiredMessageResponseTypeDef = TypedDict(
     "_RequiredMessageResponseTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalMessageResponseTypeDef = TypedDict(
@@ -4958,26 +4777,14 @@
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OpenHoursOutputTypeDef = TypedDict(
-    "OpenHoursOutputTypeDef",
-    {
-        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-    },
-    total=False,
-)
-
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "SMS": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "PUSH": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "VOICE": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4990,22 +4797,14 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
-RandomSplitActivityOutputTypeDef = TypedDict(
-    "RandomSplitActivityOutputTypeDef",
-    {
-        "Branches": List[RandomSplitEntryTypeDef],
-    },
-    total=False,
-)
-
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
@@ -5057,23 +4856,14 @@
         "HtmlPart": SimpleEmailPartTypeDef,
         "Subject": SimpleEmailPartTypeDef,
         "TextPart": SimpleEmailPartTypeDef,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
-    },
-)
-
-TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
@@ -5082,14 +4872,15 @@
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
+        "InAppTemplate": TemplateTypeDef,
     },
     total=False,
 )
 
 _RequiredTemplatesResponseTypeDef = TypedDict(
     "_RequiredTemplatesResponseTypeDef",
     {
@@ -5178,36 +4969,50 @@
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationSettingsResponseTypeDef = TypedDict(
-    "GetApplicationSettingsResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-UpdateApplicationSettingsResponseTypeDef = TypedDict(
-    "UpdateApplicationSettingsResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
+
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5274,22 +5079,14 @@
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
 
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
-    {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5305,36 +5102,19 @@
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignEventFilterOutputTypeDef = TypedDict(
-    "CampaignEventFilterOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
-    },
-)
-
-EventConditionOutputTypeDef = TypedDict(
-    "EventConditionOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "MessageActivity": str,
-    },
-    total=False,
-)
-
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
     {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -5408,23 +5188,14 @@
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentLocationOutputTypeDef = TypedDict(
-    "SegmentLocationOutputTypeDef",
-    {
-        "Country": SetDimensionOutputTypeDef,
-        "GPSPoint": GPSPointDimensionTypeDef,
-    },
-    total=False,
-)
-
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
         "GPSPoint": GPSPointDimensionTypeDef,
     },
     total=False,
@@ -5537,14 +5308,38 @@
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetApplicationSettingsResponseTypeDef = TypedDict(
+    "GetApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsResponseTypeDef = TypedDict(
+    "UpdateApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+    },
+)
+
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointBatchRequest": EndpointBatchRequestTypeDef,
     },
 )
@@ -5565,49 +5360,16 @@
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
-        "EventFilter": CampaignEventFilterOutputTypeDef,
-        "QuietTime": QuietTimeTypeDef,
-    },
-    total=False,
-)
-
-_RequiredScheduleOutputTypeDef = TypedDict(
-    "_RequiredScheduleOutputTypeDef",
-    {
-        "StartTime": str,
-    },
-)
-_OptionalScheduleOutputTypeDef = TypedDict(
-    "_OptionalScheduleOutputTypeDef",
-    {
-        "EndTime": str,
-        "EventFilter": CampaignEventFilterOutputTypeDef,
-        "Frequency": FrequencyType,
-        "IsLocalTime": bool,
+        "EventFilter": CampaignEventFilterTypeDef,
         "QuietTime": QuietTimeTypeDef,
-        "Timezone": str,
-    },
-    total=False,
-)
-
-
-class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
-    pass
-
-
-EventStartConditionOutputTypeDef = TypedDict(
-    "EventStartConditionOutputTypeDef",
-    {
-        "EventFilter": EventFilterOutputTypeDef,
-        "SegmentId": str,
     },
     total=False,
 )
 
 _RequiredScheduleTypeDef = TypedDict(
     "_RequiredScheduleTypeDef",
     {
@@ -5668,27 +5430,14 @@
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentDimensionsOutputTypeDef = TypedDict(
-    "SegmentDimensionsOutputTypeDef",
-    {
-        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "Behavior": SegmentBehaviorsTypeDef,
-        "Demographic": SegmentDemographicsOutputTypeDef,
-        "Location": SegmentLocationOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionTypeDef],
-        "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
-    },
-    total=False,
-)
-
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "Behavior": SegmentBehaviorsTypeDef,
         "Demographic": SegmentDemographicsTypeDef,
         "Location": SegmentLocationTypeDef,
@@ -5710,25 +5459,14 @@
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignInAppMessageOutputTypeDef = TypedDict(
-    "CampaignInAppMessageOutputTypeDef",
-    {
-        "Body": str,
-        "Content": List[InAppMessageContentTypeDef],
-        "CustomConfig": Dict[str, str],
-        "Layout": LayoutType,
-    },
-    total=False,
-)
-
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
         "Content": Sequence[InAppMessageContentTypeDef],
         "CustomConfig": Mapping[str, str],
         "Layout": LayoutType,
@@ -5877,24 +5615,14 @@
         "GCMMessage": GCMMessageTypeDef,
         "SMSMessage": SMSMessageTypeDef,
         "VoiceMessage": VoiceMessageTypeDef,
     },
     total=False,
 )
 
-StartConditionOutputTypeDef = TypedDict(
-    "StartConditionOutputTypeDef",
-    {
-        "Description": str,
-        "EventStartCondition": EventStartConditionOutputTypeDef,
-        "SegmentStartCondition": SegmentConditionTypeDef,
-    },
-    total=False,
-)
-
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionTypeDef,
         "SegmentStartCondition": SegmentConditionTypeDef,
     },
@@ -5905,35 +5633,14 @@
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
 
-SegmentGroupOutputTypeDef = TypedDict(
-    "SegmentGroupOutputTypeDef",
-    {
-        "Dimensions": List[SegmentDimensionsOutputTypeDef],
-        "SourceSegments": List[SegmentReferenceTypeDef],
-        "SourceType": SourceTypeType,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-SimpleConditionOutputTypeDef = TypedDict(
-    "SimpleConditionOutputTypeDef",
-    {
-        "EventCondition": EventConditionOutputTypeDef,
-        "SegmentCondition": SegmentConditionTypeDef,
-        "SegmentDimensions": SegmentDimensionsOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": Sequence[SegmentDimensionsTypeDef],
         "SourceSegments": Sequence[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
@@ -5947,30 +5654,14 @@
         "EventCondition": EventConditionTypeDef,
         "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsTypeDef,
     },
     total=False,
 )
 
-MessageConfigurationOutputTypeDef = TypedDict(
-    "MessageConfigurationOutputTypeDef",
-    {
-        "ADMMessage": MessageTypeDef,
-        "APNSMessage": MessageTypeDef,
-        "BaiduMessage": MessageTypeDef,
-        "CustomMessage": CampaignCustomMessageTypeDef,
-        "DefaultMessage": MessageTypeDef,
-        "EmailMessage": CampaignEmailMessageTypeDef,
-        "GCMMessage": MessageTypeDef,
-        "SMSMessage": CampaignSmsMessageTypeDef,
-        "InAppMessage": CampaignInAppMessageOutputTypeDef,
-    },
-    total=False,
-)
-
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": MessageTypeDef,
         "APNSMessage": MessageTypeDef,
         "BaiduMessage": MessageTypeDef,
         "CustomMessage": CampaignCustomMessageTypeDef,
@@ -6105,41 +5796,14 @@
 
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
 
-SegmentGroupListOutputTypeDef = TypedDict(
-    "SegmentGroupListOutputTypeDef",
-    {
-        "Groups": List[SegmentGroupOutputTypeDef],
-        "Include": IncludeType,
-    },
-    total=False,
-)
-
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Conditions": List[SimpleConditionOutputTypeDef],
-        "Operator": OperatorType,
-    },
-    total=False,
-)
-
-MultiConditionalBranchOutputTypeDef = TypedDict(
-    "MultiConditionalBranchOutputTypeDef",
-    {
-        "Condition": SimpleConditionOutputTypeDef,
-        "NextActivity": str,
-    },
-    total=False,
-)
-
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -6169,17 +5833,17 @@
         "Id": str,
         "SizePercent": int,
     },
 )
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
-        "MessageConfiguration": MessageConfigurationOutputTypeDef,
-        "Schedule": ScheduleOutputTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
+        "MessageConfiguration": MessageConfigurationTypeDef,
+        "Schedule": ScheduleTypeDef,
         "State": CampaignStateTypeDef,
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
@@ -6250,51 +5914,30 @@
         "Id": str,
         "SegmentType": SegmentTypeType,
     },
 )
 _OptionalSegmentResponseTypeDef = TypedDict(
     "_OptionalSegmentResponseTypeDef",
     {
-        "Dimensions": SegmentDimensionsOutputTypeDef,
+        "Dimensions": SegmentDimensionsTypeDef,
         "ImportDefinition": SegmentImportResourceTypeDef,
         "LastModifiedDate": str,
         "Name": str,
-        "SegmentGroups": SegmentGroupListOutputTypeDef,
+        "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
 
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
 
-ConditionalSplitActivityOutputTypeDef = TypedDict(
-    "ConditionalSplitActivityOutputTypeDef",
-    {
-        "Condition": ConditionOutputTypeDef,
-        "EvaluationWaitTime": WaitTimeTypeDef,
-        "FalseActivity": str,
-        "TrueActivity": str,
-    },
-    total=False,
-)
-
-MultiConditionalSplitActivityOutputTypeDef = TypedDict(
-    "MultiConditionalSplitActivityOutputTypeDef",
-    {
-        "Branches": List[MultiConditionalBranchOutputTypeDef],
-        "DefaultActivity": str,
-        "EvaluationWaitTime": WaitTimeTypeDef,
-    },
-    total=False,
-)
-
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -6335,24 +5978,24 @@
         "SegmentVersion": int,
     },
 )
 _OptionalCampaignResponseTypeDef = TypedDict(
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
         "Hook": CampaignHookTypeDef,
         "IsPaused": bool,
         "Limits": CampaignLimitsTypeDef,
-        "MessageConfiguration": MessageConfigurationOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationTypeDef,
         "Name": str,
-        "Schedule": ScheduleOutputTypeDef,
+        "Schedule": ScheduleTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
@@ -6452,32 +6095,14 @@
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActivityOutputTypeDef = TypedDict(
-    "ActivityOutputTypeDef",
-    {
-        "CUSTOM": CustomMessageActivityOutputTypeDef,
-        "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
-        "Description": str,
-        "EMAIL": EmailMessageActivityTypeDef,
-        "Holdout": HoldoutActivityTypeDef,
-        "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
-        "PUSH": PushMessageActivityTypeDef,
-        "RandomSplit": RandomSplitActivityOutputTypeDef,
-        "SMS": SMSMessageActivityTypeDef,
-        "Wait": WaitActivityTypeDef,
-        "ContactCenter": ContactCenterActivityTypeDef,
-    },
-    total=False,
-)
-
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
     },
 )
@@ -6610,32 +6235,32 @@
         "Id": str,
         "Name": str,
     },
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
-        "Activities": Dict[str, ActivityOutputTypeDef],
+        "Activities": Dict[str, ActivityTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
         "Limits": JourneyLimitsTypeDef,
         "LocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "RefreshFrequency": str,
-        "Schedule": JourneyScheduleOutputTypeDef,
+        "Schedule": JourneyScheduleTypeDef,
         "StartActivity": str,
-        "StartCondition": StartConditionOutputTypeDef,
+        "StartCondition": StartConditionTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
-        "OpenHours": OpenHoursOutputTypeDef,
-        "ClosedDays": ClosedDaysOutputTypeDef,
+        "OpenHours": OpenHoursTypeDef,
+        "ClosedDays": ClosedDaysTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
 
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
```

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint/type_defs.pyi` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,28 @@
     "APNSVoipSandboxChannelResponseTypeDef",
     "ActivityResponseTypeDef",
     "ContactCenterActivityTypeDef",
     "HoldoutActivityTypeDef",
     "AddressConfigurationTypeDef",
     "AndroidPushNotificationTemplateTypeDef",
     "ApplicationResponseTypeDef",
+    "JourneyTimeframeCapTypeDef",
     "CampaignHookTypeDef",
     "CampaignLimitsTypeDef",
     "QuietTimeTypeDef",
-    "AttributeDimensionOutputTypeDef",
     "AttributeDimensionTypeDef",
     "AttributesResourceTypeDef",
     "BaiduChannelRequestTypeDef",
     "BaiduChannelResponseTypeDef",
     "BaiduMessageTypeDef",
     "BlobTypeDef",
     "CampaignCustomMessageTypeDef",
     "CampaignEmailMessageTypeDef",
     "CampaignStateTypeDef",
-    "CustomDeliveryConfigurationOutputTypeDef",
+    "CustomDeliveryConfigurationTypeDef",
     "CampaignSmsMessageTypeDef",
     "ChannelResponseTypeDef",
     "ClosedDaysRuleTypeDef",
     "WaitTimeTypeDef",
     "CreateApplicationRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailTemplateRequestTypeDef",
@@ -98,15 +98,14 @@
     "ExportJobRequestTypeDef",
     "ImportJobRequestTypeDef",
     "TemplateCreateMessageBodyTypeDef",
     "CreateRecommenderConfigurationTypeDef",
     "RecommenderConfigurationResponseTypeDef",
     "SMSTemplateRequestTypeDef",
     "VoiceTemplateRequestTypeDef",
-    "CustomDeliveryConfigurationTypeDef",
     "JourneyCustomMessageTypeDef",
     "DefaultButtonConfigurationTypeDef",
     "DefaultMessageTypeDef",
     "DefaultPushNotificationMessageTypeDef",
     "DefaultPushNotificationTemplateTypeDef",
     "DeleteAdmChannelRequestRequestTypeDef",
     "DeleteApnsChannelRequestRequestTypeDef",
@@ -144,18 +143,16 @@
     "JourneyEmailMessageTypeDef",
     "EmailTemplateResponseTypeDef",
     "EndpointDemographicTypeDef",
     "EndpointLocationTypeDef",
     "EndpointUserTypeDef",
     "EndpointItemResponseTypeDef",
     "EndpointMessageResultTypeDef",
-    "EndpointUserOutputTypeDef",
     "EndpointSendConfigurationTypeDef",
     "MetricDimensionTypeDef",
-    "SetDimensionOutputTypeDef",
     "SetDimensionTypeDef",
     "EventItemResponseTypeDef",
     "SessionTypeDef",
     "ExportJobResourceTypeDef",
     "GCMChannelRequestTypeDef",
     "GPSCoordinatesTypeDef",
     "GetAdmChannelRequestRequestTypeDef",
@@ -212,23 +209,21 @@
     "GetVoiceTemplateRequestRequestTypeDef",
     "VoiceTemplateResponseTypeDef",
     "ImportJobResourceTypeDef",
     "InAppMessageBodyConfigTypeDef",
     "OverrideButtonConfigurationTypeDef",
     "InAppMessageHeaderConfigTypeDef",
     "JourneyChannelSettingsTypeDef",
-    "JourneyLimitsTypeDef",
     "JourneyPushMessageTypeDef",
-    "JourneyScheduleOutputTypeDef",
     "JourneyRunResponseTypeDef",
     "JourneySMSMessageTypeDef",
     "JourneyStateRequestTypeDef",
     "ListJourneysRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagsModelOutputTypeDef",
+    "TagsModelTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "MessageTypeDef",
     "MessageResultTypeDef",
     "NumberValidateRequestTypeDef",
     "NumberValidateResponseTypeDef",
     "OpenHoursRuleTypeDef",
@@ -239,15 +234,14 @@
     "ResultRowValueTypeDef",
     "SMSChannelRequestTypeDef",
     "SegmentConditionTypeDef",
     "SegmentReferenceTypeDef",
     "SegmentImportResourceTypeDef",
     "SendOTPMessageRequestParametersTypeDef",
     "SimpleEmailPartTypeDef",
-    "TagsModelTypeDef",
     "TemplateActiveVersionRequestTypeDef",
     "TemplateTypeDef",
     "TemplateResponseTypeDef",
     "TemplateVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRecommenderConfigurationTypeDef",
     "VoiceChannelRequestTypeDef",
@@ -256,20 +250,19 @@
     "UpdateAdmChannelRequestRequestTypeDef",
     "UpdateApnsChannelRequestRequestTypeDef",
     "UpdateApnsSandboxChannelRequestRequestTypeDef",
     "UpdateApnsVoipChannelRequestRequestTypeDef",
     "UpdateApnsVoipSandboxChannelRequestRequestTypeDef",
     "ActivitiesResponseTypeDef",
     "ApplicationsResponseTypeDef",
-    "ApplicationSettingsResourceTypeDef",
-    "WriteApplicationSettingsRequestTypeDef",
+    "ApplicationSettingsJourneyLimitsTypeDef",
+    "JourneyLimitsTypeDef",
     "UpdateBaiduChannelRequestRequestTypeDef",
     "RawEmailTypeDef",
     "ChannelsResponseTypeDef",
-    "ClosedDaysOutputTypeDef",
     "ClosedDaysTypeDef",
     "WaitActivityTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppResponseTypeDef",
     "DeleteAdmChannelResponseTypeDef",
     "DeleteApnsChannelResponseTypeDef",
     "DeleteApnsSandboxChannelResponseTypeDef",
@@ -307,15 +300,14 @@
     "GetRecommenderConfigurationResponseTypeDef",
     "ListRecommenderConfigurationsResponseTypeDef",
     "UpdateRecommenderConfigurationResponseTypeDef",
     "CreateSmsTemplateRequestRequestTypeDef",
     "UpdateSmsTemplateRequestRequestTypeDef",
     "CreateVoiceTemplateRequestRequestTypeDef",
     "UpdateVoiceTemplateRequestRequestTypeDef",
-    "CustomMessageActivityOutputTypeDef",
     "CustomMessageActivityTypeDef",
     "PushNotificationTemplateRequestTypeDef",
     "PushNotificationTemplateResponseTypeDef",
     "DeleteEmailChannelResponseTypeDef",
     "GetEmailChannelResponseTypeDef",
     "UpdateEmailChannelResponseTypeDef",
     "DeleteEmailTemplateResponseTypeDef",
@@ -344,19 +336,17 @@
     "GetVoiceChannelResponseTypeDef",
     "UpdateVoiceChannelResponseTypeDef",
     "UpdateEmailChannelRequestRequestTypeDef",
     "EmailMessageActivityTypeDef",
     "GetEmailTemplateResponseTypeDef",
     "EndpointBatchItemTypeDef",
     "EndpointRequestTypeDef",
+    "EndpointResponseTypeDef",
     "PublicEndpointTypeDef",
     "SendUsersMessageResponseTypeDef",
-    "EndpointResponseTypeDef",
-    "EventDimensionsOutputTypeDef",
-    "SegmentDemographicsOutputTypeDef",
     "EventDimensionsTypeDef",
     "SegmentDemographicsTypeDef",
     "ItemResponseTypeDef",
     "EventTypeDef",
     "ExportJobResponseTypeDef",
     "UpdateGcmChannelRequestRequestTypeDef",
     "GPSPointDimensionTypeDef",
@@ -373,148 +363,129 @@
     "ImportJobResponseTypeDef",
     "InAppMessageButtonTypeDef",
     "PushMessageActivityTypeDef",
     "JourneyRunsResponseTypeDef",
     "SMSMessageActivityTypeDef",
     "UpdateJourneyStateRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "MessageResponseTypeDef",
     "PhoneNumberValidateRequestRequestTypeDef",
     "PhoneNumberValidateResponseTypeDef",
-    "OpenHoursOutputTypeDef",
     "OpenHoursTypeDef",
     "PutEventStreamRequestRequestTypeDef",
-    "RandomSplitActivityOutputTypeDef",
     "RandomSplitActivityTypeDef",
     "SegmentBehaviorsTypeDef",
     "RemoveAttributesRequestRequestTypeDef",
     "ResultRowTypeDef",
     "UpdateSmsChannelRequestRequestTypeDef",
     "SendOTPMessageRequestRequestTypeDef",
     "SimpleEmailTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TagsModelUnionTypeDef",
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     "TemplateConfigurationTypeDef",
     "TemplatesResponseTypeDef",
     "TemplateVersionsResponseTypeDef",
     "UpdateRecommenderConfigurationRequestRequestTypeDef",
     "UpdateVoiceChannelRequestRequestTypeDef",
     "VerifyOTPMessageResponseTypeDef",
     "VerifyOTPMessageRequestRequestTypeDef",
     "GetCampaignActivitiesResponseTypeDef",
     "GetAppsResponseTypeDef",
-    "GetApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsResponseTypeDef",
-    "UpdateApplicationSettingsRequestRequestTypeDef",
+    "ApplicationSettingsResourceTypeDef",
+    "WriteApplicationSettingsRequestTypeDef",
     "GetChannelsResponseTypeDef",
     "GetRecommenderConfigurationsResponseTypeDef",
     "CreatePushTemplateRequestRequestTypeDef",
     "UpdatePushTemplateRequestRequestTypeDef",
     "GetPushTemplateResponseTypeDef",
     "EndpointBatchRequestTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
-    "SendUsersMessagesResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "EndpointsResponseTypeDef",
     "GetEndpointResponseTypeDef",
-    "CampaignEventFilterOutputTypeDef",
-    "EventConditionOutputTypeDef",
-    "EventFilterOutputTypeDef",
+    "SendUsersMessagesResponseTypeDef",
     "CampaignEventFilterTypeDef",
     "EventConditionTypeDef",
     "EventFilterTypeDef",
     "EventsResponseTypeDef",
     "EventsBatchTypeDef",
     "CreateExportJobResponseTypeDef",
     "ExportJobsResponseTypeDef",
     "GetExportJobResponseTypeDef",
-    "SegmentLocationOutputTypeDef",
     "SegmentLocationTypeDef",
     "CreateImportJobResponseTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobsResponseTypeDef",
     "InAppMessageContentTypeDef",
     "GetJourneyRunsResponseTypeDef",
     "SendMessagesResponseTypeDef",
     "SendOTPMessageResponseTypeDef",
     "BaseKpiResultTypeDef",
     "EmailMessageTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
+    "GetApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsResponseTypeDef",
+    "UpdateApplicationSettingsRequestRequestTypeDef",
     "UpdateEndpointsBatchRequestRequestTypeDef",
     "DeleteUserEndpointsResponseTypeDef",
     "GetUserEndpointsResponseTypeDef",
     "InAppCampaignScheduleTypeDef",
-    "ScheduleOutputTypeDef",
-    "EventStartConditionOutputTypeDef",
     "ScheduleTypeDef",
     "EventStartConditionTypeDef",
     "PutEventsResponseTypeDef",
     "EventsRequestTypeDef",
     "GetExportJobsResponseTypeDef",
     "GetSegmentExportJobsResponseTypeDef",
-    "SegmentDimensionsOutputTypeDef",
     "SegmentDimensionsTypeDef",
     "GetImportJobsResponseTypeDef",
     "GetSegmentImportJobsResponseTypeDef",
-    "CampaignInAppMessageOutputTypeDef",
     "CampaignInAppMessageTypeDef",
     "InAppMessageTypeDef",
     "InAppTemplateRequestTypeDef",
     "InAppTemplateResponseTypeDef",
     "ApplicationDateRangeKpiResponseTypeDef",
     "CampaignDateRangeKpiResponseTypeDef",
     "JourneyDateRangeKpiResponseTypeDef",
     "DirectMessageConfigurationTypeDef",
-    "StartConditionOutputTypeDef",
     "StartConditionTypeDef",
     "PutEventsRequestRequestTypeDef",
-    "SegmentGroupOutputTypeDef",
-    "SimpleConditionOutputTypeDef",
     "SegmentGroupTypeDef",
     "SimpleConditionTypeDef",
-    "MessageConfigurationOutputTypeDef",
     "MessageConfigurationTypeDef",
     "InAppMessageCampaignTypeDef",
     "CreateInAppTemplateRequestRequestTypeDef",
     "UpdateInAppTemplateRequestRequestTypeDef",
     "GetInAppTemplateResponseTypeDef",
     "GetApplicationDateRangeKpiResponseTypeDef",
     "GetCampaignDateRangeKpiResponseTypeDef",
     "GetJourneyDateRangeKpiResponseTypeDef",
     "MessageRequestTypeDef",
     "SendUsersMessageRequestTypeDef",
-    "SegmentGroupListOutputTypeDef",
-    "ConditionOutputTypeDef",
-    "MultiConditionalBranchOutputTypeDef",
     "SegmentGroupListTypeDef",
     "ConditionTypeDef",
     "MultiConditionalBranchTypeDef",
     "TreatmentResourceTypeDef",
     "WriteTreatmentResourceTypeDef",
     "InAppMessagesResponseTypeDef",
     "SendMessagesRequestRequestTypeDef",
     "SendUsersMessagesRequestRequestTypeDef",
     "SegmentResponseTypeDef",
-    "ConditionalSplitActivityOutputTypeDef",
-    "MultiConditionalSplitActivityOutputTypeDef",
     "WriteSegmentRequestTypeDef",
     "ConditionalSplitActivityTypeDef",
     "MultiConditionalSplitActivityTypeDef",
     "CampaignResponseTypeDef",
     "WriteCampaignRequestTypeDef",
     "GetInAppMessagesResponseTypeDef",
     "CreateSegmentResponseTypeDef",
     "DeleteSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "GetSegmentVersionResponseTypeDef",
     "SegmentsResponseTypeDef",
     "UpdateSegmentResponseTypeDef",
-    "ActivityOutputTypeDef",
     "CreateSegmentRequestRequestTypeDef",
     "UpdateSegmentRequestRequestTypeDef",
     "ActivityTypeDef",
     "CampaignsResponseTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignResponseTypeDef",
     "GetCampaignResponseTypeDef",
@@ -925,14 +896,23 @@
 )
 
 class ApplicationResponseTypeDef(
     _RequiredApplicationResponseTypeDef, _OptionalApplicationResponseTypeDef
 ):
     pass
 
+JourneyTimeframeCapTypeDef = TypedDict(
+    "JourneyTimeframeCapTypeDef",
+    {
+        "Cap": int,
+        "Days": int,
+    },
+    total=False,
+)
+
 CampaignHookTypeDef = TypedDict(
     "CampaignHookTypeDef",
     {
         "LambdaFunctionName": str,
         "Mode": ModeType,
         "WebUrl": str,
     },
@@ -956,33 +936,14 @@
     {
         "End": str,
         "Start": str,
     },
     total=False,
 )
 
-_RequiredAttributeDimensionOutputTypeDef = TypedDict(
-    "_RequiredAttributeDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-_OptionalAttributeDimensionOutputTypeDef = TypedDict(
-    "_OptionalAttributeDimensionOutputTypeDef",
-    {
-        "AttributeType": AttributeTypeType,
-    },
-    total=False,
-)
-
-class AttributeDimensionOutputTypeDef(
-    _RequiredAttributeDimensionOutputTypeDef, _OptionalAttributeDimensionOutputTypeDef
-):
-    pass
-
 _RequiredAttributeDimensionTypeDef = TypedDict(
     "_RequiredAttributeDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalAttributeDimensionTypeDef = TypedDict(
@@ -1111,31 +1072,30 @@
     "CampaignStateTypeDef",
     {
         "CampaignStatus": CampaignStatusType,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationOutputTypeDef",
+_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_RequiredCustomDeliveryConfigurationTypeDef",
     {
         "DeliveryUri": str,
     },
 )
-_OptionalCustomDeliveryConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationOutputTypeDef",
+_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
+    "_OptionalCustomDeliveryConfigurationTypeDef",
     {
-        "EndpointTypes": List[EndpointTypesElementType],
+        "EndpointTypes": Sequence[EndpointTypesElementType],
     },
     total=False,
 )
 
-class CustomDeliveryConfigurationOutputTypeDef(
-    _RequiredCustomDeliveryConfigurationOutputTypeDef,
-    _OptionalCustomDeliveryConfigurationOutputTypeDef,
+class CustomDeliveryConfigurationTypeDef(
+    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
 ):
     pass
 
 CampaignSmsMessageTypeDef = TypedDict(
     "CampaignSmsMessageTypeDef",
     {
         "Body": str,
@@ -1366,33 +1326,14 @@
         "tags": Mapping[str, str],
         "TemplateDescription": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-_RequiredCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_RequiredCustomDeliveryConfigurationTypeDef",
-    {
-        "DeliveryUri": str,
-    },
-)
-_OptionalCustomDeliveryConfigurationTypeDef = TypedDict(
-    "_OptionalCustomDeliveryConfigurationTypeDef",
-    {
-        "EndpointTypes": Sequence[EndpointTypesElementType],
-    },
-    total=False,
-)
-
-class CustomDeliveryConfigurationTypeDef(
-    _RequiredCustomDeliveryConfigurationTypeDef, _OptionalCustomDeliveryConfigurationTypeDef
-):
-    pass
-
 JourneyCustomMessageTypeDef = TypedDict(
     "JourneyCustomMessageTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
@@ -1622,25 +1563,27 @@
         "ApplicationId": str,
     },
 )
 
 _RequiredGCMChannelResponseTypeDef = TypedDict(
     "_RequiredGCMChannelResponseTypeDef",
     {
-        "Credential": str,
         "Platform": str,
     },
 )
 _OptionalGCMChannelResponseTypeDef = TypedDict(
     "_OptionalGCMChannelResponseTypeDef",
     {
         "ApplicationId": str,
         "CreationDate": str,
+        "Credential": str,
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
         "HasCredential": bool,
+        "HasFcmServiceCredentials": bool,
         "Id": str,
         "IsArchived": bool,
         "LastModifiedBy": str,
         "LastModifiedDate": str,
         "Version": int,
     },
     total=False,
@@ -1839,14 +1782,15 @@
         "Action": ActionType,
         "Body": str,
         "CollapseKey": str,
         "Data": Mapping[str, str],
         "IconReference": str,
         "ImageIconUrl": str,
         "ImageUrl": str,
+        "PreferredAuthenticationMethod": str,
         "Priority": str,
         "RawContent": str,
         "RestrictedPackageName": str,
         "SilentPush": bool,
         "SmallImageIconUrl": str,
         "Sound": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -1972,15 +1916,15 @@
     },
     total=False,
 )
 
 EndpointUserTypeDef = TypedDict(
     "EndpointUserTypeDef",
     {
-        "UserAttributes": Mapping[str, Sequence[str]],
+        "UserAttributes": Dict[str, List[str]],
         "UserId": str,
     },
     total=False,
 )
 
 EndpointItemResponseTypeDef = TypedDict(
     "EndpointItemResponseTypeDef",
@@ -2010,23 +1954,14 @@
 )
 
 class EndpointMessageResultTypeDef(
     _RequiredEndpointMessageResultTypeDef, _OptionalEndpointMessageResultTypeDef
 ):
     pass
 
-EndpointUserOutputTypeDef = TypedDict(
-    "EndpointUserOutputTypeDef",
-    {
-        "UserAttributes": Dict[str, List[str]],
-        "UserId": str,
-    },
-    total=False,
-)
-
 EndpointSendConfigurationTypeDef = TypedDict(
     "EndpointSendConfigurationTypeDef",
     {
         "BodyOverride": str,
         "Context": Mapping[str, str],
         "RawContent": str,
         "Substitutions": Mapping[str, Sequence[str]],
@@ -2039,33 +1974,14 @@
     "MetricDimensionTypeDef",
     {
         "ComparisonOperator": str,
         "Value": float,
     },
 )
 
-_RequiredSetDimensionOutputTypeDef = TypedDict(
-    "_RequiredSetDimensionOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-_OptionalSetDimensionOutputTypeDef = TypedDict(
-    "_OptionalSetDimensionOutputTypeDef",
-    {
-        "DimensionType": DimensionTypeType,
-    },
-    total=False,
-)
-
-class SetDimensionOutputTypeDef(
-    _RequiredSetDimensionOutputTypeDef, _OptionalSetDimensionOutputTypeDef
-):
-    pass
-
 _RequiredSetDimensionTypeDef = TypedDict(
     "_RequiredSetDimensionTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 _OptionalSetDimensionTypeDef = TypedDict(
@@ -2124,33 +2040,25 @@
 )
 
 class ExportJobResourceTypeDef(
     _RequiredExportJobResourceTypeDef, _OptionalExportJobResourceTypeDef
 ):
     pass
 
-_RequiredGCMChannelRequestTypeDef = TypedDict(
-    "_RequiredGCMChannelRequestTypeDef",
+GCMChannelRequestTypeDef = TypedDict(
+    "GCMChannelRequestTypeDef",
     {
         "ApiKey": str,
-    },
-)
-_OptionalGCMChannelRequestTypeDef = TypedDict(
-    "_OptionalGCMChannelRequestTypeDef",
-    {
+        "DefaultAuthenticationMethod": str,
         "Enabled": bool,
+        "ServiceJson": str,
     },
     total=False,
 )
 
-class GCMChannelRequestTypeDef(
-    _RequiredGCMChannelRequestTypeDef, _OptionalGCMChannelRequestTypeDef
-):
-    pass
-
 GPSCoordinatesTypeDef = TypedDict(
     "GPSCoordinatesTypeDef",
     {
         "Latitude": float,
         "Longitude": float,
     },
 )
@@ -2929,43 +2837,22 @@
     {
         "ConnectCampaignArn": str,
         "ConnectCampaignExecutionRoleArn": str,
     },
     total=False,
 )
 
-JourneyLimitsTypeDef = TypedDict(
-    "JourneyLimitsTypeDef",
-    {
-        "DailyCap": int,
-        "EndpointReentryCap": int,
-        "MessagesPerSecond": int,
-        "EndpointReentryInterval": str,
-    },
-    total=False,
-)
-
 JourneyPushMessageTypeDef = TypedDict(
     "JourneyPushMessageTypeDef",
     {
         "TimeToLive": str,
     },
     total=False,
 )
 
-JourneyScheduleOutputTypeDef = TypedDict(
-    "JourneyScheduleOutputTypeDef",
-    {
-        "EndTime": datetime,
-        "StartTime": datetime,
-        "Timezone": str,
-    },
-    total=False,
-)
-
 JourneyRunResponseTypeDef = TypedDict(
     "JourneyRunResponseTypeDef",
     {
         "CreationTime": str,
         "LastUpdateTime": str,
         "RunId": str,
         "Status": JourneyRunStatusType,
@@ -3015,16 +2902,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagsModelOutputTypeDef = TypedDict(
-    "TagsModelOutputTypeDef",
+TagsModelTypeDef = TypedDict(
+    "TagsModelTypeDef",
     {
         "tags": Dict[str, str],
     },
 )
 
 _RequiredListTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateVersionsRequestRequestTypeDef",
@@ -3269,21 +3156,14 @@
     {
         "Charset": str,
         "Data": str,
     },
     total=False,
 )
 
-TagsModelTypeDef = TypedDict(
-    "TagsModelTypeDef",
-    {
-        "tags": Mapping[str, str],
-    },
-)
-
 TemplateActiveVersionRequestTypeDef = TypedDict(
     "TemplateActiveVersionRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
@@ -3468,44 +3348,33 @@
     {
         "Item": List[ApplicationResponseTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredApplicationSettingsResourceTypeDef = TypedDict(
-    "_RequiredApplicationSettingsResourceTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalApplicationSettingsResourceTypeDef = TypedDict(
-    "_OptionalApplicationSettingsResourceTypeDef",
+ApplicationSettingsJourneyLimitsTypeDef = TypedDict(
+    "ApplicationSettingsJourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "LastModifiedDate": str,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "DailyCap": int,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
-class ApplicationSettingsResourceTypeDef(
-    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
-):
-    pass
-
-WriteApplicationSettingsRequestTypeDef = TypedDict(
-    "WriteApplicationSettingsRequestTypeDef",
+JourneyLimitsTypeDef = TypedDict(
+    "JourneyLimitsTypeDef",
     {
-        "CampaignHook": CampaignHookTypeDef,
-        "CloudWatchMetricsEnabled": bool,
-        "EventTaggingEnabled": bool,
-        "Limits": CampaignLimitsTypeDef,
-        "QuietTime": QuietTimeTypeDef,
+        "DailyCap": int,
+        "EndpointReentryCap": int,
+        "MessagesPerSecond": int,
+        "EndpointReentryInterval": str,
+        "TimeframeCap": JourneyTimeframeCapTypeDef,
+        "TotalCap": int,
     },
     total=False,
 )
 
 UpdateBaiduChannelRequestRequestTypeDef = TypedDict(
     "UpdateBaiduChannelRequestRequestTypeDef",
     {
@@ -3525,26 +3394,14 @@
 ChannelsResponseTypeDef = TypedDict(
     "ChannelsResponseTypeDef",
     {
         "Channels": Dict[str, ChannelResponseTypeDef],
     },
 )
 
-ClosedDaysOutputTypeDef = TypedDict(
-    "ClosedDaysOutputTypeDef",
-    {
-        "EMAIL": List[ClosedDaysRuleTypeDef],
-        "SMS": List[ClosedDaysRuleTypeDef],
-        "PUSH": List[ClosedDaysRuleTypeDef],
-        "VOICE": List[ClosedDaysRuleTypeDef],
-        "CUSTOM": List[ClosedDaysRuleTypeDef],
-    },
-    total=False,
-)
-
 ClosedDaysTypeDef = TypedDict(
     "ClosedDaysTypeDef",
     {
         "EMAIL": Sequence[ClosedDaysRuleTypeDef],
         "SMS": Sequence[ClosedDaysRuleTypeDef],
         "PUSH": Sequence[ClosedDaysRuleTypeDef],
         "VOICE": Sequence[ClosedDaysRuleTypeDef],
@@ -3952,27 +3809,14 @@
 
 class UpdateVoiceTemplateRequestRequestTypeDef(
     _RequiredUpdateVoiceTemplateRequestRequestTypeDef,
     _OptionalUpdateVoiceTemplateRequestRequestTypeDef,
 ):
     pass
 
-CustomMessageActivityOutputTypeDef = TypedDict(
-    "CustomMessageActivityOutputTypeDef",
-    {
-        "DeliveryUri": str,
-        "EndpointTypes": List[EndpointTypesElementType],
-        "MessageConfig": JourneyCustomMessageTypeDef,
-        "NextActivity": str,
-        "TemplateName": str,
-        "TemplateVersion": str,
-    },
-    total=False,
-)
-
 CustomMessageActivityTypeDef = TypedDict(
     "CustomMessageActivityTypeDef",
     {
         "DeliveryUri": str,
         "EndpointTypes": Sequence[EndpointTypesElementType],
         "MessageConfig": JourneyCustomMessageTypeDef,
         "NextActivity": str,
@@ -4315,14 +4159,36 @@
         "OptOut": str,
         "RequestId": str,
         "User": EndpointUserTypeDef,
     },
     total=False,
 )
 
+EndpointResponseTypeDef = TypedDict(
+    "EndpointResponseTypeDef",
+    {
+        "Address": str,
+        "ApplicationId": str,
+        "Attributes": Dict[str, List[str]],
+        "ChannelType": ChannelTypeType,
+        "CohortId": str,
+        "CreationDate": str,
+        "Demographic": EndpointDemographicTypeDef,
+        "EffectiveDate": str,
+        "EndpointStatus": str,
+        "Id": str,
+        "Location": EndpointLocationTypeDef,
+        "Metrics": Dict[str, float],
+        "OptOut": str,
+        "RequestId": str,
+        "User": EndpointUserTypeDef,
+    },
+    total=False,
+)
+
 PublicEndpointTypeDef = TypedDict(
     "PublicEndpointTypeDef",
     {
         "Address": str,
         "Attributes": Mapping[str, Sequence[str]],
         "ChannelType": ChannelTypeType,
         "Demographic": EndpointDemographicTypeDef,
@@ -4353,59 +4219,14 @@
 )
 
 class SendUsersMessageResponseTypeDef(
     _RequiredSendUsersMessageResponseTypeDef, _OptionalSendUsersMessageResponseTypeDef
 ):
     pass
 
-EndpointResponseTypeDef = TypedDict(
-    "EndpointResponseTypeDef",
-    {
-        "Address": str,
-        "ApplicationId": str,
-        "Attributes": Dict[str, List[str]],
-        "ChannelType": ChannelTypeType,
-        "CohortId": str,
-        "CreationDate": str,
-        "Demographic": EndpointDemographicTypeDef,
-        "EffectiveDate": str,
-        "EndpointStatus": str,
-        "Id": str,
-        "Location": EndpointLocationTypeDef,
-        "Metrics": Dict[str, float],
-        "OptOut": str,
-        "RequestId": str,
-        "User": EndpointUserOutputTypeDef,
-    },
-    total=False,
-)
-
-EventDimensionsOutputTypeDef = TypedDict(
-    "EventDimensionsOutputTypeDef",
-    {
-        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "EventType": SetDimensionOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-SegmentDemographicsOutputTypeDef = TypedDict(
-    "SegmentDemographicsOutputTypeDef",
-    {
-        "AppVersion": SetDimensionOutputTypeDef,
-        "Channel": SetDimensionOutputTypeDef,
-        "DeviceType": SetDimensionOutputTypeDef,
-        "Make": SetDimensionOutputTypeDef,
-        "Model": SetDimensionOutputTypeDef,
-        "Platform": SetDimensionOutputTypeDef,
-    },
-    total=False,
-)
-
 EventDimensionsTypeDef = TypedDict(
     "EventDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "EventType": SetDimensionTypeDef,
         "Metrics": Mapping[str, MetricDimensionTypeDef],
     },
@@ -4740,19 +4561,27 @@
         "JourneyStateRequest": JourneyStateRequestTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagsModel": TagsModelOutputTypeDef,
+        "TagsModel": TagsModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagsModel": TagsModelTypeDef,
+    },
+)
+
 _RequiredMessageResponseTypeDef = TypedDict(
     "_RequiredMessageResponseTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalMessageResponseTypeDef = TypedDict(
@@ -4779,26 +4608,14 @@
     "PhoneNumberValidateResponseTypeDef",
     {
         "NumberValidateResponse": NumberValidateResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OpenHoursOutputTypeDef = TypedDict(
-    "OpenHoursOutputTypeDef",
-    {
-        "EMAIL": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "SMS": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "PUSH": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "VOICE": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-        "CUSTOM": Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]],
-    },
-    total=False,
-)
-
 OpenHoursTypeDef = TypedDict(
     "OpenHoursTypeDef",
     {
         "EMAIL": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "SMS": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "PUSH": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
         "VOICE": Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]],
@@ -4811,22 +4628,14 @@
     "PutEventStreamRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteEventStream": WriteEventStreamTypeDef,
     },
 )
 
-RandomSplitActivityOutputTypeDef = TypedDict(
-    "RandomSplitActivityOutputTypeDef",
-    {
-        "Branches": List[RandomSplitEntryTypeDef],
-    },
-    total=False,
-)
-
 RandomSplitActivityTypeDef = TypedDict(
     "RandomSplitActivityTypeDef",
     {
         "Branches": Sequence[RandomSplitEntryTypeDef],
     },
     total=False,
 )
@@ -4878,23 +4687,14 @@
         "HtmlPart": SimpleEmailPartTypeDef,
         "Subject": SimpleEmailPartTypeDef,
         "TextPart": SimpleEmailPartTypeDef,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagsModel": TagsModelTypeDef,
-    },
-)
-
-TagsModelUnionTypeDef = Union[TagsModelTypeDef, TagsModelOutputTypeDef]
 UpdateTemplateActiveVersionRequestRequestTypeDef = TypedDict(
     "UpdateTemplateActiveVersionRequestRequestTypeDef",
     {
         "TemplateActiveVersionRequest": TemplateActiveVersionRequestTypeDef,
         "TemplateName": str,
         "TemplateType": str,
     },
@@ -4903,14 +4703,15 @@
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "EmailTemplate": TemplateTypeDef,
         "PushTemplate": TemplateTypeDef,
         "SMSTemplate": TemplateTypeDef,
         "VoiceTemplate": TemplateTypeDef,
+        "InAppTemplate": TemplateTypeDef,
     },
     total=False,
 )
 
 _RequiredTemplatesResponseTypeDef = TypedDict(
     "_RequiredTemplatesResponseTypeDef",
     {
@@ -4995,36 +4796,48 @@
     "GetAppsResponseTypeDef",
     {
         "ApplicationsResponse": ApplicationsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationSettingsResponseTypeDef = TypedDict(
-    "GetApplicationSettingsResponseTypeDef",
+_RequiredApplicationSettingsResourceTypeDef = TypedDict(
+    "_RequiredApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationId": str,
     },
 )
-
-UpdateApplicationSettingsResponseTypeDef = TypedDict(
-    "UpdateApplicationSettingsResponseTypeDef",
+_OptionalApplicationSettingsResourceTypeDef = TypedDict(
+    "_OptionalApplicationSettingsResourceTypeDef",
     {
-        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "LastModifiedDate": str,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
-UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationSettingsRequestRequestTypeDef",
+class ApplicationSettingsResourceTypeDef(
+    _RequiredApplicationSettingsResourceTypeDef, _OptionalApplicationSettingsResourceTypeDef
+):
+    pass
+
+WriteApplicationSettingsRequestTypeDef = TypedDict(
+    "WriteApplicationSettingsRequestTypeDef",
     {
-        "ApplicationId": str,
-        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+        "CampaignHook": CampaignHookTypeDef,
+        "CloudWatchMetricsEnabled": bool,
+        "EventTaggingEnabled": bool,
+        "Limits": CampaignLimitsTypeDef,
+        "QuietTime": QuietTimeTypeDef,
+        "JourneyLimits": ApplicationSettingsJourneyLimitsTypeDef,
     },
+    total=False,
 )
 
 GetChannelsResponseTypeDef = TypedDict(
     "GetChannelsResponseTypeDef",
     {
         "ChannelsResponse": ChannelsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5089,22 +4902,14 @@
     {
         "ApplicationId": str,
         "EndpointId": str,
         "EndpointRequest": EndpointRequestTypeDef,
     },
 )
 
-SendUsersMessagesResponseTypeDef = TypedDict(
-    "SendUsersMessagesResponseTypeDef",
-    {
-        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5120,36 +4925,19 @@
     "GetEndpointResponseTypeDef",
     {
         "EndpointResponse": EndpointResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignEventFilterOutputTypeDef = TypedDict(
-    "CampaignEventFilterOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
-    },
-)
-
-EventConditionOutputTypeDef = TypedDict(
-    "EventConditionOutputTypeDef",
-    {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "MessageActivity": str,
-    },
-    total=False,
-)
-
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
+SendUsersMessagesResponseTypeDef = TypedDict(
+    "SendUsersMessagesResponseTypeDef",
     {
-        "Dimensions": EventDimensionsOutputTypeDef,
-        "FilterType": FilterTypeType,
+        "SendUsersMessageResponse": SendUsersMessageResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CampaignEventFilterTypeDef = TypedDict(
     "CampaignEventFilterTypeDef",
     {
         "Dimensions": EventDimensionsTypeDef,
@@ -5221,23 +5009,14 @@
     "GetExportJobResponseTypeDef",
     {
         "ExportJobResponse": ExportJobResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentLocationOutputTypeDef = TypedDict(
-    "SegmentLocationOutputTypeDef",
-    {
-        "Country": SetDimensionOutputTypeDef,
-        "GPSPoint": GPSPointDimensionTypeDef,
-    },
-    total=False,
-)
-
 SegmentLocationTypeDef = TypedDict(
     "SegmentLocationTypeDef",
     {
         "Country": SetDimensionTypeDef,
         "GPSPoint": GPSPointDimensionTypeDef,
     },
     total=False,
@@ -5348,14 +5127,38 @@
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionsResponse": TemplateVersionsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetApplicationSettingsResponseTypeDef = TypedDict(
+    "GetApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsResponseTypeDef = TypedDict(
+    "UpdateApplicationSettingsResponseTypeDef",
+    {
+        "ApplicationSettingsResource": ApplicationSettingsResourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationSettingsRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "WriteApplicationSettingsRequest": WriteApplicationSettingsRequestTypeDef,
+    },
+)
+
 UpdateEndpointsBatchRequestRequestTypeDef = TypedDict(
     "UpdateEndpointsBatchRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EndpointBatchRequest": EndpointBatchRequestTypeDef,
     },
 )
@@ -5376,47 +5179,16 @@
     },
 )
 
 InAppCampaignScheduleTypeDef = TypedDict(
     "InAppCampaignScheduleTypeDef",
     {
         "EndDate": str,
-        "EventFilter": CampaignEventFilterOutputTypeDef,
-        "QuietTime": QuietTimeTypeDef,
-    },
-    total=False,
-)
-
-_RequiredScheduleOutputTypeDef = TypedDict(
-    "_RequiredScheduleOutputTypeDef",
-    {
-        "StartTime": str,
-    },
-)
-_OptionalScheduleOutputTypeDef = TypedDict(
-    "_OptionalScheduleOutputTypeDef",
-    {
-        "EndTime": str,
-        "EventFilter": CampaignEventFilterOutputTypeDef,
-        "Frequency": FrequencyType,
-        "IsLocalTime": bool,
+        "EventFilter": CampaignEventFilterTypeDef,
         "QuietTime": QuietTimeTypeDef,
-        "Timezone": str,
-    },
-    total=False,
-)
-
-class ScheduleOutputTypeDef(_RequiredScheduleOutputTypeDef, _OptionalScheduleOutputTypeDef):
-    pass
-
-EventStartConditionOutputTypeDef = TypedDict(
-    "EventStartConditionOutputTypeDef",
-    {
-        "EventFilter": EventFilterOutputTypeDef,
-        "SegmentId": str,
     },
     total=False,
 )
 
 _RequiredScheduleTypeDef = TypedDict(
     "_RequiredScheduleTypeDef",
     {
@@ -5475,27 +5247,14 @@
     "GetSegmentExportJobsResponseTypeDef",
     {
         "ExportJobsResponse": ExportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentDimensionsOutputTypeDef = TypedDict(
-    "SegmentDimensionsOutputTypeDef",
-    {
-        "Attributes": Dict[str, AttributeDimensionOutputTypeDef],
-        "Behavior": SegmentBehaviorsTypeDef,
-        "Demographic": SegmentDemographicsOutputTypeDef,
-        "Location": SegmentLocationOutputTypeDef,
-        "Metrics": Dict[str, MetricDimensionTypeDef],
-        "UserAttributes": Dict[str, AttributeDimensionOutputTypeDef],
-    },
-    total=False,
-)
-
 SegmentDimensionsTypeDef = TypedDict(
     "SegmentDimensionsTypeDef",
     {
         "Attributes": Mapping[str, AttributeDimensionTypeDef],
         "Behavior": SegmentBehaviorsTypeDef,
         "Demographic": SegmentDemographicsTypeDef,
         "Location": SegmentLocationTypeDef,
@@ -5517,25 +5276,14 @@
     "GetSegmentImportJobsResponseTypeDef",
     {
         "ImportJobsResponse": ImportJobsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CampaignInAppMessageOutputTypeDef = TypedDict(
-    "CampaignInAppMessageOutputTypeDef",
-    {
-        "Body": str,
-        "Content": List[InAppMessageContentTypeDef],
-        "CustomConfig": Dict[str, str],
-        "Layout": LayoutType,
-    },
-    total=False,
-)
-
 CampaignInAppMessageTypeDef = TypedDict(
     "CampaignInAppMessageTypeDef",
     {
         "Body": str,
         "Content": Sequence[InAppMessageContentTypeDef],
         "CustomConfig": Mapping[str, str],
         "Layout": LayoutType,
@@ -5676,24 +5424,14 @@
         "GCMMessage": GCMMessageTypeDef,
         "SMSMessage": SMSMessageTypeDef,
         "VoiceMessage": VoiceMessageTypeDef,
     },
     total=False,
 )
 
-StartConditionOutputTypeDef = TypedDict(
-    "StartConditionOutputTypeDef",
-    {
-        "Description": str,
-        "EventStartCondition": EventStartConditionOutputTypeDef,
-        "SegmentStartCondition": SegmentConditionTypeDef,
-    },
-    total=False,
-)
-
 StartConditionTypeDef = TypedDict(
     "StartConditionTypeDef",
     {
         "Description": str,
         "EventStartCondition": EventStartConditionTypeDef,
         "SegmentStartCondition": SegmentConditionTypeDef,
     },
@@ -5704,35 +5442,14 @@
     "PutEventsRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EventsRequest": EventsRequestTypeDef,
     },
 )
 
-SegmentGroupOutputTypeDef = TypedDict(
-    "SegmentGroupOutputTypeDef",
-    {
-        "Dimensions": List[SegmentDimensionsOutputTypeDef],
-        "SourceSegments": List[SegmentReferenceTypeDef],
-        "SourceType": SourceTypeType,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-SimpleConditionOutputTypeDef = TypedDict(
-    "SimpleConditionOutputTypeDef",
-    {
-        "EventCondition": EventConditionOutputTypeDef,
-        "SegmentCondition": SegmentConditionTypeDef,
-        "SegmentDimensions": SegmentDimensionsOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentGroupTypeDef = TypedDict(
     "SegmentGroupTypeDef",
     {
         "Dimensions": Sequence[SegmentDimensionsTypeDef],
         "SourceSegments": Sequence[SegmentReferenceTypeDef],
         "SourceType": SourceTypeType,
         "Type": TypeType,
@@ -5746,30 +5463,14 @@
         "EventCondition": EventConditionTypeDef,
         "SegmentCondition": SegmentConditionTypeDef,
         "SegmentDimensions": SegmentDimensionsTypeDef,
     },
     total=False,
 )
 
-MessageConfigurationOutputTypeDef = TypedDict(
-    "MessageConfigurationOutputTypeDef",
-    {
-        "ADMMessage": MessageTypeDef,
-        "APNSMessage": MessageTypeDef,
-        "BaiduMessage": MessageTypeDef,
-        "CustomMessage": CampaignCustomMessageTypeDef,
-        "DefaultMessage": MessageTypeDef,
-        "EmailMessage": CampaignEmailMessageTypeDef,
-        "GCMMessage": MessageTypeDef,
-        "SMSMessage": CampaignSmsMessageTypeDef,
-        "InAppMessage": CampaignInAppMessageOutputTypeDef,
-    },
-    total=False,
-)
-
 MessageConfigurationTypeDef = TypedDict(
     "MessageConfigurationTypeDef",
     {
         "ADMMessage": MessageTypeDef,
         "APNSMessage": MessageTypeDef,
         "BaiduMessage": MessageTypeDef,
         "CustomMessage": CampaignCustomMessageTypeDef,
@@ -5898,41 +5599,14 @@
 )
 
 class SendUsersMessageRequestTypeDef(
     _RequiredSendUsersMessageRequestTypeDef, _OptionalSendUsersMessageRequestTypeDef
 ):
     pass
 
-SegmentGroupListOutputTypeDef = TypedDict(
-    "SegmentGroupListOutputTypeDef",
-    {
-        "Groups": List[SegmentGroupOutputTypeDef],
-        "Include": IncludeType,
-    },
-    total=False,
-)
-
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Conditions": List[SimpleConditionOutputTypeDef],
-        "Operator": OperatorType,
-    },
-    total=False,
-)
-
-MultiConditionalBranchOutputTypeDef = TypedDict(
-    "MultiConditionalBranchOutputTypeDef",
-    {
-        "Condition": SimpleConditionOutputTypeDef,
-        "NextActivity": str,
-    },
-    total=False,
-)
-
 SegmentGroupListTypeDef = TypedDict(
     "SegmentGroupListTypeDef",
     {
         "Groups": Sequence[SegmentGroupTypeDef],
         "Include": IncludeType,
     },
     total=False,
@@ -5962,17 +5636,17 @@
         "Id": str,
         "SizePercent": int,
     },
 )
 _OptionalTreatmentResourceTypeDef = TypedDict(
     "_OptionalTreatmentResourceTypeDef",
     {
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
-        "MessageConfiguration": MessageConfigurationOutputTypeDef,
-        "Schedule": ScheduleOutputTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
+        "MessageConfiguration": MessageConfigurationTypeDef,
+        "Schedule": ScheduleTypeDef,
         "State": CampaignStateTypeDef,
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
     },
     total=False,
 )
@@ -6039,49 +5713,28 @@
         "Id": str,
         "SegmentType": SegmentTypeType,
     },
 )
 _OptionalSegmentResponseTypeDef = TypedDict(
     "_OptionalSegmentResponseTypeDef",
     {
-        "Dimensions": SegmentDimensionsOutputTypeDef,
+        "Dimensions": SegmentDimensionsTypeDef,
         "ImportDefinition": SegmentImportResourceTypeDef,
         "LastModifiedDate": str,
         "Name": str,
-        "SegmentGroups": SegmentGroupListOutputTypeDef,
+        "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Dict[str, str],
         "Version": int,
     },
     total=False,
 )
 
 class SegmentResponseTypeDef(_RequiredSegmentResponseTypeDef, _OptionalSegmentResponseTypeDef):
     pass
 
-ConditionalSplitActivityOutputTypeDef = TypedDict(
-    "ConditionalSplitActivityOutputTypeDef",
-    {
-        "Condition": ConditionOutputTypeDef,
-        "EvaluationWaitTime": WaitTimeTypeDef,
-        "FalseActivity": str,
-        "TrueActivity": str,
-    },
-    total=False,
-)
-
-MultiConditionalSplitActivityOutputTypeDef = TypedDict(
-    "MultiConditionalSplitActivityOutputTypeDef",
-    {
-        "Branches": List[MultiConditionalBranchOutputTypeDef],
-        "DefaultActivity": str,
-        "EvaluationWaitTime": WaitTimeTypeDef,
-    },
-    total=False,
-)
-
 WriteSegmentRequestTypeDef = TypedDict(
     "WriteSegmentRequestTypeDef",
     {
         "Dimensions": SegmentDimensionsTypeDef,
         "Name": str,
         "SegmentGroups": SegmentGroupListTypeDef,
         "tags": Mapping[str, str],
@@ -6122,24 +5775,24 @@
         "SegmentVersion": int,
     },
 )
 _OptionalCampaignResponseTypeDef = TypedDict(
     "_OptionalCampaignResponseTypeDef",
     {
         "AdditionalTreatments": List[TreatmentResourceTypeDef],
-        "CustomDeliveryConfiguration": CustomDeliveryConfigurationOutputTypeDef,
+        "CustomDeliveryConfiguration": CustomDeliveryConfigurationTypeDef,
         "DefaultState": CampaignStateTypeDef,
         "Description": str,
         "HoldoutPercent": int,
         "Hook": CampaignHookTypeDef,
         "IsPaused": bool,
         "Limits": CampaignLimitsTypeDef,
-        "MessageConfiguration": MessageConfigurationOutputTypeDef,
+        "MessageConfiguration": MessageConfigurationTypeDef,
         "Name": str,
-        "Schedule": ScheduleOutputTypeDef,
+        "Schedule": ScheduleTypeDef,
         "State": CampaignStateTypeDef,
         "tags": Dict[str, str],
         "TemplateConfiguration": TemplateConfigurationTypeDef,
         "TreatmentDescription": str,
         "TreatmentName": str,
         "Version": int,
         "Priority": int,
@@ -6235,32 +5888,14 @@
     "UpdateSegmentResponseTypeDef",
     {
         "SegmentResponse": SegmentResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActivityOutputTypeDef = TypedDict(
-    "ActivityOutputTypeDef",
-    {
-        "CUSTOM": CustomMessageActivityOutputTypeDef,
-        "ConditionalSplit": ConditionalSplitActivityOutputTypeDef,
-        "Description": str,
-        "EMAIL": EmailMessageActivityTypeDef,
-        "Holdout": HoldoutActivityTypeDef,
-        "MultiCondition": MultiConditionalSplitActivityOutputTypeDef,
-        "PUSH": PushMessageActivityTypeDef,
-        "RandomSplit": RandomSplitActivityOutputTypeDef,
-        "SMS": SMSMessageActivityTypeDef,
-        "Wait": WaitActivityTypeDef,
-        "ContactCenter": ContactCenterActivityTypeDef,
-    },
-    total=False,
-)
-
 CreateSegmentRequestRequestTypeDef = TypedDict(
     "CreateSegmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "WriteSegmentRequest": WriteSegmentRequestTypeDef,
     },
 )
@@ -6391,32 +6026,32 @@
         "Id": str,
         "Name": str,
     },
 )
 _OptionalJourneyResponseTypeDef = TypedDict(
     "_OptionalJourneyResponseTypeDef",
     {
-        "Activities": Dict[str, ActivityOutputTypeDef],
+        "Activities": Dict[str, ActivityTypeDef],
         "CreationDate": str,
         "LastModifiedDate": str,
         "Limits": JourneyLimitsTypeDef,
         "LocalTime": bool,
         "QuietTime": QuietTimeTypeDef,
         "RefreshFrequency": str,
-        "Schedule": JourneyScheduleOutputTypeDef,
+        "Schedule": JourneyScheduleTypeDef,
         "StartActivity": str,
-        "StartCondition": StartConditionOutputTypeDef,
+        "StartCondition": StartConditionTypeDef,
         "State": StateType,
         "tags": Dict[str, str],
         "WaitForQuietTime": bool,
         "RefreshOnSegmentUpdate": bool,
         "JourneyChannelSettings": JourneyChannelSettingsTypeDef,
         "SendingSchedule": bool,
-        "OpenHours": OpenHoursOutputTypeDef,
-        "ClosedDays": ClosedDaysOutputTypeDef,
+        "OpenHours": OpenHoursTypeDef,
+        "ClosedDays": ClosedDaysTypeDef,
         "TimezoneEstimationMethods": List[TimezoneEstimationMethodsElementType],
     },
     total=False,
 )
 
 class JourneyResponseTypeDef(_RequiredJourneyResponseTypeDef, _OptionalJourneyResponseTypeDef):
     pass
```

### Comparing `types-aiobotocore-pinpoint-2.5.2.post1/types_aiobotocore_pinpoint.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-2.5.2.post2/types_aiobotocore_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

