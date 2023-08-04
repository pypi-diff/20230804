# Comparing `tmp/types-aiobotocore-resiliencehub-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-resiliencehub-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-resiliencehub-2.5.2.post1.tar` & `types-aiobotocore-resiliencehub-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.637482 types-aiobotocore-resiliencehub-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.637482 types-aiobotocore-resiliencehub-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41871 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41811 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-08-02 14:47:50.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61091 2023-08-02 14:47:53.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60986 2023-08-02 14:47:53.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12500 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10958 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:50:41.000000 types-aiobotocore-resiliencehub-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      490 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      489 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43867 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43805 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11692 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11690 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    67894 2023-08-04 13:50:44.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    67775 2023-08-04 13:50:43.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12500 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      836 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/LICENSE` & `types-aiobotocore-resiliencehub-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/setup.py` & `types-aiobotocore-resiliencehub-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resiliencehub",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__main__.py` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ResilienceHub 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.py` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -52,18 +53,20 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceUnionTypeDef,
+    EksSourceTypeDef,
+    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -73,25 +76,28 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
+    PermissionModelTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -136,14 +142,27 @@
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
+    async def batch_update_recommendation_status(
+        self,
+        *,
+        appArn: str,
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
+        """
+        Enables you to include or exclude one or more operational recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#can_paginate)
         """
@@ -159,14 +178,16 @@
     async def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -445,15 +466,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#generate_presigned_url)
         """
 
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
+        eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
@@ -468,14 +489,24 @@
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_alarm_recommendations)
         """
 
+    async def list_app_assessment_compliance_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
+        """
+        List of compliance drifts that were detected while running an assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessment_compliance_drifts)
+        """
+
     async def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -554,15 +585,21 @@
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
 
     async def list_app_versions(
-        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        appArn: str,
+        endTime: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startTime: TimestampTypeDef = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -658,15 +695,17 @@
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
 
-    async def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
+    async def publish_app_version(
+        self, *, appArn: str, versionName: str = ...
+    ) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#publish_app_version)
         """
 
@@ -744,14 +783,16 @@
     async def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -52,18 +53,20 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceUnionTypeDef,
+    EksSourceTypeDef,
+    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -73,25 +76,28 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
+    PermissionModelTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -131,14 +137,26 @@
     ) -> AddDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
+    async def batch_update_recommendation_status(
+        self,
+        *,
+        appArn: str,
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
+        """
+        Enables you to include or exclude one or more operational recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#can_paginate)
         """
@@ -152,14 +170,16 @@
     async def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -416,15 +436,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#generate_presigned_url)
         """
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
+        eksSources: Sequence[EksSourceTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
@@ -437,14 +457,23 @@
     ) -> ListAlarmRecommendationsResponseTypeDef:
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_alarm_recommendations)
         """
+    async def list_app_assessment_compliance_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
+        """
+        List of compliance drifts that were detected while running an assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessment_compliance_drifts)
+        """
     async def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -516,15 +545,21 @@
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
     async def list_app_versions(
-        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        appArn: str,
+        endTime: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startTime: TimestampTypeDef = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -611,15 +646,17 @@
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
-    async def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
+    async def publish_app_version(
+        self, *, appArn: str, versionName: str = ...
+    ) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#publish_app_version)
         """
     async def put_draft_app_version_template(
@@ -690,14 +727,16 @@
     async def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.py` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,31 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
+    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
+    "DifferenceTypeType",
     "DisruptionTypeType",
+    "DriftStatusType",
+    "DriftTypeType",
     "EstimatedCostTierType",
+    "EventTypeType",
+    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -55,41 +62,50 @@
 
 
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
+AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
+DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
+DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
+DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
+EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
+ExcludeRecommendationReasonType = Literal[
+    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
+]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
@@ -110,14 +126,15 @@
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
@@ -213,14 +230,15 @@
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
@@ -299,26 +317,28 @@
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,31 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
+    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
+    "DifferenceTypeType",
     "DisruptionTypeType",
+    "DriftStatusType",
+    "DriftTypeType",
     "EstimatedCostTierType",
+    "EventTypeType",
+    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -53,41 +60,50 @@
 )
 
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
+AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
+DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
+DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
+DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
+EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
+ExcludeRecommendationReasonType = Literal[
+    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
+]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
@@ -108,14 +124,15 @@
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
@@ -211,14 +228,15 @@
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
@@ -297,26 +315,28 @@
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.py` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,29 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
+    DriftStatusType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -60,18 +65,20 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "AppTypeDef",
+    "EventSubscriptionTypeDef",
+    "PermissionModelTypeDef",
     "AppVersionSummaryTypeDef",
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
-    "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -81,25 +88,25 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
-    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
+    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -110,15 +117,14 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -131,56 +137,65 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
+    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
+    "AppTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "ListAppVersionsResponseTypeDef",
+    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "EksSourceUnionTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -205,14 +220,16 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
+        "excludeReason": ExcludeRecommendationReasonType,
+        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -308,107 +325,130 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
+        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
+_RequiredEventSubscriptionTypeDef = TypedDict(
+    "_RequiredEventSubscriptionTypeDef",
     {
-        "appArn": str,
-        "creationTime": datetime,
+        "eventType": EventTypeType,
         "name": str,
     },
 )
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
+_OptionalEventSubscriptionTypeDef = TypedDict(
+    "_OptionalEventSubscriptionTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
+        "snsTopicArn": str,
     },
     total=False,
 )
 
 
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+class EventSubscriptionTypeDef(
+    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
+):
     pass
 
 
-AppVersionSummaryTypeDef = TypedDict(
-    "AppVersionSummaryTypeDef",
+_RequiredPermissionModelTypeDef = TypedDict(
+    "_RequiredPermissionModelTypeDef",
     {
-        "appVersion": str,
+        "type": PermissionModelTypeType,
     },
 )
+_OptionalPermissionModelTypeDef = TypedDict(
+    "_OptionalPermissionModelTypeDef",
+    {
+        "crossAccountRoleArns": Sequence[str],
+        "invokerRoleName": str,
+    },
+    total=False,
+)
 
-_RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
-    "_RequiredRecommendationDisruptionComplianceTypeDef",
+
+class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
+    pass
+
+
+_RequiredAppVersionSummaryTypeDef = TypedDict(
+    "_RequiredAppVersionSummaryTypeDef",
     {
-        "expectedComplianceStatus": ComplianceStatusType,
+        "appVersion": str,
     },
 )
-_OptionalRecommendationDisruptionComplianceTypeDef = TypedDict(
-    "_OptionalRecommendationDisruptionComplianceTypeDef",
+_OptionalAppVersionSummaryTypeDef = TypedDict(
+    "_OptionalAppVersionSummaryTypeDef",
     {
-        "expectedRpoDescription": str,
-        "expectedRpoInSecs": int,
-        "expectedRtoDescription": str,
-        "expectedRtoInSecs": int,
+        "creationTime": datetime,
+        "identifier": int,
+        "versionName": str,
     },
     total=False,
 )
 
 
-class RecommendationDisruptionComplianceTypeDef(
-    _RequiredRecommendationDisruptionComplianceTypeDef,
-    _OptionalRecommendationDisruptionComplianceTypeDef,
+class AppVersionSummaryTypeDef(
+    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
 ):
     pass
 
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
+BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
     {
-        "name": str,
+        "entryId": str,
+        "errorMessage": str,
     },
 )
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+
+UpdateRecommendationStatusItemTypeDef = TypedDict(
+    "UpdateRecommendationStatusItemTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "policyArn": str,
-        "tags": Mapping[str, str],
+        "resourceId": str,
+        "targetAccountId": str,
+        "targetRegion": str,
     },
     total=False,
 )
 
+_RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
+    "_RequiredRecommendationDisruptionComplianceTypeDef",
+    {
+        "expectedComplianceStatus": ComplianceStatusType,
+    },
+)
+_OptionalRecommendationDisruptionComplianceTypeDef = TypedDict(
+    "_OptionalRecommendationDisruptionComplianceTypeDef",
+    {
+        "expectedRpoDescription": str,
+        "expectedRpoInSecs": int,
+        "expectedRtoDescription": str,
+        "expectedRtoInSecs": int,
+    },
+    total=False,
+)
 
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+
+class RecommendationDisruptionComplianceTypeDef(
+    _RequiredRecommendationDisruptionComplianceTypeDef,
+    _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
 
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
@@ -678,22 +718,14 @@
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
-EksSourceOutputTypeDef = TypedDict(
-    "EksSourceOutputTypeDef",
-    {
-        "eksClusterArn": str,
-        "namespaces": List[str],
-    },
-)
-
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
@@ -717,14 +749,37 @@
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+    },
+)
+_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
+    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+):
+    pass
+
+
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -875,36 +930,15 @@
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -1055,20 +1089,34 @@
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
 
-PublishAppVersionRequestRequestTypeDef = TypedDict(
-    "PublishAppVersionRequestRequestTypeDef",
+_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
+_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishAppVersionRequestRequestTypeDef",
+    {
+        "versionName": str,
+    },
+    total=False,
+)
+
+
+class PublishAppVersionRequestRequestTypeDef(
+    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
+):
+    pass
+
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1165,38 +1213,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "policyArn": str,
-    },
-    total=False,
-)
-
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1326,14 +1350,16 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
+        "identifier": int,
+        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1382,14 +1408,15 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
+        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1468,30 +1495,49 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
+        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
 
+ComplianceDriftTypeDef = TypedDict(
+    "ComplianceDriftTypeDef",
+    {
+        "actualReferenceId": str,
+        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+        "appId": str,
+        "appVersion": str,
+        "diffType": Literal["NotEqual"],
+        "driftType": Literal["ApplicationCompliance"],
+        "entityId": str,
+        "entityType": str,
+        "expectedReferenceId": str,
+        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+    },
+    total=False,
+)
+
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1605,47 +1651,159 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+        "creationTime": datetime,
+        "name": str,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "driftStatus": AppDriftStatusTypeType,
+        "eventSubscriptions": List[EventSubscriptionTypeDef],
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastDriftEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
+    total=False,
 )
 
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
     },
+    total=False,
 )
 
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
+
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+
+class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
+    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+):
+    pass
+
+
+_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+
+class UpdateRecommendationStatusRequestEntryTypeDef(
+    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
+    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
+):
+    pass
+
+
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -1852,28 +2010,76 @@
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceOutputTypeDef],
+        "eksSources": List[EksSourceTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2018,14 +2224,23 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
+    {
+        "complianceDrifts": List[ComplianceDriftTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2045,14 +2260,56 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
+        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
+    },
+)
+
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -2096,39 +2353,14 @@
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[EksSourceUnionTypeDef],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
-
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2242,21 +2474,23 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
+        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,29 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
+    DriftStatusType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -59,18 +64,20 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "AppTypeDef",
+    "EventSubscriptionTypeDef",
+    "PermissionModelTypeDef",
     "AppVersionSummaryTypeDef",
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
-    "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -80,25 +87,25 @@
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
-    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
+    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -109,15 +116,14 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -130,56 +136,65 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
+    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
+    "AppTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "ListAppVersionsResponseTypeDef",
+    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "EksSourceUnionTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -204,14 +219,16 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
+        "excludeReason": ExcludeRecommendationReasonType,
+        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -303,56 +320,100 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
+        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
+_RequiredEventSubscriptionTypeDef = TypedDict(
+    "_RequiredEventSubscriptionTypeDef",
     {
-        "appArn": str,
-        "creationTime": datetime,
+        "eventType": EventTypeType,
         "name": str,
     },
 )
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
+_OptionalEventSubscriptionTypeDef = TypedDict(
+    "_OptionalEventSubscriptionTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
+        "snsTopicArn": str,
     },
     total=False,
 )
 
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+class EventSubscriptionTypeDef(
+    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
+):
     pass
 
-AppVersionSummaryTypeDef = TypedDict(
-    "AppVersionSummaryTypeDef",
+_RequiredPermissionModelTypeDef = TypedDict(
+    "_RequiredPermissionModelTypeDef",
+    {
+        "type": PermissionModelTypeType,
+    },
+)
+_OptionalPermissionModelTypeDef = TypedDict(
+    "_OptionalPermissionModelTypeDef",
+    {
+        "crossAccountRoleArns": Sequence[str],
+        "invokerRoleName": str,
+    },
+    total=False,
+)
+
+class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
+    pass
+
+_RequiredAppVersionSummaryTypeDef = TypedDict(
+    "_RequiredAppVersionSummaryTypeDef",
     {
         "appVersion": str,
     },
 )
+_OptionalAppVersionSummaryTypeDef = TypedDict(
+    "_OptionalAppVersionSummaryTypeDef",
+    {
+        "creationTime": datetime,
+        "identifier": int,
+        "versionName": str,
+    },
+    total=False,
+)
+
+class AppVersionSummaryTypeDef(
+    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
+):
+    pass
+
+BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    {
+        "entryId": str,
+        "errorMessage": str,
+    },
+)
+
+UpdateRecommendationStatusItemTypeDef = TypedDict(
+    "UpdateRecommendationStatusItemTypeDef",
+    {
+        "resourceId": str,
+        "targetAccountId": str,
+        "targetRegion": str,
+    },
+    total=False,
+)
 
 _RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
     "_RequiredRecommendationDisruptionComplianceTypeDef",
     {
         "expectedComplianceStatus": ComplianceStatusType,
     },
 )
@@ -369,37 +430,14 @@
 
 class RecommendationDisruptionComplianceTypeDef(
     _RequiredRecommendationDisruptionComplianceTypeDef,
     _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "policyArn": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
         "type": str,
     },
@@ -647,22 +685,14 @@
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
-EksSourceOutputTypeDef = TypedDict(
-    "EksSourceOutputTypeDef",
-    {
-        "eksClusterArn": str,
-        "namespaces": List[str],
-    },
-)
-
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
@@ -684,14 +714,35 @@
 
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+    },
+)
+_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
+    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+):
+    pass
+
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -830,34 +881,15 @@
 
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -998,20 +1030,32 @@
 )
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
-PublishAppVersionRequestRequestTypeDef = TypedDict(
-    "PublishAppVersionRequestRequestTypeDef",
+_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
+_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishAppVersionRequestRequestTypeDef",
+    {
+        "versionName": str,
+    },
+    total=False,
+)
+
+class PublishAppVersionRequestRequestTypeDef(
+    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
+):
+    pass
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1104,36 +1148,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "policyArn": str,
-    },
-    total=False,
-)
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1259,14 +1281,16 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
+        "identifier": int,
+        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1315,14 +1339,15 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
+        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1395,28 +1420,47 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
+        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
+ComplianceDriftTypeDef = TypedDict(
+    "ComplianceDriftTypeDef",
+    {
+        "actualReferenceId": str,
+        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+        "appId": str,
+        "appVersion": str,
+        "diffType": Literal["NotEqual"],
+        "driftType": Literal["ApplicationCompliance"],
+        "entityId": str,
+        "entityType": str,
+        "expectedReferenceId": str,
+        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+    },
+    total=False,
+)
+
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1526,47 +1570,149 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+        "creationTime": datetime,
+        "name": str,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "driftStatus": AppDriftStatusTypeType,
+        "eventSubscriptions": List[EventSubscriptionTypeDef],
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastDriftEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
+    total=False,
 )
 
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
     },
+    total=False,
 )
 
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
+    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+):
+    pass
+
+_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+class UpdateRecommendationStatusRequestEntryTypeDef(
+    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
+    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
+):
+    pass
+
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -1759,28 +1905,72 @@
 
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceOutputTypeDef],
+        "eksSources": List[EksSourceTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -1917,14 +2107,23 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
+    {
+        "complianceDrifts": List[ComplianceDriftTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1944,14 +2143,56 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
+        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
+    },
+)
+
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -1995,37 +2236,14 @@
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[EksSourceUnionTypeDef],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2139,21 +2357,23 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
+        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt` & `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

