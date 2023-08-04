# Comparing `tmp/types-aiobotocore-config-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-config-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-config-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-config-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
```

## Comparing `types-aiobotocore-config-2.5.2.post1.tar` & `types-aiobotocore-config-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.061613 types-aiobotocore-config-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    38077 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.061613 types-aiobotocore-config-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:35:35.000000 types-aiobotocore-config-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92772 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92640 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-08-02 14:35:37.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-08-02 14:35:37.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44399 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   136691 2023-08-02 14:35:40.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   136524 2023-08-02 14:35:39.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38077 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.655732 types-aiobotocore-config-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18131 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.655732 types-aiobotocore-config-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:42:53.000000 types-aiobotocore-config-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92692 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92560 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44399 2023-08-04 11:42:55.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   128018 2023-08-04 11:42:58.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127867 2023-08-04 11:42:57.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:54.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.647732 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19652 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:41.000000 types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-config-2.5.2.post1/LICENSE` & `types-aiobotocore-config-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/setup.py` & `types-aiobotocore-config-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-config",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConfigService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.pyi` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__main__.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConfigService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceUnionTypeDef,
+    AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleUnionTypeDef,
-    ConfigurationRecorderUnionTypeDef,
+    ConfigRuleTypeDef,
+    ConfigurationRecorderTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -106,15 +106,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationUnionTypeDef,
+    EvaluationTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -133,30 +133,30 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceUnionTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataUnionTypeDef,
-    OrganizationManagedRuleMetadataUnionTypeDef,
+    OrganizationCustomRuleMetadataTypeDef,
+    OrganizationManagedRuleMetadataTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationUnionTypeDef,
+    RemediationConfigurationTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
@@ -1164,42 +1164,42 @@
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_aggregation_authorization)
         """
 
     async def put_config_rule(
-        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_config_rule)
         """
 
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_aggregator)
         """
 
     async def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
+        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_recorder)
@@ -1234,15 +1234,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_delivery_channel)
         """
 
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
+        Evaluations: Sequence[EvaluationTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
@@ -1258,16 +1258,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_external_evaluation)
         """
 
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1291,15 +1291,15 @@
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
         """
 
     async def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_configurations)
```

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.pyi` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,24 +61,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceUnionTypeDef,
+    AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleUnionTypeDef,
-    ConfigurationRecorderUnionTypeDef,
+    ConfigRuleTypeDef,
+    ConfigurationRecorderTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -106,15 +106,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationUnionTypeDef,
+    EvaluationTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -133,30 +133,30 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceUnionTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataUnionTypeDef,
-    OrganizationManagedRuleMetadataUnionTypeDef,
+    OrganizationCustomRuleMetadataTypeDef,
+    OrganizationManagedRuleMetadataTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationUnionTypeDef,
+    RemediationConfigurationTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
@@ -1087,40 +1087,40 @@
         Authorizes the aggregator account and region to collect data from the source
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_aggregation_authorization)
         """
     async def put_config_rule(
-        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_config_rule)
         """
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_aggregator)
         """
     async def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
+        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_recorder)
@@ -1152,15 +1152,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_delivery_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_delivery_channel)
         """
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
+        Evaluations: Sequence[EvaluationTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
@@ -1174,16 +1174,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_external_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_external_evaluation)
         """
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1205,15 +1205,15 @@
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
         """
     async def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_configurations)
```

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.pyi` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.pyi` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.py` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_config.type_defs import AccountAggregationSourceOutputTypeDef
+    from types_aiobotocore_config.type_defs import AccountAggregationSourceTypeDef
 
-    data: AccountAggregationSourceOutputTypeDef = ...
+    data: AccountAggregationSourceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -54,15 +54,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
@@ -72,19 +71,18 @@
     "ResourceKeyTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
     "EvaluationModeConfigurationTypeDef",
-    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceOutputTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
     "ConformancePackInputParameterTypeDef",
@@ -132,19 +130,17 @@
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EvaluationContextTypeDef",
-    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "TimestampTypeDef",
-    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
@@ -167,36 +163,31 @@
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
-    "OrganizationCustomRuleMetadataOutputTypeDef",
-    "OrganizationManagedRuleMetadataOutputTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
-    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
@@ -272,15 +263,14 @@
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
-    "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "EvaluationTypeDef",
     "ExternalEvaluationTypeDef",
     "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
     "TimeWindowTypeDef",
@@ -301,29 +291,23 @@
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
-    "OrganizationCustomRuleMetadataUnionTypeDef",
-    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
-    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
-    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -338,85 +322,57 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
-    "EvaluationUnionTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "PutEvaluationsResponseTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
-    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
-    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
-    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "RemediationConfigurationUnionTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
     "DescribeConfigRulesResponseTypeDef",
-    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-)
-
-_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
-    "_RequiredAccountAggregationSourceOutputTypeDef",
-    {
-        "AccountIds": List[str],
-    },
-)
-_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
-    "_OptionalAccountAggregationSourceOutputTypeDef",
-    {
-        "AllAwsRegions": bool,
-        "AwsRegions": List[str],
-    },
-    total=False,
 )
 
-
-class AccountAggregationSourceOutputTypeDef(
-    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
-):
-    pass
-
-
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": Sequence[str],
+        "AccountIds": List[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": Sequence[str],
+        "AwsRegions": List[str],
     },
     total=False,
 )
 
 
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
@@ -621,29 +577,18 @@
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "ComplianceResourceTypes": List[str],
-        "TagKey": str,
-        "TagValue": str,
-        "ComplianceResourceId": str,
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": Sequence[str],
+        "ComplianceResourceTypes": List[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
@@ -662,33 +607,32 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceOutputTypeDef",
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceOutputTypeDef",
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
 
-class OrganizationAggregationSourceOutputTypeDef(
-    _RequiredOrganizationAggregationSourceOutputTypeDef,
-    _OptionalOrganizationAggregationSourceOutputTypeDef,
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
 ):
     pass
 
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
@@ -1284,36 +1228,14 @@
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
-_RequiredEvaluationOutputTypeDef = TypedDict(
-    "_RequiredEvaluationOutputTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": datetime,
-    },
-)
-_OptionalEvaluationOutputTypeDef = TypedDict(
-    "_OptionalEvaluationOutputTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-
-class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
-    pass
-
-
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1337,26 +1259,18 @@
 
 
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
 
 TimestampTypeDef = Union[datetime, str]
-ExclusionByResourceTypesOutputTypeDef = TypedDict(
-    "ExclusionByResourceTypesOutputTypeDef",
-    {
-        "resourceTypes": List[ResourceTypeType],
-    },
-    total=False,
-)
-
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": Sequence[ResourceTypeType],
+        "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
@@ -1764,36 +1678,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
-    {
-        "RoleArn": str,
-    },
-)
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
-    {
-        "AwsRegions": Sequence[str],
-        "AllAwsRegions": bool,
-    },
-    total=False,
-)
-
-
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
-):
-    pass
-
-
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -1803,67 +1695,65 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
 
-class OrganizationCustomRuleMetadataOutputTypeDef(
-    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
-    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
 ):
     pass
 
 
-_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
 
-class OrganizationManagedRuleMetadataOutputTypeDef(
-    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
-    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
 
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
@@ -1891,69 +1781,14 @@
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
-    {
-        "LambdaFunctionArn": str,
-        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
-    },
-)
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
-    {
-        "Description": str,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ResourceTypesScope": Sequence[str],
-        "ResourceIdScope": str,
-        "TagKeyScope": str,
-        "TagValueScope": str,
-    },
-    total=False,
-)
-
-
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
-):
-    pass
-
-
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
-    {
-        "RuleIdentifier": str,
-    },
-)
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
-    {
-        "Description": str,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ResourceTypesScope": Sequence[str],
-        "ResourceIdScope": str,
-        "TagKeyScope": str,
-        "TagValueScope": str,
-    },
-    total=False,
-)
-
-
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
-):
-    pass
-
-
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2005,25 +1840,18 @@
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
-StaticValueOutputTypeDef = TypedDict(
-    "StaticValueOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
@@ -2107,17 +1935,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AccountAggregationSourceUnionTypeDef = Union[
-    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
-]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2473,16 +2298,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -3235,22 +3060,14 @@
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
-    {
-        "FailedEvaluations": List[EvaluationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
@@ -3716,14 +3533,38 @@
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
@@ -3745,49 +3586,40 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-OrganizationAggregationSourceUnionTypeDef = Union[
-    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
-]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
 _OptionalOrganizationConfigRuleTypeDef = TypedDict(
     "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
 
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
 
-OrganizationCustomRuleMetadataUnionTypeDef = Union[
-    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
-]
-OrganizationManagedRuleMetadataUnionTypeDef = Union[
-    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
-]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3805,32 +3637,20 @@
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 
-RecordingGroupOutputTypeDef = TypedDict(
-    "RecordingGroupOutputTypeDef",
-    {
-        "allSupported": bool,
-        "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
-        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
-        "recordingStrategy": RecordingStrategyTypeDef,
-    },
-    total=False,
-)
-
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": Sequence[ResourceTypeType],
+        "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
@@ -3841,98 +3661,44 @@
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-RemediationParameterValueOutputTypeDef = TypedDict(
-    "RemediationParameterValueOutputTypeDef",
-    {
-        "ResourceValue": ResourceValueTypeDef,
-        "StaticValue": StaticValueOutputTypeDef,
-    },
-    total=False,
-)
-
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-_RequiredSourceOutputTypeDef = TypedDict(
-    "_RequiredSourceOutputTypeDef",
-    {
-        "Owner": OwnerType,
-    },
-)
-_OptionalSourceOutputTypeDef = TypedDict(
-    "_OptionalSourceOutputTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
-        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
-    },
-    total=False,
-)
-
-
-class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
-    pass
-
-
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": Sequence[SourceDetailTypeDef],
+        "SourceDetails": List[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4144,15 +3910,44 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
-EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutExternalEvaluationRequestRequestTypeDef = TypedDict(
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
@@ -4192,24 +3987,14 @@
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationRecorderOutputTypeDef = TypedDict(
-    "ConfigurationRecorderOutputTypeDef",
-    {
-        "name": str,
-        "roleARN": str,
-        "recordingGroup": RecordingGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
         "recordingGroup": RecordingGroupTypeDef,
     },
@@ -4221,58 +4006,27 @@
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRemediationConfigurationOutputTypeDef",
-    {
-        "ConfigRuleName": str,
-        "TargetType": Literal["SSM_DOCUMENT"],
-        "TargetId": str,
-    },
-)
-_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRemediationConfigurationOutputTypeDef",
-    {
-        "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
-        "ResourceType": str,
-        "Automatic": bool,
-        "ExecutionControls": ExecutionControlsTypeDef,
-        "MaximumAutomaticAttempts": int,
-        "RetryAttemptSeconds": int,
-        "Arn": str,
-        "CreatedByService": str,
-    },
-    total=False,
-)
-
-
-class RemediationConfigurationOutputTypeDef(
-    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
+        "Parameters": Dict[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
@@ -4283,42 +4037,14 @@
 
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
 
-_RequiredConfigRuleOutputTypeDef = TypedDict(
-    "_RequiredConfigRuleOutputTypeDef",
-    {
-        "Source": SourceOutputTypeDef,
-    },
-)
-_OptionalConfigRuleOutputTypeDef = TypedDict(
-    "_OptionalConfigRuleOutputTypeDef",
-    {
-        "ConfigRuleName": str,
-        "ConfigRuleArn": str,
-        "ConfigRuleId": str,
-        "Description": str,
-        "Scope": ScopeOutputTypeDef,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ConfigRuleState": ConfigRuleStateType,
-        "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
-    },
-    total=False,
-)
-
-
-class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
-    pass
-
-
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4329,15 +4055,15 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
@@ -4421,36 +4147,14 @@
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
-    {
-        "ResultToken": str,
-    },
-)
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
-    {
-        "Evaluations": Sequence[EvaluationUnionTypeDef],
-        "TestMode": bool,
-    },
-    total=False,
-)
-
-
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
-):
-    pass
-
-
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4465,59 +4169,59 @@
     },
     total=False,
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
+        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationRecorderUnionTypeDef = Union[
-    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
-]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
+        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationOutputTypeDef],
+        "FailedItems": List[RemediationConfigurationTypeDef],
     },
     total=False,
 )
 
-RemediationConfigurationUnionTypeDef = Union[
-    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
-]
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
+    },
+)
+
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleOutputTypeDef],
+        "ConfigRules": List[ConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
@@ -4538,14 +4242,7 @@
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.pyi` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_config.type_defs import AccountAggregationSourceOutputTypeDef
+    from types_aiobotocore_config.type_defs import AccountAggregationSourceTypeDef
 
-    data: AccountAggregationSourceOutputTypeDef = ...
+    data: AccountAggregationSourceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -53,15 +53,14 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
@@ -71,19 +70,18 @@
     "ResourceKeyTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
     "EvaluationModeConfigurationTypeDef",
-    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceOutputTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
     "ConformancePackInputParameterTypeDef",
@@ -131,19 +129,17 @@
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
     "EvaluationContextTypeDef",
-    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
     "TimestampTypeDef",
-    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
     "FieldInfoTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
@@ -166,36 +162,31 @@
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
-    "OrganizationCustomRuleMetadataOutputTypeDef",
-    "OrganizationManagedRuleMetadataOutputTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
-    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigResponseTypeDef",
@@ -271,15 +262,14 @@
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
-    "PutEvaluationsResponseTypeDef",
     "EvaluationResultIdentifierTypeDef",
     "EvaluationTypeDef",
     "ExternalEvaluationTypeDef",
     "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     "GetResourceConfigHistoryRequestRequestTypeDef",
     "PutRemediationExceptionsRequestRequestTypeDef",
     "TimeWindowTypeDef",
@@ -300,29 +290,23 @@
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
-    "OrganizationCustomRuleMetadataUnionTypeDef",
-    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
-    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
-    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -337,83 +321,57 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
-    "EvaluationUnionTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "PutEvaluationsResponseTypeDef",
     "PutExternalEvaluationRequestRequestTypeDef",
     "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
-    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
-    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
-    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "RemediationConfigurationUnionTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
     "DescribeConfigRulesResponseTypeDef",
-    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
 )
 
-_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
-    "_RequiredAccountAggregationSourceOutputTypeDef",
-    {
-        "AccountIds": List[str],
-    },
-)
-_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
-    "_OptionalAccountAggregationSourceOutputTypeDef",
-    {
-        "AllAwsRegions": bool,
-        "AwsRegions": List[str],
-    },
-    total=False,
-)
-
-class AccountAggregationSourceOutputTypeDef(
-    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
-):
-    pass
-
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": Sequence[str],
+        "AccountIds": List[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": Sequence[str],
+        "AwsRegions": List[str],
     },
     total=False,
 )
 
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
@@ -614,29 +572,18 @@
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "ComplianceResourceTypes": List[str],
-        "TagKey": str,
-        "TagValue": str,
-        "ComplianceResourceId": str,
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": Sequence[str],
+        "ComplianceResourceTypes": List[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
@@ -655,32 +602,31 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceOutputTypeDef",
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceOutputTypeDef",
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-class OrganizationAggregationSourceOutputTypeDef(
-    _RequiredOrganizationAggregationSourceOutputTypeDef,
-    _OptionalOrganizationAggregationSourceOutputTypeDef,
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
 ):
     pass
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -1259,34 +1205,14 @@
     "EvaluationContextTypeDef",
     {
         "EvaluationContextIdentifier": str,
     },
     total=False,
 )
 
-_RequiredEvaluationOutputTypeDef = TypedDict(
-    "_RequiredEvaluationOutputTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": datetime,
-    },
-)
-_OptionalEvaluationOutputTypeDef = TypedDict(
-    "_OptionalEvaluationOutputTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
-    pass
-
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1308,26 +1234,18 @@
     total=False,
 )
 
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
 TimestampTypeDef = Union[datetime, str]
-ExclusionByResourceTypesOutputTypeDef = TypedDict(
-    "ExclusionByResourceTypesOutputTypeDef",
-    {
-        "resourceTypes": List[ResourceTypeType],
-    },
-    total=False,
-)
-
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": Sequence[ResourceTypeType],
+        "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
@@ -1715,34 +1633,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
-    {
-        "RoleArn": str,
-    },
-)
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
-    {
-        "AwsRegions": Sequence[str],
-        "AllAwsRegions": bool,
-    },
-    total=False,
-)
-
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
-):
-    pass
-
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -1752,64 +1650,62 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationCustomRuleMetadataOutputTypeDef(
-    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
-    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
 ):
     pass
 
-_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationManagedRuleMetadataOutputTypeDef(
-    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
-    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
 ):
     pass
 
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
@@ -1834,65 +1730,14 @@
 
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
-    {
-        "LambdaFunctionArn": str,
-        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
-    },
-)
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
-    {
-        "Description": str,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ResourceTypesScope": Sequence[str],
-        "ResourceIdScope": str,
-        "TagKeyScope": str,
-        "TagValueScope": str,
-    },
-    total=False,
-)
-
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
-):
-    pass
-
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
-    {
-        "RuleIdentifier": str,
-    },
-)
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
-    {
-        "Description": str,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ResourceTypesScope": Sequence[str],
-        "ResourceIdScope": str,
-        "TagKeyScope": str,
-        "TagValueScope": str,
-    },
-    total=False,
-)
-
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
-):
-    pass
-
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -1942,25 +1787,18 @@
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
-StaticValueOutputTypeDef = TypedDict(
-    "StaticValueOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
 StaticValueTypeDef = TypedDict(
     "StaticValueTypeDef",
     {
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
@@ -2040,17 +1878,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AccountAggregationSourceUnionTypeDef = Union[
-    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
-]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2396,16 +2231,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -3122,22 +2957,14 @@
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
-    {
-        "FailedEvaluations": List[EvaluationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
@@ -3575,14 +3402,36 @@
 
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
+
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
@@ -3602,47 +3451,38 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-OrganizationAggregationSourceUnionTypeDef = Union[
-    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
-]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
 _OptionalOrganizationConfigRuleTypeDef = TypedDict(
     "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
-OrganizationCustomRuleMetadataUnionTypeDef = Union[
-    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
-]
-OrganizationManagedRuleMetadataUnionTypeDef = Union[
-    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
-]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3658,32 +3498,20 @@
 
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-RecordingGroupOutputTypeDef = TypedDict(
-    "RecordingGroupOutputTypeDef",
-    {
-        "allSupported": bool,
-        "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
-        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
-        "recordingStrategy": RecordingStrategyTypeDef,
-    },
-    total=False,
-)
-
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": Sequence[ResourceTypeType],
+        "resourceTypes": List[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
@@ -3694,92 +3522,42 @@
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-RemediationParameterValueOutputTypeDef = TypedDict(
-    "RemediationParameterValueOutputTypeDef",
-    {
-        "ResourceValue": ResourceValueTypeDef,
-        "StaticValue": StaticValueOutputTypeDef,
-    },
-    total=False,
-)
-
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-_RequiredSourceOutputTypeDef = TypedDict(
-    "_RequiredSourceOutputTypeDef",
-    {
-        "Owner": OwnerType,
-    },
-)
-_OptionalSourceOutputTypeDef = TypedDict(
-    "_OptionalSourceOutputTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
-        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
-    },
-    total=False,
-)
-
-class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
-    pass
-
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": Sequence[SourceDetailTypeDef],
+        "SourceDetails": List[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3989,15 +3767,42 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
-EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutExternalEvaluationRequestRequestTypeDef = TypedDict(
     "PutExternalEvaluationRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
         "ExternalEvaluation": ExternalEvaluationTypeDef,
     },
 )
@@ -4037,24 +3842,14 @@
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationRecorderOutputTypeDef = TypedDict(
-    "ConfigurationRecorderOutputTypeDef",
-    {
-        "name": str,
-        "roleARN": str,
-        "recordingGroup": RecordingGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
         "recordingGroup": RecordingGroupTypeDef,
     },
@@ -4066,56 +3861,27 @@
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRemediationConfigurationOutputTypeDef",
-    {
-        "ConfigRuleName": str,
-        "TargetType": Literal["SSM_DOCUMENT"],
-        "TargetId": str,
-    },
-)
-_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRemediationConfigurationOutputTypeDef",
-    {
-        "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
-        "ResourceType": str,
-        "Automatic": bool,
-        "ExecutionControls": ExecutionControlsTypeDef,
-        "MaximumAutomaticAttempts": int,
-        "RetryAttemptSeconds": int,
-        "Arn": str,
-        "CreatedByService": str,
-    },
-    total=False,
-)
-
-class RemediationConfigurationOutputTypeDef(
-    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
+        "Parameters": Dict[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
@@ -4124,40 +3890,14 @@
 )
 
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
-_RequiredConfigRuleOutputTypeDef = TypedDict(
-    "_RequiredConfigRuleOutputTypeDef",
-    {
-        "Source": SourceOutputTypeDef,
-    },
-)
-_OptionalConfigRuleOutputTypeDef = TypedDict(
-    "_OptionalConfigRuleOutputTypeDef",
-    {
-        "ConfigRuleName": str,
-        "ConfigRuleArn": str,
-        "ConfigRuleId": str,
-        "Description": str,
-        "Scope": ScopeOutputTypeDef,
-        "InputParameters": str,
-        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
-        "ConfigRuleState": ConfigRuleStateType,
-        "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
-    },
-    total=False,
-)
-
-class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
-    pass
-
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4168,15 +3908,15 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
@@ -4258,34 +3998,14 @@
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
-    {
-        "ResultToken": str,
-    },
-)
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
-    {
-        "Evaluations": Sequence[EvaluationUnionTypeDef],
-        "TestMode": bool,
-    },
-    total=False,
-)
-
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
-):
-    pass
-
 ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
     "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
     {
         "Filters": ResourceEvaluationFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4300,59 +4020,59 @@
     },
     total=False,
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
+        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationRecorderUnionTypeDef = Union[
-    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
-]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
+        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationOutputTypeDef],
+        "FailedItems": List[RemediationConfigurationTypeDef],
     },
     total=False,
 )
 
-RemediationConfigurationUnionTypeDef = Union[
-    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
-]
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
+    },
+)
+
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleOutputTypeDef],
+        "ConfigRules": List[ConfigRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
@@ -4371,14 +4091,7 @@
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/SOURCES.txt` & `types-aiobotocore-config-2.5.2.post2/types_aiobotocore_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

