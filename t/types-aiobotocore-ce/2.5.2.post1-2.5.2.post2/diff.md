# Comparing `tmp/types-aiobotocore-ce-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ce-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ce-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-ce-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:30 2023, max compression
```

## Comparing `types-aiobotocore-ce-2.5.2.post1.tar` & `types-aiobotocore-ce-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33853 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66703 2023-08-02 14:33:58.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66630 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.959325 types-aiobotocore-ce-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-08-04 12:00:30.955325 types-aiobotocore-ce-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:30.959325 types-aiobotocore-ce-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.955325 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33821 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33775 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63392 2023-08-04 11:41:11.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63323 2023-08-04 11:41:10.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:09.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.955325 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:00:30.000000 types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ce-2.5.2.post1/LICENSE` & `types-aiobotocore-ce-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2.post1/setup.py` & `types-aiobotocore-ce-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ce",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__main__.py` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.py` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionUnionTypeDef,
+    AnomalySubscriptionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleUnionTypeDef,
+    CostCategorySplitChargeRuleTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionUnionTypeDef,
+    ExpressionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -167,15 +167,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
 
     async def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
+        AnomalySubscription: AnomalySubscriptionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
@@ -185,15 +185,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
@@ -299,15 +299,15 @@
 
     async def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
@@ -315,15 +315,15 @@
         """
 
     async def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef,
+        Filter: "ExpressionTypeDef",
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -333,15 +333,15 @@
 
     async def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -351,15 +351,15 @@
 
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -369,15 +369,15 @@
     async def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -388,15 +388,15 @@
 
     async def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -409,15 +409,15 @@
         """
 
     async def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -431,15 +431,15 @@
 
     async def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
@@ -447,15 +447,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
 
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -466,15 +466,15 @@
 
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -489,44 +489,44 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: ExpressionUnionTypeDef = ...
+        Filter: "ExpressionTypeDef" = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
 
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_utilization)
         """
 
     async def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -538,15 +538,15 @@
 
     async def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -556,15 +556,15 @@
 
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -680,15 +680,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: ExpressionUnionTypeDef = ...
+        ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly monitor subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -707,15 +707,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.pyi` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionUnionTypeDef,
+    AnomalySubscriptionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleUnionTypeDef,
+    CostCategorySplitChargeRuleTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionUnionTypeDef,
+    ExpressionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -159,15 +159,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
     async def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
+        AnomalySubscription: AnomalySubscriptionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
@@ -176,15 +176,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
@@ -281,30 +281,30 @@
         """
     async def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage)
         """
     async def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef,
+        Filter: "ExpressionTypeDef",
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -313,15 +313,15 @@
         """
     async def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -330,15 +330,15 @@
         """
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -347,15 +347,15 @@
     async def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -365,15 +365,15 @@
         """
     async def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -385,15 +385,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_coverage)
         """
     async def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -406,30 +406,30 @@
         """
     async def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -439,15 +439,15 @@
         """
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -461,42 +461,42 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: ExpressionUnionTypeDef = ...
+        Filter: "ExpressionTypeDef" = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_utilization)
         """
     async def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -507,15 +507,15 @@
         """
     async def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -524,15 +524,15 @@
         """
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: ExpressionUnionTypeDef = ...,
+        Filter: "ExpressionTypeDef" = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -638,15 +638,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: ExpressionUnionTypeDef = ...
+        ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly monitor subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -663,15 +663,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.py` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.pyi` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.py` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_ce.type_defs import AnomalyDateIntervalTypeDef
 
     data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -65,42 +65,37 @@
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
-    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
-    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
     "ResponseMetadataTypeDef",
-    "TagValuesOutputTypeDef",
+    "TagValuesTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
-    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
-    "TagValuesTypeDef",
-    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
@@ -125,22 +120,20 @@
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
-    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -154,20 +147,19 @@
     "ListCostAllocationTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvideAnomalyFeedbackResponseTypeDef",
     "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UpdateAnomalyMonitorResponseTypeDef",
     "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostCategoryDefinitionResponseTypeDef",
-    "ExpressionOutputTypeDef",
+    "ExpressionTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
-    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -182,36 +174,34 @@
     "InstanceDetailsTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "GetAnomalySubscriptionsResponseTypeDef",
-    "AnomalySubscriptionUnionTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
+    "GetAnomalySubscriptionsResponseTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CostCategorySplitChargeRuleUnionTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -353,40 +343,22 @@
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
     total=False,
 )
 
-CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
-    "CostCategorySplitChargeRuleParameterOutputTypeDef",
-    {
-        "Type": Literal["ALLOCATION_PERCENTAGES"],
-        "Values": List[str],
-    },
-)
-
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
-CostCategoryValuesOutputTypeDef = TypedDict(
-    "CostCategoryValuesOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
-    },
-    total=False,
-)
-
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -446,20 +418,20 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TagValuesOutputTypeDef = TypedDict(
-    "TagValuesOutputTypeDef",
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
     {
         "Key": str,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
@@ -499,24 +471,14 @@
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-DimensionValuesOutputTypeDef = TypedDict(
-    "DimensionValuesOutputTypeDef",
-    {
-        "Key": DimensionType,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
-    },
-    total=False,
-)
-
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -625,25 +587,14 @@
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
     total=False,
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
-    {
-        "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
-    },
-    total=False,
-)
-
-ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -1033,41 +984,14 @@
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
-    "_RequiredAnomalySubscriptionOutputTypeDef",
-    {
-        "MonitorArnList": List[str],
-        "Subscribers": List[SubscriberTypeDef],
-        "Frequency": AnomalySubscriptionFrequencyType,
-        "SubscriptionName": str,
-    },
-)
-_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
-    "_OptionalAnomalySubscriptionOutputTypeDef",
-    {
-        "SubscriptionArn": str,
-        "AccountId": str,
-        "Threshold": float,
-        "ThresholdExpression": "ExpressionOutputTypeDef",
-    },
-    total=False,
-)
-
-
-class AnomalySubscriptionOutputTypeDef(
-    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
-):
-    pass
-
-
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1173,38 +1097,14 @@
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
-    {
-        "Source": str,
-        "Targets": List[str],
-        "Method": CostCategorySplitChargeMethodType,
-    },
-)
-_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
-    {
-        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class CostCategorySplitChargeRuleOutputTypeDef(
-    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
-    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
-):
-    pass
-
-
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1445,23 +1345,23 @@
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExpressionOutputTypeDef = TypedDict(
-    "ExpressionOutputTypeDef",
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
     {
-        "Or": List[Dict[str, Any]],
-        "And": List[Dict[str, Any]],
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesOutputTypeDef,
-        "Tags": TagValuesOutputTypeDef,
-        "CostCategories": CostCategoryValuesOutputTypeDef,
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
     },
     total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
@@ -1498,27 +1398,14 @@
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
-    {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
-        "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
-    },
-    total=False,
-)
-
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1965,26 +1852,14 @@
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AnomalySubscriptionUnionTypeDef = Union[
-    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
-]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1999,14 +1874,23 @@
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2031,29 +1915,79 @@
         "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
     total=False,
 )
 
 
 class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
 
-CostCategorySplitChargeRuleUnionTypeDef = Union[
-    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
-]
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2213,67 +2147,14 @@
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
@@ -2281,15 +2162,15 @@
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesOutputTypeDef],
+        "Tags": List[TagValuesTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
```

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.pyi` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_ce.type_defs import AnomalyDateIntervalTypeDef
 
     data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -64,42 +64,37 @@
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
-    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
-    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
     "ResponseMetadataTypeDef",
-    "TagValuesOutputTypeDef",
+    "TagValuesTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
-    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
-    "TagValuesTypeDef",
-    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
@@ -124,22 +119,20 @@
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
-    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -153,20 +146,19 @@
     "ListCostAllocationTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvideAnomalyFeedbackResponseTypeDef",
     "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UpdateAnomalyMonitorResponseTypeDef",
     "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostCategoryDefinitionResponseTypeDef",
-    "ExpressionOutputTypeDef",
+    "ExpressionTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
-    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -181,36 +173,34 @@
     "InstanceDetailsTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "GetAnomalySubscriptionsResponseTypeDef",
-    "AnomalySubscriptionUnionTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
+    "GetAnomalySubscriptionsResponseTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CostCategorySplitChargeRuleUnionTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -346,40 +336,22 @@
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
     total=False,
 )
 
-CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
-    "CostCategorySplitChargeRuleParameterOutputTypeDef",
-    {
-        "Type": Literal["ALLOCATION_PERCENTAGES"],
-        "Values": List[str],
-    },
-)
-
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
-CostCategoryValuesOutputTypeDef = TypedDict(
-    "CostCategoryValuesOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
-    },
-    total=False,
-)
-
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -439,20 +411,20 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-TagValuesOutputTypeDef = TypedDict(
-    "TagValuesOutputTypeDef",
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
     {
         "Key": str,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
     },
     total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
@@ -490,24 +462,14 @@
 
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
-DimensionValuesOutputTypeDef = TypedDict(
-    "DimensionValuesOutputTypeDef",
-    {
-        "Key": DimensionType,
-        "Values": List[str],
-        "MatchOptions": List[MatchOptionType],
-    },
-    total=False,
-)
-
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -616,25 +578,14 @@
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
     total=False,
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
-    {
-        "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
-    },
-    total=False,
-)
-
-ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -1016,39 +967,14 @@
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
-    "_RequiredAnomalySubscriptionOutputTypeDef",
-    {
-        "MonitorArnList": List[str],
-        "Subscribers": List[SubscriberTypeDef],
-        "Frequency": AnomalySubscriptionFrequencyType,
-        "SubscriptionName": str,
-    },
-)
-_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
-    "_OptionalAnomalySubscriptionOutputTypeDef",
-    {
-        "SubscriptionArn": str,
-        "AccountId": str,
-        "Threshold": float,
-        "ThresholdExpression": "ExpressionOutputTypeDef",
-    },
-    total=False,
-)
-
-class AnomalySubscriptionOutputTypeDef(
-    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
-):
-    pass
-
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1148,36 +1074,14 @@
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
-    {
-        "Source": str,
-        "Targets": List[str],
-        "Method": CostCategorySplitChargeMethodType,
-    },
-)
-_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
-    {
-        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-class CostCategorySplitChargeRuleOutputTypeDef(
-    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
-    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
-):
-    pass
-
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1410,23 +1314,23 @@
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExpressionOutputTypeDef = TypedDict(
-    "ExpressionOutputTypeDef",
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
     {
-        "Or": List[Dict[str, Any]],
-        "And": List[Dict[str, Any]],
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesOutputTypeDef,
-        "Tags": TagValuesOutputTypeDef,
-        "CostCategories": CostCategoryValuesOutputTypeDef,
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
     },
     total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
@@ -1463,27 +1367,14 @@
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
-    {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
-        "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
-    },
-    total=False,
-)
-
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1902,26 +1793,14 @@
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AnomalySubscriptionUnionTypeDef = Union[
-    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
-]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1934,14 +1813,23 @@
 
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1966,27 +1854,73 @@
         "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
     total=False,
 )
 
 class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
-CostCategorySplitChargeRuleUnionTypeDef = Union[
-    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
-]
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
+    },
+    total=False,
+)
+
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2144,63 +2078,14 @@
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
@@ -2208,15 +2093,15 @@
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesOutputTypeDef],
+        "Tags": List[TagValuesTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
```

### Comparing `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/SOURCES.txt` & `types-aiobotocore-ce-2.5.2.post2/types_aiobotocore_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

