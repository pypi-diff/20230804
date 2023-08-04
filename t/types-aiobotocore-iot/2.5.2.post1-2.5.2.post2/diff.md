# Comparing `tmp/types-aiobotocore-iot-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iot-2.5.2.post1.tar` & `types-aiobotocore-iot-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.305564 types-aiobotocore-iot-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55522 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.305564 types-aiobotocore-iot-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   190224 2023-08-02 14:40:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   189906 2023-08-02 14:40:25.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24962 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    71670 2023-08-02 14:40:28.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    71609 2023-08-02 14:40:27.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   272446 2023-08-02 14:40:35.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   272098 2023-08-02 14:40:31.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:24.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.297564 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:26.000000 types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22394 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20892 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14184 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   190004 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   189686 2023-08-04 13:40:32.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25057 2023-08-04 13:40:35.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25055 2023-08-04 13:40:35.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    71670 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    71609 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   256609 2023-08-04 13:40:43.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   256282 2023-08-04 13:40:39.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22394 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-2.5.2.post1/LICENSE` & `types-aiobotocore-iot-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post1/setup.py` & `types-aiobotocore-iot-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__init__.pyi` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/__main__.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoT 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,29 +113,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigUnionTypeDef,
-    AggregationTypeUnionTypeDef,
+    AbortConfigTypeDef,
+    AggregationTypeTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadUnionTypeDef,
+    AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetUnionTypeDef,
+    AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoUnionTypeDef,
+    AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorUnionTypeDef,
+    BehaviorTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -193,15 +193,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetUnionTypeDef,
+    DetectMitigationActionsTaskTargetTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -215,15 +215,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigUnionTypeDef,
+    JobExecutionsRetryConfigTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -280,40 +280,40 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsUnionTypeDef,
+    MitigationActionParamsTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileUnionTypeDef,
+    OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigUnionTypeDef,
+    SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationUnionTypeDef,
-    ThingGroupPropertiesUnionTypeDef,
-    ThingIndexingConfigurationUnionTypeDef,
-    ThingTypePropertiesUnionTypeDef,
+    ThingGroupIndexingConfigurationTypeDef,
+    ThingGroupPropertiesTypeDef,
+    ThingIndexingConfigurationTypeDef,
+    ThingTypePropertiesTypeDef,
     TimeoutConfigTypeDef,
     TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
@@ -327,15 +327,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeUnionTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -701,15 +701,15 @@
         """
 
     async def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -718,15 +718,15 @@
         """
 
     async def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeUnionTypeDef,
+        aggregationType: AggregationTypeTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -745,22 +745,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
+        schedulingConfig: SchedulingConfigTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
@@ -772,18 +772,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -802,15 +802,15 @@
         """
 
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsUnionTypeDef,
+        actionParams: MitigationActionParamsTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
@@ -818,15 +818,15 @@
         """
 
     async def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileUnionTypeDef],
+        files: Sequence[OTAUpdateFileTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -965,15 +965,15 @@
         """
 
     async def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
+        behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -999,44 +999,44 @@
         """
 
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadUnionTypeDef = ...,
+        attributePayload: AttributePayloadTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
 
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
 
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
+        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
@@ -2893,33 +2893,33 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#set_v2_logging_options)
         """
 
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetUnionTypeDef,
+        target: AuditMitigationActionsTaskTargetTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
 
     async def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetUnionTypeDef,
+        target: DetectMitigationActionsTaskTargetTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2961,15 +2961,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#tag_resource)
         """
 
     async def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoUnionTypeDef],
+        authInfos: Sequence[AuthInfoTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -3141,15 +3141,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
 
     async def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
+        thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -3170,15 +3170,15 @@
 
     async def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeUnionTypeDef = ...,
+        aggregationType: AggregationTypeTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -3188,16 +3188,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
 
     async def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
@@ -3205,32 +3205,32 @@
     async def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
 
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsUnionTypeDef = ...
+        actionParams: MitigationActionParamsTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3327,15 +3327,15 @@
         """
 
     async def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
+        behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3363,30 +3363,30 @@
         """
 
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadUnionTypeDef = ...,
+        attributePayload: AttributePayloadTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
 
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
+        thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
@@ -3414,15 +3414,15 @@
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_topic_rule_destination)
         """
 
     async def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
+        self, *, behaviors: Sequence[BehaviorTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/client.pyi` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -113,29 +113,29 @@
     ListThingTypesPaginator,
     ListTopicRuleDestinationsPaginator,
     ListTopicRulesPaginator,
     ListV2LoggingLevelsPaginator,
     ListViolationEventsPaginator,
 )
 from .type_defs import (
-    AbortConfigUnionTypeDef,
-    AggregationTypeUnionTypeDef,
+    AbortConfigTypeDef,
+    AggregationTypeTypeDef,
     AlertTargetTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
-    AttributePayloadUnionTypeDef,
+    AttributePayloadTypeDef,
     AuditCheckConfigurationTypeDef,
-    AuditMitigationActionsTaskTargetUnionTypeDef,
+    AuditMitigationActionsTaskTargetTypeDef,
     AuditNotificationTargetTypeDef,
-    AuthInfoUnionTypeDef,
+    AuthInfoTypeDef,
     AuthorizerConfigTypeDef,
     AwsJobAbortConfigTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    BehaviorUnionTypeDef,
+    BehaviorTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketsAggregationTypeTypeDef,
     CancelJobResponseTypeDef,
     ConfigurationTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -193,15 +193,15 @@
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileResponseTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeThingGroupResponseTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
-    DetectMitigationActionsTaskTargetUnionTypeDef,
+    DetectMitigationActionsTaskTargetTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
     GetBucketsAggregationResponseTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesResponseTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     GetJobDocumentResponseTypeDef,
@@ -215,15 +215,15 @@
     GetPolicyVersionResponseTypeDef,
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     GetTopicRuleResponseTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     HttpContextTypeDef,
-    JobExecutionsRetryConfigUnionTypeDef,
+    JobExecutionsRetryConfigTypeDef,
     JobExecutionsRolloutConfigTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     ListAuditSuppressionsResponseTypeDef,
@@ -280,40 +280,40 @@
     ListTopicRulesResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
     LoggingOptionsPayloadTypeDef,
     LogTargetTypeDef,
     MaintenanceWindowTypeDef,
     MetricToRetainTypeDef,
-    MitigationActionParamsUnionTypeDef,
+    MitigationActionParamsTypeDef,
     MqttContextTypeDef,
-    OTAUpdateFileUnionTypeDef,
+    OTAUpdateFileTypeDef,
     PresignedUrlConfigTypeDef,
     ProvisioningHookTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingResponseTypeDef,
     RegistrationConfigTypeDef,
     ResourceIdentifierTypeDef,
-    SchedulingConfigUnionTypeDef,
+    SchedulingConfigTypeDef,
     SearchIndexResponseTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StreamFileTypeDef,
     TagTypeDef,
     TestAuthorizationResponseTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
-    ThingGroupIndexingConfigurationUnionTypeDef,
-    ThingGroupPropertiesUnionTypeDef,
-    ThingIndexingConfigurationUnionTypeDef,
-    ThingTypePropertiesUnionTypeDef,
+    ThingGroupIndexingConfigurationTypeDef,
+    ThingGroupPropertiesTypeDef,
+    ThingIndexingConfigurationTypeDef,
+    ThingTypePropertiesTypeDef,
     TimeoutConfigTypeDef,
     TimestampTypeDef,
     TlsConfigTypeDef,
     TlsContextTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRulePayloadTypeDef,
     TransferCertificateResponseTypeDef,
@@ -327,15 +327,15 @@
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateSecurityProfileResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     VersionUpdateByJobsConfigTypeDef,
-    ViolationEventOccurrenceRangeUnionTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -671,15 +671,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_domain_configuration)
         """
     async def create_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
         queryString: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         indexName: str = ...,
         queryVersion: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDynamicThingGroupResponseTypeDef:
         """
         Creates a dynamic thing group.
 
@@ -687,15 +687,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_dynamic_thing_group)
         """
     async def create_fleet_metric(
         self,
         *,
         metricName: str,
         queryString: str,
-        aggregationType: AggregationTypeUnionTypeDef,
+        aggregationType: AggregationTypeTypeDef,
         period: int,
         aggregationField: str,
         description: str = ...,
         queryVersion: str = ...,
         indexName: str = ...,
         unit: FleetMetricUnitType = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -713,22 +713,22 @@
         targets: Sequence[str],
         documentSource: str = ...,
         document: str = ...,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         targetSelection: TargetSelectionType = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         namespaceId: str = ...,
         jobTemplateArn: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         documentParameters: Mapping[str, str] = ...,
-        schedulingConfig: SchedulingConfigUnionTypeDef = ...,
+        schedulingConfig: SchedulingConfigTypeDef = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobResponseTypeDef:
         """
         Creates a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_job)
@@ -739,18 +739,18 @@
         jobTemplateId: str,
         description: str,
         jobArn: str = ...,
         documentSource: str = ...,
         document: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...,
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...,
         maintenanceWindows: Sequence[MaintenanceWindowTypeDef] = ...,
         destinationPackageVersions: Sequence[str] = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_job_template)
@@ -767,30 +767,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_keys_and_certificate)
         """
     async def create_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str,
-        actionParams: MitigationActionParamsUnionTypeDef,
+        actionParams: MitigationActionParamsTypeDef,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateMitigationActionResponseTypeDef:
         """
         Defines an action that can be applied to audit findings by using
         StartAuditMitigationActionsTask.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_mitigation_action)
         """
     async def create_ota_update(
         self,
         *,
         otaUpdateId: str,
         targets: Sequence[str],
-        files: Sequence[OTAUpdateFileUnionTypeDef],
+        files: Sequence[OTAUpdateFileTypeDef],
         roleArn: str,
         description: str = ...,
         protocols: Sequence[ProtocolType] = ...,
         targetSelection: TargetSelectionType = ...,
         awsJobExecutionsRolloutConfig: AwsJobExecutionsRolloutConfigTypeDef = ...,
         awsJobPresignedUrlConfig: AwsJobPresignedUrlConfigTypeDef = ...,
         awsJobAbortConfig: AwsJobAbortConfigTypeDef = ...,
@@ -919,15 +919,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_scheduled_audit)
         """
     async def create_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
+        behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSecurityProfileResponseTypeDef:
         """
         Creates a Device Defender security profile.
@@ -951,42 +951,42 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_stream)
         """
     async def create_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadUnionTypeDef = ...,
+        attributePayload: AttributePayloadTypeDef = ...,
         billingGroupName: str = ...
     ) -> CreateThingResponseTypeDef:
         """
         Creates a thing record in the registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing)
         """
     async def create_thing_group(
         self,
         *,
         thingGroupName: str,
         parentGroupName: str = ...,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef = ...,
+        thingGroupProperties: ThingGroupPropertiesTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingGroupResponseTypeDef:
         """
         Create a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_group)
         """
     async def create_thing_type(
         self,
         *,
         thingTypeName: str,
-        thingTypeProperties: ThingTypePropertiesUnionTypeDef = ...,
+        thingTypeProperties: ThingTypePropertiesTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateThingTypeResponseTypeDef:
         """
         Creates a new thing type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.create_thing_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#create_thing_type)
@@ -2673,32 +2673,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.set_v2_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#set_v2_logging_options)
         """
     async def start_audit_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: AuditMitigationActionsTaskTargetUnionTypeDef,
+        target: AuditMitigationActionsTaskTargetTypeDef,
         auditCheckToActionsMapping: Mapping[str, Sequence[str]],
         clientRequestToken: str
     ) -> StartAuditMitigationActionsTaskResponseTypeDef:
         """
         Starts a task that applies a set of mitigation actions to the specified target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_audit_mitigation_actions_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#start_audit_mitigation_actions_task)
         """
     async def start_detect_mitigation_actions_task(
         self,
         *,
         taskId: str,
-        target: DetectMitigationActionsTaskTargetUnionTypeDef,
+        target: DetectMitigationActionsTaskTargetTypeDef,
         actions: Sequence[str],
         clientRequestToken: str,
-        violationEventOccurrenceRange: ViolationEventOccurrenceRangeUnionTypeDef = ...,
+        violationEventOccurrenceRange: ViolationEventOccurrenceRangeTypeDef = ...,
         includeOnlyActiveViolations: bool = ...,
         includeSuppressedAlerts: bool = ...
     ) -> StartDetectMitigationActionsTaskResponseTypeDef:
         """
         Starts a Device Defender ML Detect mitigation actions task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.start_detect_mitigation_actions_task)
@@ -2735,15 +2735,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#tag_resource)
         """
     async def test_authorization(
         self,
         *,
-        authInfos: Sequence[AuthInfoUnionTypeDef],
+        authInfos: Sequence[AuthInfoTypeDef],
         principal: str = ...,
         cognitoIdentityPoolId: str = ...,
         clientId: str = ...,
         policyNamesToAdd: Sequence[str] = ...,
         policyNamesToSkip: Sequence[str] = ...
     ) -> TestAuthorizationResponseTypeDef:
         """
@@ -2902,15 +2902,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_domain_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_domain_configuration)
         """
     async def update_dynamic_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
+        thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...,
         indexName: str = ...,
         queryString: str = ...,
         queryVersion: str = ...
     ) -> UpdateDynamicThingGroupResponseTypeDef:
         """
         Updates a dynamic thing group.
@@ -2929,15 +2929,15 @@
         """
     async def update_fleet_metric(
         self,
         *,
         metricName: str,
         indexName: str,
         queryString: str = ...,
-        aggregationType: AggregationTypeUnionTypeDef = ...,
+        aggregationType: AggregationTypeTypeDef = ...,
         period: int = ...,
         aggregationField: str = ...,
         description: str = ...,
         queryVersion: str = ...,
         unit: FleetMetricUnitType = ...,
         expectedVersion: int = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -2946,47 +2946,47 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_fleet_metric)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_fleet_metric)
         """
     async def update_indexing_configuration(
         self,
         *,
-        thingIndexingConfiguration: ThingIndexingConfigurationUnionTypeDef = ...,
-        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationUnionTypeDef = ...
+        thingIndexingConfiguration: ThingIndexingConfigurationTypeDef = ...,
+        thingGroupIndexingConfiguration: ThingGroupIndexingConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the search configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_indexing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_indexing_configuration)
         """
     async def update_job(
         self,
         *,
         jobId: str,
         description: str = ...,
         presignedUrlConfig: PresignedUrlConfigTypeDef = ...,
         jobExecutionsRolloutConfig: JobExecutionsRolloutConfigTypeDef = ...,
-        abortConfig: AbortConfigUnionTypeDef = ...,
+        abortConfig: AbortConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...,
         namespaceId: str = ...,
-        jobExecutionsRetryConfig: JobExecutionsRetryConfigUnionTypeDef = ...
+        jobExecutionsRetryConfig: JobExecutionsRetryConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates supported fields of the specified job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_job)
         """
     async def update_mitigation_action(
         self,
         *,
         actionName: str,
         roleArn: str = ...,
-        actionParams: MitigationActionParamsUnionTypeDef = ...
+        actionParams: MitigationActionParamsTypeDef = ...
     ) -> UpdateMitigationActionResponseTypeDef:
         """
         Updates the definition for the specified mitigation action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_mitigation_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_mitigation_action)
         """
@@ -3076,15 +3076,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_scheduled_audit)
         """
     async def update_security_profile(
         self,
         *,
         securityProfileName: str,
         securityProfileDescription: str = ...,
-        behaviors: Sequence[BehaviorUnionTypeDef] = ...,
+        behaviors: Sequence[BehaviorTypeDef] = ...,
         alertTargets: Mapping[Literal["SNS"], AlertTargetTypeDef] = ...,
         additionalMetricsToRetain: Sequence[str] = ...,
         additionalMetricsToRetainV2: Sequence[MetricToRetainTypeDef] = ...,
         deleteBehaviors: bool = ...,
         deleteAlertTargets: bool = ...,
         deleteAdditionalMetricsToRetain: bool = ...,
         expectedVersion: int = ...
@@ -3110,29 +3110,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_stream)
         """
     async def update_thing(
         self,
         *,
         thingName: str,
         thingTypeName: str = ...,
-        attributePayload: AttributePayloadUnionTypeDef = ...,
+        attributePayload: AttributePayloadTypeDef = ...,
         expectedVersion: int = ...,
         removeThingType: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates the data for a thing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing)
         """
     async def update_thing_group(
         self,
         *,
         thingGroupName: str,
-        thingGroupProperties: ThingGroupPropertiesUnionTypeDef,
+        thingGroupProperties: ThingGroupPropertiesTypeDef,
         expectedVersion: int = ...
     ) -> UpdateThingGroupResponseTypeDef:
         """
         Update a thing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_thing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_thing_group)
@@ -3157,15 +3157,15 @@
         """
         Updates a topic rule destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.update_topic_rule_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#update_topic_rule_destination)
         """
     async def validate_security_profile_behaviors(
-        self, *, behaviors: Sequence[BehaviorUnionTypeDef]
+        self, *, behaviors: Sequence[BehaviorTypeDef]
     ) -> ValidateSecurityProfileBehaviorsResponseTypeDef:
         """
         Validates a Device Defender security profile behaviors specification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Client.validate_security_profile_behaviors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/client/#validate_security_profile_behaviors)
         """
```

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,14 +403,15 @@
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
@@ -506,14 +507,15 @@
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
@@ -592,26 +594,28 @@
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

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/literals.pyi` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,15 @@
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
@@ -504,14 +505,15 @@
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
@@ -590,26 +592,28 @@
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

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/paginator.pyi` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.py` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
-from aiobotocore.response import StreamingBody
+from botocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AggregationTypeNameType,
     AuditCheckRunStatusType,
     AuditFindingSeverityType,
     AuditFrequencyType,
@@ -99,64 +99,57 @@
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionOutputTypeDef",
+    "KafkaActionTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "KafkaActionTypeDef",
-    "MetricValueOutputTypeDef",
+    "MetricValueTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
-    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
-    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
-    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
-    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
-    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
-    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
@@ -167,15 +160,14 @@
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
-    "CodeSigningSignatureOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TimestampTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "PresignedUrlConfigTypeDef",
@@ -254,25 +246,23 @@
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     "DescribeThingRequestRequestTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
-    "ThingTypePropertiesOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
-    "DetectMitigationActionsTaskTargetOutputTypeDef",
-    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
@@ -301,15 +291,14 @@
     "GroupNameAndArnTypeDef",
     "HttpActionHeaderTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
-    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
@@ -422,18 +411,16 @@
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
-    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "AssetPropertyValueTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "CancelJobResponseTypeDef",
@@ -514,70 +501,63 @@
     "UpdateDomainConfigurationResponseTypeDef",
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
-    "ThingGroupPropertiesOutputTypeDef",
-    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
-    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "AuthInfoUnionTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
-    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "CodeSigningSignatureTypeDef",
     "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "CustomCodeSigningOutputTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
     "ListDetectMitigationActionsTasksRequestRequestTypeDef",
     "ListMetricValuesRequestRequestTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
-    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
@@ -585,23 +565,21 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
-    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "DetectMitigationActionsTaskTargetUnionTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
-    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
     "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
     "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
@@ -664,20 +642,18 @@
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
     "HttpAuthorizationTypeDef",
-    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
-    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -693,73 +669,56 @@
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
-    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
-    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
     "ThingDocumentTypeDef",
-    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
-    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
-    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
-    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
-    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "CustomCodeSigningTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
-    "ViolationEventOccurrenceRangeUnionTypeDef",
-    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
-    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
-    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
-    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
-    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
-    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
@@ -771,58 +730,52 @@
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
-    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
-    "BehaviorUnionTypeDef",
-    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRuleTypeDef",
     "TopicRulePayloadTypeDef",
+    "TopicRuleTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
     "OTAUpdateInfoTypeDef",
-    "OTAUpdateFileUnionTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -997,35 +950,33 @@
 )
 
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
 
-_RequiredKafkaActionOutputTypeDef = TypedDict(
-    "_RequiredKafkaActionOutputTypeDef",
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Dict[str, str],
+        "clientProperties": Mapping[str, str],
     },
 )
-_OptionalKafkaActionOutputTypeDef = TypedDict(
-    "_OptionalKafkaActionOutputTypeDef",
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
 
-class KafkaActionOutputTypeDef(
-    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
-):
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
     pass
 
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
@@ -1150,45 +1101,23 @@
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
-    {
-        "destinationArn": str,
-        "topic": str,
-        "clientProperties": Mapping[str, str],
-    },
-)
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
-    {
-        "key": str,
-        "partition": str,
-    },
-    total=False,
-)
-
-
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
-    pass
-
-
-MetricValueOutputTypeDef = TypedDict(
-    "MetricValueOutputTypeDef",
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
     {
         "count": int,
-        "cidrs": List[str],
-        "ports": List[int],
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
         "number": float,
-        "numbers": List[float],
-        "strings": List[str],
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1216,36 +1145,14 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
-_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
-    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
-    {
-        "thingGroupNames": List[str],
-    },
-)
-_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
-    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
-    {
-        "overrideDynamicGroups": bool,
-    },
-    total=False,
-)
-
-
-class AddThingsToThingGroupParamsOutputTypeDef(
-    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
-    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
-):
-    pass
-
-
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1259,35 +1166,14 @@
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
 
-_RequiredAggregationTypeOutputTypeDef = TypedDict(
-    "_RequiredAggregationTypeOutputTypeDef",
-    {
-        "name": AggregationTypeNameType,
-    },
-)
-_OptionalAggregationTypeOutputTypeDef = TypedDict(
-    "_OptionalAggregationTypeOutputTypeDef",
-    {
-        "values": List[str],
-    },
-    total=False,
-)
-
-
-class AggregationTypeOutputTypeDef(
-    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
-):
-    pass
-
-
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1415,23 +1301,14 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
-AttributePayloadOutputTypeDef = TypedDict(
-    "AttributePayloadOutputTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "merge": bool,
-    },
-    total=False,
-)
-
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
@@ -1481,30 +1358,20 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetOutputTypeDef",
-    {
-        "auditTaskId": str,
-        "findingIds": List[str],
-        "auditCheckToReasonCodeFilter": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 AuditMitigationActionsTaskTargetTypeDef = TypedDict(
     "AuditMitigationActionsTaskTargetTypeDef",
     {
         "auditTaskId": str,
-        "findingIds": Sequence[str],
-        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+        "findingIds": List[str],
+        "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
@@ -1521,33 +1388,14 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
-_RequiredAuthInfoOutputTypeDef = TypedDict(
-    "_RequiredAuthInfoOutputTypeDef",
-    {
-        "resources": List[str],
-    },
-)
-_OptionalAuthInfoOutputTypeDef = TypedDict(
-    "_OptionalAuthInfoOutputTypeDef",
-    {
-        "actionType": ActionTypeType,
-    },
-    total=False,
-)
-
-
-class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
-    pass
-
-
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1644,27 +1492,14 @@
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
-    {
-        "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
-        "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
-    },
-    total=False,
-)
-
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
@@ -1852,22 +1687,14 @@
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
-CodeSigningSignatureOutputTypeDef = TypedDict(
-    "CodeSigningSignatureOutputTypeDef",
-    {
-        "inlineDocument": bytes,
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2837,23 +2664,14 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ThingTypePropertiesOutputTypeDef = TypedDict(
-    "ThingTypePropertiesOutputTypeDef",
-    {
-        "thingTypeDescription": str,
-        "searchableAttributes": List[str],
-    },
-    total=False,
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -2913,42 +2731,32 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetOutputTypeDef",
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeOutputTypeDef",
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
-    {
-        "violationIds": Sequence[str],
-        "securityProfileName": str,
-        "behaviorName": str,
-    },
-    total=False,
-)
-
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3294,26 +3102,18 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
-IndexingFilterOutputTypeDef = TypedDict(
-    "IndexingFilterOutputTypeDef",
-    {
-        "namedShadowNames": List[str],
-    },
-    total=False,
-)
-
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": Sequence[str],
+        "namedShadowNames": List[str],
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -4970,38 +4770,30 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
-AbortConfigOutputTypeDef = TypedDict(
-    "AbortConfigOutputTypeDef",
-    {
-        "criteriaList": List[AbortCriteriaTypeDef],
-    },
-)
-
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueOutputTypeDef,
+        "value": MetricValueTypeDef,
     },
     total=False,
 )
 
-AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -5380,15 +5172,15 @@
 )
 
 DescribeFleetMetricResponseTypeDef = TypedDict(
     "DescribeFleetMetricResponseTypeDef",
     {
         "metricName": str,
         "queryString": str,
-        "aggregationType": AggregationTypeOutputTypeDef,
+        "aggregationType": AggregationTypeTypeDef,
         "period": int,
         "aggregationField": str,
         "description": str,
         "queryVersion": str,
         "indexName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
@@ -5909,24 +5701,14 @@
     "UpdateThingGroupResponseTypeDef",
     {
         "version": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ThingGroupPropertiesOutputTypeDef = TypedDict(
-    "ThingGroupPropertiesOutputTypeDef",
-    {
-        "thingGroupDescription": str,
-        "attributePayload": AttributePayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -5993,17 +5775,14 @@
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AuditMitigationActionsTaskTargetUnionTypeDef = Union[
-    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
-]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -6039,15 +5818,39 @@
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
+
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6081,28 +5884,14 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
-BehaviorCriteriaOutputTypeDef = TypedDict(
-    "BehaviorCriteriaOutputTypeDef",
-    {
-        "comparisonOperator": ComparisonOperatorType,
-        "value": MetricValueOutputTypeDef,
-        "durationSeconds": int,
-        "consecutiveDatapointsToAlarm": int,
-        "consecutiveDatapointsToClear": int,
-        "statisticalThreshold": StatisticalThresholdTypeDef,
-        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
-    },
-    total=False,
-)
-
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6275,25 +6064,14 @@
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomCodeSigningOutputTypeDef = TypedDict(
-    "CustomCodeSigningOutputTypeDef",
-    {
-        "signature": CodeSigningSignatureOutputTypeDef,
-        "certificateChain": CodeSigningCertificateChainTypeDef,
-        "hashAlgorithm": str,
-        "signatureAlgorithm": str,
-    },
-    total=False,
-)
-
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6450,22 +6228,14 @@
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
-    {
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-    },
-)
-
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -6727,25 +6497,14 @@
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-SchedulingConfigOutputTypeDef = TypedDict(
-    "SchedulingConfigOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-        "endBehavior": JobEndBehaviorType,
-        "maintenanceWindows": List[MaintenanceWindowTypeDef],
-    },
-    total=False,
-)
-
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -6976,34 +6735,31 @@
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
+        "thingTypeProperties": ThingTypePropertiesTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
+        "thingTypeProperties": ThingTypePropertiesTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
-ThingTypePropertiesUnionTypeDef = Union[
-    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
-]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -7013,17 +6769,41 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DetectMitigationActionsTaskTargetUnionTypeDef = Union[
-    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
-]
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7050,48 +6830,25 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
-_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
-    {
-        "thingGroupIndexingMode": ThingGroupIndexingModeType,
-    },
-)
-_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
-    {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
-    },
-    total=False,
-)
-
-
-class ThingGroupIndexingConfigurationOutputTypeDef(
-    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
-    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": Sequence[FieldTypeDef],
-        "customFields": Sequence[FieldTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
     },
     total=False,
 )
 
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
@@ -8093,55 +7850,28 @@
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
-_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredThingIndexingConfigurationOutputTypeDef",
-    {
-        "thingIndexingMode": ThingIndexingModeType,
-    },
-)
-_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalThingIndexingConfigurationOutputTypeDef",
-    {
-        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
-        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
-        "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
-        "filter": IndexingFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ThingIndexingConfigurationOutputTypeDef(
-    _RequiredThingIndexingConfigurationOutputTypeDef,
-    _OptionalThingIndexingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": Sequence[FieldTypeDef],
-        "customFields": Sequence[FieldTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 
 class ThingIndexingConfigurationTypeDef(
@@ -8182,21 +7912,14 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
-JobExecutionsRetryConfigOutputTypeDef = TypedDict(
-    "JobExecutionsRetryConfigOutputTypeDef",
-    {
-        "criteriaList": List[RetryCriteriaTypeDef],
-    },
-)
-
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
@@ -8404,53 +8127,27 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
-MitigationActionParamsOutputTypeDef = TypedDict(
-    "MitigationActionParamsOutputTypeDef",
-    {
-        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
-        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
-        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
-        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
-        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
-        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
-    },
-    total=False,
-)
-
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
-MqttHeadersOutputTypeDef = TypedDict(
-    "MqttHeadersOutputTypeDef",
-    {
-        "payloadFormatIndicator": str,
-        "contentType": str,
-        "responseTopic": str,
-        "correlationData": str,
-        "messageExpiry": str,
-        "userProperties": List[UserPropertyTypeDef],
-    },
-    total=False,
-)
-
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
@@ -8488,38 +8185,14 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredTimestreamActionOutputTypeDef = TypedDict(
-    "_RequiredTimestreamActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "databaseName": str,
-        "tableName": str,
-        "dimensions": List[TimestreamDimensionTypeDef],
-    },
-)
-_OptionalTimestreamActionOutputTypeDef = TypedDict(
-    "_OptionalTimestreamActionOutputTypeDef",
-    {
-        "timestamp": TimestreamTimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class TimestreamActionOutputTypeDef(
-    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
-):
-    pass
-
-
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -8580,15 +8253,14 @@
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8599,39 +8271,14 @@
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
-_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
-    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
-    {
-        "propertyValues": List[AssetPropertyValueTypeDef],
-    },
-)
-_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
-    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
-    {
-        "entryId": str,
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-    },
-    total=False,
-)
-
-
-class PutAssetPropertyValueEntryOutputTypeDef(
-    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
-    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
-):
-    pass
-
-
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8697,17 +8344,14 @@
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
-ThingGroupPropertiesUnionTypeDef = Union[
-    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8748,70 +8392,23 @@
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[AuthInfoUnionTypeDef],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
-    },
-    total=False,
-)
-
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
-
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-_RequiredBehaviorOutputTypeDef = TypedDict(
-    "_RequiredBehaviorOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalBehaviorOutputTypeDef = TypedDict(
-    "_OptionalBehaviorOutputTypeDef",
-    {
-        "metric": str,
-        "metricDimension": MetricDimensionTypeDef,
-        "criteria": BehaviorCriteriaOutputTypeDef,
-        "suppressAlerts": bool,
-    },
-    total=False,
-)
-
-
-class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
-    pass
-
-
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8905,45 +8502,14 @@
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-
-ViolationEventOccurrenceRangeUnionTypeDef = Union[
-    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
-]
-SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8964,17 +8530,14 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-ThingGroupIndexingConfigurationUnionTypeDef = Union[
-    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
-]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -9036,45 +8599,24 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHttpActionOutputTypeDef = TypedDict(
-    "_RequiredHttpActionOutputTypeDef",
-    {
-        "url": str,
-    },
-)
-_OptionalHttpActionOutputTypeDef = TypedDict(
-    "_OptionalHttpActionOutputTypeDef",
-    {
-        "confirmationUrl": str,
-        "headers": List[HttpActionHeaderTypeDef],
-        "auth": HttpAuthorizationTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
-    pass
-
-
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionTypeDef = TypedDict(
@@ -9091,23 +8633,20 @@
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
+        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ThingIndexingConfigurationUnionTypeDef = Union[
-    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
-]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
@@ -9135,17 +8674,14 @@
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobExecutionsRetryConfigUnionTypeDef = Union[
-    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9156,40 +8692,14 @@
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeMitigationActionResponseTypeDef = TypedDict(
-    "DescribeMitigationActionResponseTypeDef",
-    {
-        "actionName": str,
-        "actionType": MitigationActionTypeType,
-        "actionArn": str,
-        "actionId": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsOutputTypeDef,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MitigationActionTypeDef = TypedDict(
-    "MitigationActionTypeDef",
-    {
-        "name": str,
-        "id": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
@@ -9206,59 +8716,59 @@
 class CreateMitigationActionRequestRequestTypeDef(
     _RequiredCreateMitigationActionRequestRequestTypeDef,
     _OptionalCreateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
-MitigationActionParamsUnionTypeDef = Union[
-    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
-]
-_RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMitigationActionRequestRequestTypeDef",
+DescribeMitigationActionResponseTypeDef = TypedDict(
+    "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
+        "actionType": MitigationActionTypeType,
+        "actionArn": str,
+        "actionId": str,
+        "roleArn": str,
+        "actionParams": MitigationActionParamsTypeDef,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMitigationActionRequestRequestTypeDef",
+
+MitigationActionTypeDef = TypedDict(
+    "MitigationActionTypeDef",
     {
+        "name": str,
+        "id": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
     total=False,
 )
 
-
-class UpdateMitigationActionRequestRequestTypeDef(
-    _RequiredUpdateMitigationActionRequestRequestTypeDef,
-    _OptionalUpdateMitigationActionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRepublishActionOutputTypeDef = TypedDict(
-    "_RequiredRepublishActionOutputTypeDef",
+_RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
-        "roleArn": str,
-        "topic": str,
+        "actionName": str,
     },
 )
-_OptionalRepublishActionOutputTypeDef = TypedDict(
-    "_OptionalRepublishActionOutputTypeDef",
+_OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMitigationActionRequestRequestTypeDef",
     {
-        "qos": int,
-        "headers": MqttHeadersOutputTypeDef,
+        "roleArn": str,
+        "actionParams": MitigationActionParamsTypeDef,
     },
     total=False,
 )
 
 
-class RepublishActionOutputTypeDef(
-    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
+class UpdateMitigationActionRequestRequestTypeDef(
+    _RequiredUpdateMitigationActionRequestRequestTypeDef,
+    _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
@@ -9494,118 +9004,163 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoOutputTypeDef,
+        "authInfo": AuthInfoTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
-IotSiteWiseActionOutputTypeDef = TypedDict(
-    "IotSiteWiseActionOutputTypeDef",
-    {
-        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
-        "roleArn": str,
-    },
-)
-
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorOutputTypeDef,
-        "lastViolationValue": MetricValueOutputTypeDef,
+        "behavior": BehaviorTypeDef,
+        "lastViolationValue": MetricValueTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorOutputTypeDef],
+        "behaviors": List[BehaviorTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorOutputTypeDef],
+        "behaviors": List[BehaviorTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorTypeDef],
+    },
+)
+
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorOutputTypeDef,
-        "metricValue": MetricValueOutputTypeDef,
+        "behavior": BehaviorTypeDef,
+        "metricValue": MetricValueTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "violationEventType": ViolationEventTypeType,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
-BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
-CodeSigningOutputTypeDef = TypedDict(
-    "CodeSigningOutputTypeDef",
-    {
-        "awsSignerJobId": str,
-        "startSigningJobParameter": StartSigningJobParameterTypeDef,
-        "customCodeSigning": CustomCodeSigningOutputTypeDef,
-    },
-    total=False,
-)
-
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
@@ -9687,17 +9242,17 @@
         "jobTemplateId": str,
         "description": str,
         "documentSource": str,
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
+        "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "destinationPackageVersions": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
@@ -9710,26 +9265,26 @@
         "forceCanceled": bool,
         "reasonCode": str,
         "comment": str,
         "targets": List[str],
         "description": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
+        "abortConfig": AbortConfigTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "completedAt": datetime,
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "schedulingConfig": SchedulingConfigTypeDef,
         "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
         "destinationPackageVersions": List[str],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
@@ -9770,30 +9325,30 @@
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
+        "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
@@ -9838,44 +9393,14 @@
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "dynamoDB": DynamoDBActionTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionTypeDef,
-        "lambda": LambdaActionTypeDef,
-        "sns": SnsActionTypeDef,
-        "sqs": SqsActionTypeDef,
-        "kinesis": KinesisActionTypeDef,
-        "republish": RepublishActionOutputTypeDef,
-        "s3": S3ActionTypeDef,
-        "firehose": FirehoseActionTypeDef,
-        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
-        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
-        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
-        "elasticsearch": ElasticsearchActionTypeDef,
-        "salesforce": SalesforceActionTypeDef,
-        "iotAnalytics": IotAnalyticsActionTypeDef,
-        "iotEvents": IotEventsActionTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-        "stepFunctions": StepFunctionsActionTypeDef,
-        "timestream": TimestreamActionOutputTypeDef,
-        "http": HttpActionOutputTypeDef,
-        "kafka": KafkaActionOutputTypeDef,
-        "openSearch": OpenSearchActionTypeDef,
-        "location": LocationActionTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9916,91 +9441,14 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
-    },
-    total=False,
-)
-
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-    },
-)
-
-OTAUpdateFileOutputTypeDef = TypedDict(
-    "OTAUpdateFileOutputTypeDef",
-    {
-        "fileName": str,
-        "fileType": int,
-        "fileVersion": str,
-        "fileLocation": FileLocationTypeDef,
-        "codeSigning": CodeSigningOutputTypeDef,
-        "attributes": Dict[str, str],
-    },
-    total=False,
-)
-
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -10049,49 +9497,81 @@
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredTopicRulePayloadTypeDef = TypedDict(
+    "_RequiredTopicRulePayloadTypeDef",
+    {
+        "sql": str,
+        "actions": Sequence[ActionTypeDef],
+    },
+)
+_OptionalTopicRulePayloadTypeDef = TypedDict(
+    "_OptionalTopicRulePayloadTypeDef",
+    {
+        "description": str,
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionTypeDef,
+    },
+    total=False,
+)
+
+
+class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
+    pass
+
+
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
         "sql": str,
         "description": str,
         "createdAt": datetime,
-        "actions": List[ActionOutputTypeDef],
+        "actions": List[ActionTypeDef],
         "ruleDisabled": bool,
         "awsIotSqlVersion": str,
-        "errorAction": ActionOutputTypeDef,
+        "errorAction": ActionTypeDef,
     },
     total=False,
 )
 
-_RequiredTopicRulePayloadTypeDef = TypedDict(
-    "_RequiredTopicRulePayloadTypeDef",
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
-        "sql": str,
-        "actions": Sequence[ActionTypeDef],
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileTypeDef],
+        "roleArn": str,
     },
 )
-_OptionalTopicRulePayloadTypeDef = TypedDict(
-    "_OptionalTopicRulePayloadTypeDef",
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
     {
         "description": str,
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
     pass
 
 
 OTAUpdateInfoTypeDef = TypedDict(
     "OTAUpdateInfoTypeDef",
     {
         "otaUpdateId": str,
@@ -10100,34 +9580,24 @@
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
         "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
         "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
+        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
-OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
-    {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
@@ -10150,45 +9620,23 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetOTAUpdateResponseTypeDef = TypedDict(
-    "GetOTAUpdateResponseTypeDef",
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
     {
-        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileUnionTypeDef],
-        "roleArn": str,
-    },
-)
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+GetOTAUpdateResponseTypeDef = TypedDict(
+    "GetOTAUpdateResponseTypeDef",
     {
-        "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
+        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot/type_defs.pyi` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
-from aiobotocore.response import StreamingBody
+from botocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AggregationTypeNameType,
     AuditCheckRunStatusType,
     AuditFindingSeverityType,
     AuditFrequencyType,
@@ -98,64 +98,57 @@
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionOutputTypeDef",
+    "KafkaActionTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "KafkaActionTypeDef",
-    "MetricValueOutputTypeDef",
+    "MetricValueTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
-    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
-    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
-    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
-    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
-    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
     "MachineLearningDetectionConfigTypeDef",
     "StatisticalThresholdTypeDef",
-    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BlobTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
@@ -166,15 +159,14 @@
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
     "CodeSigningCertificateChainTypeDef",
-    "CodeSigningSignatureOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TimestampTypeDef",
     "TagTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "PresignedUrlConfigTypeDef",
@@ -253,25 +245,23 @@
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     "DescribeThingRequestRequestTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
-    "ThingTypePropertiesOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
-    "DetectMitigationActionsTaskTargetOutputTypeDef",
-    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
@@ -300,15 +290,14 @@
     "GroupNameAndArnTypeDef",
     "HttpActionHeaderTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
-    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
@@ -421,18 +410,16 @@
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
-    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "AggregationTypeUnionTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "AssetPropertyValueTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "CancelJobResponseTypeDef",
@@ -513,70 +500,63 @@
     "UpdateDomainConfigurationResponseTypeDef",
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
-    "ThingGroupPropertiesOutputTypeDef",
-    "AttributePayloadUnionTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
-    "AuditMitigationActionsTaskTargetUnionTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
-    "AuthInfoUnionTypeDef",
+    "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
-    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "CodeSigningSignatureTypeDef",
     "MqttContextTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "CustomCodeSigningOutputTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
     "ListDetectMitigationActionsTasksRequestRequestTypeDef",
     "ListMetricValuesRequestRequestTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
-    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
     "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
@@ -584,23 +564,21 @@
     "RegisterCACertificateRequestRequestTypeDef",
     "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
-    "ThingTypePropertiesUnionTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "DetectMitigationActionsTaskTargetUnionTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
     "ExponentialRolloutRateTypeDef",
-    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
     "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
     "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
@@ -663,20 +641,18 @@
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
     "HttpAuthorizationTypeDef",
-    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
-    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -692,73 +668,56 @@
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
-    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
-    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
     "ResourceIdentifierTypeDef",
     "ThingDocumentTypeDef",
-    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
-    "AbortConfigUnionTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
-    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
-    "ThingGroupPropertiesUnionTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
-    "TestAuthorizationRequestRequestTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
-    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "CustomCodeSigningTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
-    "ViolationEventOccurrenceRangeUnionTypeDef",
-    "SchedulingConfigUnionTypeDef",
     "ListThingTypesResponseTypeDef",
     "StartSigningJobParameterTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "ThingGroupIndexingConfigurationUnionTypeDef",
     "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
-    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
-    "ThingIndexingConfigurationUnionTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
-    "JobExecutionsRetryConfigUnionTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
-    "MitigationActionParamsUnionTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
-    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
@@ -770,58 +729,52 @@
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
-    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
-    "BehaviorUnionTypeDef",
-    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRuleTypeDef",
     "TopicRulePayloadTypeDef",
+    "TopicRuleTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
     "OTAUpdateInfoTypeDef",
-    "OTAUpdateFileUnionTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
 )
 
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
@@ -984,34 +937,32 @@
     },
     total=False,
 )
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
-_RequiredKafkaActionOutputTypeDef = TypedDict(
-    "_RequiredKafkaActionOutputTypeDef",
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Dict[str, str],
+        "clientProperties": Mapping[str, str],
     },
 )
-_OptionalKafkaActionOutputTypeDef = TypedDict(
-    "_OptionalKafkaActionOutputTypeDef",
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
-class KafkaActionOutputTypeDef(
-    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
-):
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
     pass
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
         "streamName": str,
@@ -1125,43 +1076,23 @@
 )
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
-    {
-        "destinationArn": str,
-        "topic": str,
-        "clientProperties": Mapping[str, str],
-    },
-)
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
-    {
-        "key": str,
-        "partition": str,
-    },
-    total=False,
-)
-
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
-    pass
-
-MetricValueOutputTypeDef = TypedDict(
-    "MetricValueOutputTypeDef",
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
     {
         "count": int,
-        "cidrs": List[str],
-        "ports": List[int],
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
         "number": float,
-        "numbers": List[float],
-        "strings": List[str],
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1189,34 +1120,14 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
-_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
-    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
-    {
-        "thingGroupNames": List[str],
-    },
-)
-_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
-    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
-    {
-        "overrideDynamicGroups": bool,
-    },
-    total=False,
-)
-
-class AddThingsToThingGroupParamsOutputTypeDef(
-    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
-    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
-):
-    pass
-
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1228,33 +1139,14 @@
 )
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
-_RequiredAggregationTypeOutputTypeDef = TypedDict(
-    "_RequiredAggregationTypeOutputTypeDef",
-    {
-        "name": AggregationTypeNameType,
-    },
-)
-_OptionalAggregationTypeOutputTypeDef = TypedDict(
-    "_OptionalAggregationTypeOutputTypeDef",
-    {
-        "values": List[str],
-    },
-    total=False,
-)
-
-class AggregationTypeOutputTypeDef(
-    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
-):
-    pass
-
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1376,23 +1268,14 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
-AttributePayloadOutputTypeDef = TypedDict(
-    "AttributePayloadOutputTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "merge": bool,
-    },
-    total=False,
-)
-
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
@@ -1442,30 +1325,20 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetOutputTypeDef",
-    {
-        "auditTaskId": str,
-        "findingIds": List[str],
-        "auditCheckToReasonCodeFilter": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 AuditMitigationActionsTaskTargetTypeDef = TypedDict(
     "AuditMitigationActionsTaskTargetTypeDef",
     {
         "auditTaskId": str,
-        "findingIds": Sequence[str],
-        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+        "findingIds": List[str],
+        "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
@@ -1482,31 +1355,14 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
-_RequiredAuthInfoOutputTypeDef = TypedDict(
-    "_RequiredAuthInfoOutputTypeDef",
-    {
-        "resources": List[str],
-    },
-)
-_OptionalAuthInfoOutputTypeDef = TypedDict(
-    "_OptionalAuthInfoOutputTypeDef",
-    {
-        "actionType": ActionTypeType,
-    },
-    total=False,
-)
-
-class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
-    pass
-
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1601,27 +1457,14 @@
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
-    {
-        "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
-        "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
-    },
-    total=False,
-)
-
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
@@ -1803,22 +1646,14 @@
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
-CodeSigningSignatureOutputTypeDef = TypedDict(
-    "CodeSigningSignatureOutputTypeDef",
-    {
-        "inlineDocument": bytes,
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2744,23 +2579,14 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ThingTypePropertiesOutputTypeDef = TypedDict(
-    "ThingTypePropertiesOutputTypeDef",
-    {
-        "thingTypeDescription": str,
-        "searchableAttributes": List[str],
-    },
-    total=False,
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -2820,42 +2646,32 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetOutputTypeDef",
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeOutputTypeDef",
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
-    {
-        "violationIds": Sequence[str],
-        "securityProfileName": str,
-        "behaviorName": str,
-    },
-    total=False,
-)
-
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3195,26 +3011,18 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
-IndexingFilterOutputTypeDef = TypedDict(
-    "IndexingFilterOutputTypeDef",
-    {
-        "namedShadowNames": List[str],
-    },
-    total=False,
-)
-
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": Sequence[str],
+        "namedShadowNames": List[str],
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -4799,38 +4607,30 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
-AbortConfigOutputTypeDef = TypedDict(
-    "AbortConfigOutputTypeDef",
-    {
-        "criteriaList": List[AbortCriteriaTypeDef],
-    },
-)
-
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueOutputTypeDef,
+        "value": MetricValueTypeDef,
     },
     total=False,
 )
 
-AggregationTypeUnionTypeDef = Union[AggregationTypeTypeDef, AggregationTypeOutputTypeDef]
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -5205,15 +5005,15 @@
 )
 
 DescribeFleetMetricResponseTypeDef = TypedDict(
     "DescribeFleetMetricResponseTypeDef",
     {
         "metricName": str,
         "queryString": str,
-        "aggregationType": AggregationTypeOutputTypeDef,
+        "aggregationType": AggregationTypeTypeDef,
         "period": int,
         "aggregationField": str,
         "description": str,
         "queryVersion": str,
         "indexName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
@@ -5734,24 +5534,14 @@
     "UpdateThingGroupResponseTypeDef",
     {
         "version": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ThingGroupPropertiesOutputTypeDef = TypedDict(
-    "ThingGroupPropertiesOutputTypeDef",
-    {
-        "thingGroupDescription": str,
-        "attributePayload": AttributePayloadOutputTypeDef,
-    },
-    total=False,
-)
-
-AttributePayloadUnionTypeDef = Union[AttributePayloadTypeDef, AttributePayloadOutputTypeDef]
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -5814,17 +5604,14 @@
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AuditMitigationActionsTaskTargetUnionTypeDef = Union[
-    AuditMitigationActionsTaskTargetTypeDef, AuditMitigationActionsTaskTargetOutputTypeDef
-]
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Mapping[str, Sequence[str]],
         "clientRequestToken": str,
@@ -5860,15 +5647,37 @@
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AuthInfoUnionTypeDef = Union[AuthInfoTypeDef, AuthInfoOutputTypeDef]
+_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_RequiredTestAuthorizationRequestRequestTypeDef",
+    {
+        "authInfos": Sequence[AuthInfoTypeDef],
+    },
+)
+_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
+    "_OptionalTestAuthorizationRequestRequestTypeDef",
+    {
+        "principal": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyNamesToAdd": Sequence[str],
+        "policyNamesToSkip": Sequence[str],
+    },
+    total=False,
+)
+
+class TestAuthorizationRequestRequestTypeDef(
+    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
+):
+    pass
+
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5902,28 +5711,14 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
-BehaviorCriteriaOutputTypeDef = TypedDict(
-    "BehaviorCriteriaOutputTypeDef",
-    {
-        "comparisonOperator": ComparisonOperatorType,
-        "value": MetricValueOutputTypeDef,
-        "durationSeconds": int,
-        "consecutiveDatapointsToAlarm": int,
-        "consecutiveDatapointsToClear": int,
-        "statisticalThreshold": StatisticalThresholdTypeDef,
-        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
-    },
-    total=False,
-)
-
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6092,25 +5887,14 @@
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CustomCodeSigningOutputTypeDef = TypedDict(
-    "CustomCodeSigningOutputTypeDef",
-    {
-        "signature": CodeSigningSignatureOutputTypeDef,
-        "certificateChain": CodeSigningCertificateChainTypeDef,
-        "hashAlgorithm": str,
-        "signatureAlgorithm": str,
-    },
-    total=False,
-)
-
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
         "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6257,22 +6041,14 @@
 
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
-    {
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-    },
-)
-
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
         "authorizerFunctionArn": str,
     },
 )
@@ -6514,25 +6290,14 @@
 
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
-SchedulingConfigOutputTypeDef = TypedDict(
-    "SchedulingConfigOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-        "endBehavior": JobEndBehaviorType,
-        "maintenanceWindows": List[MaintenanceWindowTypeDef],
-    },
-    total=False,
-)
-
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -6753,34 +6518,31 @@
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
+        "thingTypeProperties": ThingTypePropertiesTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
+        "thingTypeProperties": ThingTypePropertiesTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
-ThingTypePropertiesUnionTypeDef = Union[
-    ThingTypePropertiesTypeDef, ThingTypePropertiesOutputTypeDef
-]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -6790,17 +6552,39 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DetectMitigationActionsTaskTargetUnionTypeDef = Union[
-    DetectMitigationActionsTaskTargetTypeDef, DetectMitigationActionsTaskTargetOutputTypeDef
-]
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6827,46 +6611,25 @@
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
-_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
-    {
-        "thingGroupIndexingMode": ThingGroupIndexingModeType,
-    },
-)
-_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
-    {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
-    },
-    total=False,
-)
-
-class ThingGroupIndexingConfigurationOutputTypeDef(
-    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
-    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": Sequence[FieldTypeDef],
-        "customFields": Sequence[FieldTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
     },
     total=False,
 )
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
@@ -7816,53 +7579,28 @@
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
-_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredThingIndexingConfigurationOutputTypeDef",
-    {
-        "thingIndexingMode": ThingIndexingModeType,
-    },
-)
-_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalThingIndexingConfigurationOutputTypeDef",
-    {
-        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
-        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
-        "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
-        "filter": IndexingFilterOutputTypeDef,
-    },
-    total=False,
-)
-
-class ThingIndexingConfigurationOutputTypeDef(
-    _RequiredThingIndexingConfigurationOutputTypeDef,
-    _OptionalThingIndexingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": Sequence[FieldTypeDef],
-        "customFields": Sequence[FieldTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 class ThingIndexingConfigurationTypeDef(
     _RequiredThingIndexingConfigurationTypeDef, _OptionalThingIndexingConfigurationTypeDef
@@ -7901,21 +7639,14 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
-JobExecutionsRetryConfigOutputTypeDef = TypedDict(
-    "JobExecutionsRetryConfigOutputTypeDef",
-    {
-        "criteriaList": List[RetryCriteriaTypeDef],
-    },
-)
-
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
@@ -8121,53 +7852,27 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
-MitigationActionParamsOutputTypeDef = TypedDict(
-    "MitigationActionParamsOutputTypeDef",
-    {
-        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
-        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
-        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
-        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
-        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
-        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
-    },
-    total=False,
-)
-
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
-MqttHeadersOutputTypeDef = TypedDict(
-    "MqttHeadersOutputTypeDef",
-    {
-        "payloadFormatIndicator": str,
-        "contentType": str,
-        "responseTopic": str,
-        "correlationData": str,
-        "messageExpiry": str,
-        "userProperties": List[UserPropertyTypeDef],
-    },
-    total=False,
-)
-
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
@@ -8205,36 +7910,14 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredTimestreamActionOutputTypeDef = TypedDict(
-    "_RequiredTimestreamActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "databaseName": str,
-        "tableName": str,
-        "dimensions": List[TimestreamDimensionTypeDef],
-    },
-)
-_OptionalTimestreamActionOutputTypeDef = TypedDict(
-    "_OptionalTimestreamActionOutputTypeDef",
-    {
-        "timestamp": TimestreamTimestampTypeDef,
-    },
-    total=False,
-)
-
-class TimestreamActionOutputTypeDef(
-    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
-):
-    pass
-
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -8293,15 +7976,14 @@
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AbortConfigUnionTypeDef = Union[AbortConfigTypeDef, AbortConfigOutputTypeDef]
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8312,37 +7994,14 @@
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
-_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
-    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
-    {
-        "propertyValues": List[AssetPropertyValueTypeDef],
-    },
-)
-_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
-    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
-    {
-        "entryId": str,
-        "assetId": str,
-        "propertyId": str,
-        "propertyAlias": str,
-    },
-    total=False,
-)
-
-class PutAssetPropertyValueEntryOutputTypeDef(
-    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
-    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
-):
-    pass
-
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8402,17 +8061,14 @@
 )
 
 class CreateThingGroupRequestRequestTypeDef(
     _RequiredCreateThingGroupRequestRequestTypeDef, _OptionalCreateThingGroupRequestRequestTypeDef
 ):
     pass
 
-ThingGroupPropertiesUnionTypeDef = Union[
-    ThingGroupPropertiesTypeDef, ThingGroupPropertiesOutputTypeDef
-]
 _RequiredUpdateDynamicThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDynamicThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
         "thingGroupProperties": ThingGroupPropertiesTypeDef,
     },
 )
@@ -8449,66 +8105,23 @@
 )
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
-_RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_RequiredTestAuthorizationRequestRequestTypeDef",
-    {
-        "authInfos": Sequence[AuthInfoUnionTypeDef],
-    },
-)
-_OptionalTestAuthorizationRequestRequestTypeDef = TypedDict(
-    "_OptionalTestAuthorizationRequestRequestTypeDef",
-    {
-        "principal": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyNamesToAdd": Sequence[str],
-        "policyNamesToSkip": Sequence[str],
-    },
-    total=False,
-)
-
-class TestAuthorizationRequestRequestTypeDef(
-    _RequiredTestAuthorizationRequestRequestTypeDef, _OptionalTestAuthorizationRequestRequestTypeDef
-):
-    pass
-
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-_RequiredBehaviorOutputTypeDef = TypedDict(
-    "_RequiredBehaviorOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalBehaviorOutputTypeDef = TypedDict(
-    "_OptionalBehaviorOutputTypeDef",
-    {
-        "metric": str,
-        "metricDimension": MetricDimensionTypeDef,
-        "criteria": BehaviorCriteriaOutputTypeDef,
-        "suppressAlerts": bool,
-    },
-    total=False,
-)
-
-class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
-    pass
-
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8596,43 +8209,14 @@
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-ViolationEventOccurrenceRangeUnionTypeDef = Union[
-    ViolationEventOccurrenceRangeTypeDef, ViolationEventOccurrenceRangeOutputTypeDef
-]
-SchedulingConfigUnionTypeDef = Union[SchedulingConfigTypeDef, SchedulingConfigOutputTypeDef]
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8653,17 +8237,14 @@
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-ThingGroupIndexingConfigurationUnionTypeDef = Union[
-    ThingGroupIndexingConfigurationTypeDef, ThingGroupIndexingConfigurationOutputTypeDef
-]
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8721,43 +8302,24 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHttpActionOutputTypeDef = TypedDict(
-    "_RequiredHttpActionOutputTypeDef",
-    {
-        "url": str,
-    },
-)
-_OptionalHttpActionOutputTypeDef = TypedDict(
-    "_OptionalHttpActionOutputTypeDef",
-    {
-        "confirmationUrl": str,
-        "headers": List[HttpActionHeaderTypeDef],
-        "auth": HttpAuthorizationTypeDef,
-    },
-    total=False,
-)
-
-class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
-    pass
-
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionTypeDef = TypedDict(
@@ -8772,23 +8334,20 @@
 
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
+        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ThingIndexingConfigurationUnionTypeDef = Union[
-    ThingIndexingConfigurationTypeDef, ThingIndexingConfigurationOutputTypeDef
-]
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
     },
     total=False,
@@ -8816,17 +8375,14 @@
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobExecutionsRetryConfigUnionTypeDef = Union[
-    JobExecutionsRetryConfigTypeDef, JobExecutionsRetryConfigOutputTypeDef
-]
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8837,65 +8393,62 @@
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMitigationActionRequestRequestTypeDef",
+    {
+        "actionName": str,
+        "roleArn": str,
+        "actionParams": MitigationActionParamsTypeDef,
+    },
+)
+_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMitigationActionRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateMitigationActionRequestRequestTypeDef(
+    _RequiredCreateMitigationActionRequestRequestTypeDef,
+    _OptionalCreateMitigationActionRequestRequestTypeDef,
+):
+    pass
+
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
-        "actionParams": MitigationActionParamsOutputTypeDef,
+        "actionParams": MitigationActionParamsTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
         "id": str,
         "roleArn": str,
-        "actionParams": MitigationActionParamsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMitigationActionRequestRequestTypeDef",
-    {
-        "actionName": str,
-        "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
-)
-_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMitigationActionRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
     total=False,
 )
 
-class CreateMitigationActionRequestRequestTypeDef(
-    _RequiredCreateMitigationActionRequestRequestTypeDef,
-    _OptionalCreateMitigationActionRequestRequestTypeDef,
-):
-    pass
-
-MitigationActionParamsUnionTypeDef = Union[
-    MitigationActionParamsTypeDef, MitigationActionParamsOutputTypeDef
-]
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -8909,35 +8462,14 @@
 
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredRepublishActionOutputTypeDef = TypedDict(
-    "_RequiredRepublishActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "topic": str,
-    },
-)
-_OptionalRepublishActionOutputTypeDef = TypedDict(
-    "_OptionalRepublishActionOutputTypeDef",
-    {
-        "qos": int,
-        "headers": MqttHeadersOutputTypeDef,
-    },
-    total=False,
-)
-
-class RepublishActionOutputTypeDef(
-    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
-):
-    pass
-
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
         "roleArn": str,
         "topic": str,
     },
 )
@@ -9161,118 +8693,159 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoOutputTypeDef,
+        "authInfo": AuthInfoTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
-IotSiteWiseActionOutputTypeDef = TypedDict(
-    "IotSiteWiseActionOutputTypeDef",
-    {
-        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
-        "roleArn": str,
-    },
-)
-
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorOutputTypeDef,
-        "lastViolationValue": MetricValueOutputTypeDef,
+        "behavior": BehaviorTypeDef,
+        "lastViolationValue": MetricValueTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
+_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSecurityProfileRequestRequestTypeDef(
+    _RequiredCreateSecurityProfileRequestRequestTypeDef,
+    _OptionalCreateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorOutputTypeDef],
+        "behaviors": List[BehaviorTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileName": str,
+    },
+)
+_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
+    {
+        "securityProfileDescription": str,
+        "behaviors": Sequence[BehaviorTypeDef],
+        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
+        "additionalMetricsToRetain": Sequence[str],
+        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
+        "deleteBehaviors": bool,
+        "deleteAlertTargets": bool,
+        "deleteAdditionalMetricsToRetain": bool,
+        "expectedVersion": int,
+    },
+    total=False,
+)
+
+class UpdateSecurityProfileRequestRequestTypeDef(
+    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
+    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
+):
+    pass
+
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
-        "behaviors": List[BehaviorOutputTypeDef],
+        "behaviors": List[BehaviorTypeDef],
         "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
         "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    {
+        "behaviors": Sequence[BehaviorTypeDef],
+    },
+)
+
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorOutputTypeDef,
-        "metricValue": MetricValueOutputTypeDef,
+        "behavior": BehaviorTypeDef,
+        "metricValue": MetricValueTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "violationEventType": ViolationEventTypeType,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "violationEventTime": datetime,
     },
     total=False,
 )
 
-BehaviorUnionTypeDef = Union[BehaviorTypeDef, BehaviorOutputTypeDef]
-CodeSigningOutputTypeDef = TypedDict(
-    "CodeSigningOutputTypeDef",
-    {
-        "awsSignerJobId": str,
-        "startSigningJobParameter": StartSigningJobParameterTypeDef,
-        "customCodeSigning": CustomCodeSigningOutputTypeDef,
-    },
-    total=False,
-)
-
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
@@ -9350,17 +8923,17 @@
         "jobTemplateId": str,
         "description": str,
         "documentSource": str,
         "document": str,
         "createdAt": datetime,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
+        "abortConfig": AbortConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "maintenanceWindows": List[MaintenanceWindowTypeDef],
         "destinationPackageVersions": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobTypeDef = TypedDict(
@@ -9373,26 +8946,26 @@
         "forceCanceled": bool,
         "reasonCode": str,
         "comment": str,
         "targets": List[str],
         "description": str,
         "presignedUrlConfig": PresignedUrlConfigTypeDef,
         "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
+        "abortConfig": AbortConfigTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "completedAt": datetime,
         "jobProcessDetails": JobProcessDetailsTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "namespaceId": str,
         "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
         "documentParameters": Dict[str, str],
         "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "schedulingConfig": SchedulingConfigTypeDef,
         "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
         "destinationPackageVersions": List[str],
     },
     total=False,
 )
 
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
@@ -9431,30 +9004,30 @@
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
+        "target": AuditMitigationActionsTaskTargetTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
@@ -9499,44 +9072,14 @@
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "dynamoDB": DynamoDBActionTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionTypeDef,
-        "lambda": LambdaActionTypeDef,
-        "sns": SnsActionTypeDef,
-        "sqs": SqsActionTypeDef,
-        "kinesis": KinesisActionTypeDef,
-        "republish": RepublishActionOutputTypeDef,
-        "s3": S3ActionTypeDef,
-        "firehose": FirehoseActionTypeDef,
-        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
-        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
-        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
-        "elasticsearch": ElasticsearchActionTypeDef,
-        "salesforce": SalesforceActionTypeDef,
-        "iotAnalytics": IotAnalyticsActionTypeDef,
-        "iotEvents": IotEventsActionTypeDef,
-        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-        "stepFunctions": StepFunctionsActionTypeDef,
-        "timestream": TimestreamActionOutputTypeDef,
-        "http": HttpActionOutputTypeDef,
-        "kafka": KafkaActionOutputTypeDef,
-        "openSearch": OpenSearchActionTypeDef,
-        "location": LocationActionTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9577,87 +9120,14 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSecurityProfileRequestRequestTypeDef(
-    _RequiredCreateSecurityProfileRequestRequestTypeDef,
-    _OptionalCreateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileName": str,
-    },
-)
-_OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityProfileRequestRequestTypeDef",
-    {
-        "securityProfileDescription": str,
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-        "alertTargets": Mapping[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": Sequence[str],
-        "additionalMetricsToRetainV2": Sequence[MetricToRetainTypeDef],
-        "deleteBehaviors": bool,
-        "deleteAlertTargets": bool,
-        "deleteAdditionalMetricsToRetain": bool,
-        "expectedVersion": int,
-    },
-    total=False,
-)
-
-class UpdateSecurityProfileRequestRequestTypeDef(
-    _RequiredUpdateSecurityProfileRequestRequestTypeDef,
-    _OptionalUpdateSecurityProfileRequestRequestTypeDef,
-):
-    pass
-
-ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
-    {
-        "behaviors": Sequence[BehaviorUnionTypeDef],
-    },
-)
-
-OTAUpdateFileOutputTypeDef = TypedDict(
-    "OTAUpdateFileOutputTypeDef",
-    {
-        "fileName": str,
-        "fileType": int,
-        "fileVersion": str,
-        "fileLocation": FileLocationTypeDef,
-        "codeSigning": CodeSigningOutputTypeDef,
-        "attributes": Dict[str, str],
-    },
-    total=False,
-)
-
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -9706,48 +9176,78 @@
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredTopicRulePayloadTypeDef = TypedDict(
+    "_RequiredTopicRulePayloadTypeDef",
+    {
+        "sql": str,
+        "actions": Sequence[ActionTypeDef],
+    },
+)
+_OptionalTopicRulePayloadTypeDef = TypedDict(
+    "_OptionalTopicRulePayloadTypeDef",
+    {
+        "description": str,
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionTypeDef,
+    },
+    total=False,
+)
+
+class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
+    pass
+
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
         "sql": str,
         "description": str,
         "createdAt": datetime,
-        "actions": List[ActionOutputTypeDef],
+        "actions": List[ActionTypeDef],
         "ruleDisabled": bool,
         "awsIotSqlVersion": str,
-        "errorAction": ActionOutputTypeDef,
+        "errorAction": ActionTypeDef,
     },
     total=False,
 )
 
-_RequiredTopicRulePayloadTypeDef = TypedDict(
-    "_RequiredTopicRulePayloadTypeDef",
+_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
-        "sql": str,
-        "actions": Sequence[ActionTypeDef],
+        "otaUpdateId": str,
+        "targets": Sequence[str],
+        "files": Sequence[OTAUpdateFileTypeDef],
+        "roleArn": str,
     },
 )
-_OptionalTopicRulePayloadTypeDef = TypedDict(
-    "_OptionalTopicRulePayloadTypeDef",
+_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
     {
         "description": str,
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "protocols": Sequence[ProtocolType],
+        "targetSelection": TargetSelectionType,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
+        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
+        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
+        "additionalParameters": Mapping[str, str],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
+class CreateOTAUpdateRequestRequestTypeDef(
+    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
+):
     pass
 
 OTAUpdateInfoTypeDef = TypedDict(
     "OTAUpdateInfoTypeDef",
     {
         "otaUpdateId": str,
         "otaUpdateArn": str,
@@ -9755,34 +9255,24 @@
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
         "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
         "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
+        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
-OTAUpdateFileUnionTypeDef = Union[OTAUpdateFileTypeDef, OTAUpdateFileOutputTypeDef]
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
-    {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
@@ -9803,44 +9293,23 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetOTAUpdateResponseTypeDef = TypedDict(
-    "GetOTAUpdateResponseTypeDef",
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
     {
-        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOTAUpdateRequestRequestTypeDef",
-    {
-        "otaUpdateId": str,
-        "targets": Sequence[str],
-        "files": Sequence[OTAUpdateFileUnionTypeDef],
-        "roleArn": str,
-    },
-)
-_OptionalCreateOTAUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOTAUpdateRequestRequestTypeDef",
+GetOTAUpdateResponseTypeDef = TypedDict(
+    "GetOTAUpdateResponseTypeDef",
     {
-        "description": str,
-        "protocols": Sequence[ProtocolType],
-        "targetSelection": TargetSelectionType,
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "awsJobAbortConfig": AwsJobAbortConfigTypeDef,
-        "awsJobTimeoutConfig": AwsJobTimeoutConfigTypeDef,
-        "additionalParameters": Mapping[str, str],
-        "tags": Sequence[TagTypeDef],
+        "otaUpdateInfo": OTAUpdateInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-class CreateOTAUpdateRequestRequestTypeDef(
-    _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-iot-2.5.2.post1/types_aiobotocore_iot.egg-info/SOURCES.txt` & `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

