# Comparing `tmp/types-aiobotocore-cloudwatch-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudwatch-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudwatch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudwatch-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-cloudwatch-2.5.2.post1.tar` & `types-aiobotocore-cloudwatch-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22083 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34930 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    25821 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46361 2023-08-02 14:34:50.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46312 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22083 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.363529 types-aiobotocore-cloudwatch-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-04 12:00:36.363529 types-aiobotocore-cloudwatch-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.363529 types-aiobotocore-cloudwatch-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.363529 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34905 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34850 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-08-04 11:42:04.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25867 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44909 2023-08-04 11:42:06.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44860 2023-08-04 11:42:05.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-04 11:42:03.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.363529 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:36.000000 types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudwatch-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/setup.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudwatch",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__main__.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatch 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -61,23 +61,23 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryUnionTypeDef,
+    MetricDataQueryTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorUnionTypeDef,
-    MetricStreamFilterUnionTypeDef,
-    MetricStreamStatisticsConfigurationUnionTypeDef,
+    MetricMathAnomalyDetectorTypeDef,
+    MetricStreamFilterTypeDef,
+    MetricStreamStatisticsConfigurationTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorUnionTypeDef,
+    SingleMetricAnomalyDetectorTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -157,16 +157,16 @@
     async def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -361,15 +361,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
         """
 
     async def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
@@ -479,17 +479,17 @@
     async def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
+        Configuration: AnomalyDetectorConfigurationTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -571,15 +571,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
+        Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -600,18 +600,18 @@
     async def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
-        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -61,23 +61,23 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryUnionTypeDef,
+    MetricDataQueryTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorUnionTypeDef,
-    MetricStreamFilterUnionTypeDef,
-    MetricStreamStatisticsConfigurationUnionTypeDef,
+    MetricMathAnomalyDetectorTypeDef,
+    MetricStreamFilterTypeDef,
+    MetricStreamStatisticsConfigurationTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorUnionTypeDef,
+    SingleMetricAnomalyDetectorTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -149,16 +149,16 @@
     async def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -337,15 +337,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
         """
     async def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
@@ -446,17 +446,17 @@
     async def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
+        Configuration: AnomalyDetectorConfigurationTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -533,15 +533,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
+        Metrics: Sequence[MetricDataQueryTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -560,18 +560,18 @@
     async def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
-        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     HistoryItemTypeType,
     ScanByType,
     StateValueType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
-    DescribeAnomalyDetectorsOutputTypeDef,
+    DescribeAnomalyDetectorsOutputMetricTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryUnionTypeDef,
+    MetricDataQueryTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -141,15 +141,15 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeAnomalyDetectorsOutputTypeDef]:
+    ) -> AsyncIterator[DescribeAnomalyDetectorsOutputMetricTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 
 class GetMetricDataPaginator(AioPaginator):
@@ -157,15 +157,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     HistoryItemTypeType,
     ScanByType,
     StateValueType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
-    DescribeAnomalyDetectorsOutputTypeDef,
+    DescribeAnomalyDetectorsOutputMetricTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryUnionTypeDef,
+    MetricDataQueryTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -135,30 +135,30 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeAnomalyDetectorsOutputTypeDef]:
+    ) -> AsyncIterator[DescribeAnomalyDetectorsOutputMetricTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 class GetMetricDataPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
-    MetricDataQueryOutputTypeDef,
+    MetricDataQueryAlarmTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
@@ -331,15 +331,15 @@
     unit: Awaitable[StandardUnitType]
     evaluation_periods: Awaitable[int]
     datapoints_to_alarm: Awaitable[int]
     threshold: Awaitable[float]
     comparison_operator: Awaitable[ComparisonOperatorType]
     treat_missing_data: Awaitable[str]
     evaluate_low_sample_count_percentile: Awaitable[str]
-    metrics: Awaitable[List[MetricDataQueryOutputTypeDef]]
+    metrics: Awaitable[List[MetricDataQueryAlarmTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
 
     async def delete(self) -> None:
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
-    MetricDataQueryOutputTypeDef,
+    MetricDataQueryAlarmTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
@@ -302,15 +302,15 @@
     unit: Awaitable[StandardUnitType]
     evaluation_periods: Awaitable[int]
     datapoints_to_alarm: Awaitable[int]
     threshold: Awaitable[float]
     comparison_operator: Awaitable[ComparisonOperatorType]
     treat_missing_data: Awaitable[str]
     evaluate_low_sample_count_percentile: Awaitable[str]
-    metrics: Awaitable[List[MetricDataQueryOutputTypeDef]]
+    metrics: Awaitable[List[MetricDataQueryAlarmTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
 
     async def delete(self) -> None:
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
-    "RangeOutputTypeDef",
+    "RangeTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
@@ -66,39 +66,37 @@
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterOutputTypeDef",
+    "MetricStreamFilterTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "InsightRuleContributorDatapointTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
-    "MetricStreamFilterTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PutDashboardInputRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "AnomalyDetectorConfigurationOutputTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
-    "SingleMetricAnomalyDetectorOutputTypeDef",
+    "SingleMetricAnomalyDetectorMetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
     "GetDashboardOutputTypeDef",
@@ -109,15 +107,14 @@
     "PutManagedInsightRulesOutputTypeDef",
     "PutMetricStreamOutputTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
-    "RangeTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
@@ -129,47 +126,41 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
-    "MetricStreamFilterUnionTypeDef",
-    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
-    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
-    "SingleMetricAnomalyDetectorUnionTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "MetricStreamStatisticsConfigurationUnionTypeDef",
-    "MetricDataQueryOutputTypeDef",
-    "MetricDataQueryTypeDef",
-    "AnomalyDetectorConfigurationUnionTypeDef",
     "PutMetricStreamInputRequestTypeDef",
+    "MetricDataQueryTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
     "MetricAlarmTypeDef",
-    "MetricMathAnomalyDetectorOutputTypeDef",
-    "MetricDataQueryUnionTypeDef",
+    "MetricMathAnomalyDetectorMetricTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
+    "MetricStatAlarmTypeDef",
+    "AnomalyDetectorMetricTypeDef",
     "AnomalyDetectorTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
-    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
+    "MetricDataQueryAlarmTypeDef",
+    "DescribeAnomalyDetectorsOutputMetricTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
         "AlarmName": str,
@@ -178,16 +169,16 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
 DimensionTypeDef = TypedDict(
@@ -477,16 +468,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterOutputTypeDef = TypedDict(
-    "MetricStreamFilterOutputTypeDef",
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -604,23 +595,14 @@
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
-    {
-        "Namespace": str,
-        "MetricNames": Sequence[str],
-    },
-    total=False,
-)
-
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -696,18 +678,18 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationOutputTypeDef",
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
     {
-        "ExcludedTimeRanges": List[RangeOutputTypeDef],
+        "ExcludedTimeRanges": List[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
@@ -745,36 +727,26 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
-MetricOutputTypeDef = TypedDict(
-    "MetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-    },
-    total=False,
-)
-
 MetricTypeDef = TypedDict(
     "MetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
     },
     total=False,
 )
 
-SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorOutputTypeDef",
+SingleMetricAnomalyDetectorMetricTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": List[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
@@ -998,22 +970,14 @@
 
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
-    {
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-)
-
 DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
         "AlarmName": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "HistoryItemType": HistoryItemTypeType,
         "StartDate": TimestampTypeDef,
@@ -1283,62 +1247,32 @@
 )
 
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
 
-MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
-    "MetricStreamStatisticsConfigurationOutputTypeDef",
-    {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": List[str],
-    },
-)
-
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
-        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": Sequence[str],
+        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": List[str],
     },
 )
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricOutputTypeDef],
+        "Metrics": List[MetricTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricStatOutputTypeDef = TypedDict(
-    "_RequiredMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Period": int,
-        "Stat": str,
-    },
-)
-_OptionalMetricStatOutputTypeDef = TypedDict(
-    "_OptionalMetricStatOutputTypeDef",
-    {
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-
-class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
-    pass
-
-
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
     },
@@ -1352,26 +1286,14 @@
 )
 
 
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
 
-SingleMetricAnomalyDetectorUnionTypeDef = Union[
-    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-]
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
-    {
-        "ExcludedTimeRanges": Sequence[RangeTypeDef],
-        "MetricTimezone": str,
-    },
-    total=False,
-)
-
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1416,53 +1338,52 @@
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "IncludeFilters": List[MetricStreamFilterTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricStreamStatisticsConfigurationUnionTypeDef = Union[
-    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
-]
-_RequiredMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredMetricDataQueryOutputTypeDef",
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
     {
-        "Id": str,
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
     },
 )
-_OptionalMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalMetricDataQueryOutputTypeDef",
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
     {
-        "MetricStat": MetricStatOutputTypeDef,
-        "Expression": str,
-        "Label": str,
-        "ReturnData": bool,
-        "Period": int,
-        "AccountId": str,
+        "IncludeFilters": Sequence[MetricStreamFilterTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
     },
     total=False,
 )
 
 
-class MetricDataQueryOutputTypeDef(
-    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
 
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
@@ -1483,41 +1404,62 @@
 )
 
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
 
-AnomalyDetectorConfigurationUnionTypeDef = Union[
-    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
-]
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
-        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
-        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
-        "IncludeLinkedAccountsMetrics": bool,
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
 ):
     pass
 
 
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
@@ -1542,31 +1484,30 @@
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryOutputTypeDef],
+        "Metrics": List[MetricDataQueryTypeDef],
         "ThresholdMetricId": str,
         "EvaluationState": Literal["PARTIAL_DATA"],
         "StateTransitionedTimestamp": datetime,
     },
     total=False,
 )
 
-MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
-    "MetricMathAnomalyDetectorOutputTypeDef",
+MetricMathAnomalyDetectorMetricTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
     total=False,
 )
 
-MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1607,14 +1548,55 @@
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
 
+_RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricAlarmInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "EvaluationPeriods": int,
+        "ComparisonOperator": ComparisonOperatorType,
+    },
+)
+_OptionalPutMetricAlarmInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricAlarmInputRequestTypeDef",
+    {
+        "AlarmDescription": str,
+        "ActionsEnabled": bool,
+        "OKActions": Sequence[str],
+        "AlarmActions": Sequence[str],
+        "InsufficientDataActions": Sequence[str],
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "ExtendedStatistic": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Period": int,
+        "Unit": StandardUnitType,
+        "DatapointsToAlarm": int,
+        "Threshold": float,
+        "TreatMissingData": str,
+        "EvaluateLowSampleCountPercentile": str,
+        "Metrics": Sequence[MetricDataQueryTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "ThresholdMetricId": str,
+    },
+    total=False,
+)
+
+
+class PutMetricAlarmInputRequestTypeDef(
+    _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
+):
+    pass
+
+
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1625,152 +1607,127 @@
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
+_RequiredMetricStatAlarmTypeDef = TypedDict(
+    "_RequiredMetricStatAlarmTypeDef",
     {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
+        "Metric": MetricAlarmTypeDef,
+        "Period": int,
         "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
     },
-    total=False,
 )
-
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
+_OptionalMetricStatAlarmTypeDef = TypedDict(
+    "_OptionalMetricStatAlarmTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-)
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Unit": StandardUnitType,
     },
     total=False,
 )
 
 
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
+class MetricStatAlarmTypeDef(_RequiredMetricStatAlarmTypeDef, _OptionalMetricStatAlarmTypeDef):
     pass
 
 
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
-    {
-        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-)
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
+AnomalyDetectorMetricTypeDef = TypedDict(
+    "AnomalyDetectorMetricTypeDef",
     {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorMetricTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorMetricTypeDef,
     },
     total=False,
 )
 
-
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricAlarmInputRequestTypeDef",
-    {
-        "AlarmName": str,
-        "EvaluationPeriods": int,
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalPutMetricAlarmInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricAlarmInputRequestTypeDef",
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
     {
-        "AlarmDescription": str,
-        "ActionsEnabled": bool,
-        "OKActions": Sequence[str],
-        "AlarmActions": Sequence[str],
-        "InsufficientDataActions": Sequence[str],
-        "MetricName": str,
         "Namespace": str,
-        "Statistic": StatisticType,
-        "ExtendedStatistic": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Period": int,
-        "Unit": StandardUnitType,
-        "DatapointsToAlarm": int,
-        "Threshold": float,
-        "TreatMissingData": str,
-        "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "ThresholdMetricId": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
-
-class PutMetricAlarmInputRequestTypeDef(
-    _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
-):
-    pass
-
-
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
-MetricMathAnomalyDetectorUnionTypeDef = Union[
-    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "Configuration": AnomalyDetectorConfigurationTypeDef,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+_RequiredMetricDataQueryAlarmTypeDef = TypedDict(
+    "_RequiredMetricDataQueryAlarmTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryAlarmTypeDef = TypedDict(
+    "_OptionalMetricDataQueryAlarmTypeDef",
+    {
+        "MetricStat": MetricStatAlarmTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class MetricDataQueryAlarmTypeDef(
+    _RequiredMetricDataQueryAlarmTypeDef, _OptionalMetricDataQueryAlarmTypeDef
+):
+    pass
+
+
+DescribeAnomalyDetectorsOutputMetricTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsOutputMetricTypeDef",
+    {
+        "AnomalyDetectors": List[AnomalyDetectorMetricTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
-    "RangeOutputTypeDef",
+    "RangeTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
@@ -65,39 +65,37 @@
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterOutputTypeDef",
+    "MetricStreamFilterTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "InsightRuleContributorDatapointTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
-    "MetricStreamFilterTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
     "PutDashboardInputRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "AnomalyDetectorConfigurationOutputTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
-    "SingleMetricAnomalyDetectorOutputTypeDef",
+    "SingleMetricAnomalyDetectorMetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
     "GetDashboardOutputTypeDef",
@@ -108,15 +106,14 @@
     "PutManagedInsightRulesOutputTypeDef",
     "PutMetricStreamOutputTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
-    "RangeTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
@@ -128,47 +125,41 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
-    "MetricStreamFilterUnionTypeDef",
-    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
-    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
-    "SingleMetricAnomalyDetectorUnionTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "MetricStreamStatisticsConfigurationUnionTypeDef",
-    "MetricDataQueryOutputTypeDef",
-    "MetricDataQueryTypeDef",
-    "AnomalyDetectorConfigurationUnionTypeDef",
     "PutMetricStreamInputRequestTypeDef",
+    "MetricDataQueryTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
     "MetricAlarmTypeDef",
-    "MetricMathAnomalyDetectorOutputTypeDef",
-    "MetricDataQueryUnionTypeDef",
+    "MetricMathAnomalyDetectorMetricTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
+    "MetricStatAlarmTypeDef",
+    "AnomalyDetectorMetricTypeDef",
     "AnomalyDetectorTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
-    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
+    "MetricDataQueryAlarmTypeDef",
+    "DescribeAnomalyDetectorsOutputMetricTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
         "AlarmName": str,
@@ -177,16 +168,16 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
 DimensionTypeDef = TypedDict(
@@ -470,16 +461,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterOutputTypeDef = TypedDict(
-    "MetricStreamFilterOutputTypeDef",
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -593,23 +584,14 @@
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
-    {
-        "Namespace": str,
-        "MetricNames": Sequence[str],
-    },
-    total=False,
-)
-
 MetricStreamStatisticsMetricTypeDef = TypedDict(
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -681,18 +663,18 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationOutputTypeDef",
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
     {
-        "ExcludedTimeRanges": List[RangeOutputTypeDef],
+        "ExcludedTimeRanges": List[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
@@ -728,36 +710,26 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
-MetricOutputTypeDef = TypedDict(
-    "MetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-    },
-    total=False,
-)
-
 MetricTypeDef = TypedDict(
     "MetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
     },
     total=False,
 )
 
-SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorOutputTypeDef",
+SingleMetricAnomalyDetectorMetricTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": List[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
@@ -975,22 +947,14 @@
 )
 
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
-    {
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-)
-
 DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
         "AlarmName": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "HistoryItemType": HistoryItemTypeType,
         "StartDate": TimestampTypeDef,
@@ -1252,60 +1216,32 @@
     },
     total=False,
 )
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
-MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
-    "MetricStreamStatisticsConfigurationOutputTypeDef",
-    {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": List[str],
-    },
-)
-
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
-        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": Sequence[str],
+        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": List[str],
     },
 )
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricOutputTypeDef],
+        "Metrics": List[MetricTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricStatOutputTypeDef = TypedDict(
-    "_RequiredMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Period": int,
-        "Stat": str,
-    },
-)
-_OptionalMetricStatOutputTypeDef = TypedDict(
-    "_OptionalMetricStatOutputTypeDef",
-    {
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
-    pass
-
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
     },
@@ -1317,26 +1253,14 @@
     },
     total=False,
 )
 
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
-SingleMetricAnomalyDetectorUnionTypeDef = Union[
-    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-]
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
-    {
-        "ExcludedTimeRanges": Sequence[RangeTypeDef],
-        "MetricTimezone": str,
-    },
-    total=False,
-)
-
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1381,52 +1305,51 @@
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "IncludeFilters": List[MetricStreamFilterTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricStreamStatisticsConfigurationUnionTypeDef = Union[
-    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
-]
-_RequiredMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredMetricDataQueryOutputTypeDef",
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
     {
-        "Id": str,
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
     },
 )
-_OptionalMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalMetricDataQueryOutputTypeDef",
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
     {
-        "MetricStat": MetricStatOutputTypeDef,
-        "Expression": str,
-        "Label": str,
-        "ReturnData": bool,
-        "Period": int,
-        "AccountId": str,
+        "IncludeFilters": Sequence[MetricStreamFilterTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
     },
     total=False,
 )
 
-class MetricDataQueryOutputTypeDef(
-    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
@@ -1444,40 +1367,59 @@
     },
     total=False,
 )
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
-AnomalyDetectorConfigurationUnionTypeDef = Union[
-    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
-]
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
-        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
-        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
-        "IncludeLinkedAccountsMetrics": bool,
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
 ):
     pass
 
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
         "AlarmName": str,
@@ -1501,31 +1443,30 @@
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryOutputTypeDef],
+        "Metrics": List[MetricDataQueryTypeDef],
         "ThresholdMetricId": str,
         "EvaluationState": Literal["PARTIAL_DATA"],
         "StateTransitionedTimestamp": datetime,
     },
     total=False,
 )
 
-MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
-    "MetricMathAnomalyDetectorOutputTypeDef",
+MetricMathAnomalyDetectorMetricTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
     total=False,
 )
 
-MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1564,14 +1505,53 @@
 
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
+_RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricAlarmInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "EvaluationPeriods": int,
+        "ComparisonOperator": ComparisonOperatorType,
+    },
+)
+_OptionalPutMetricAlarmInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricAlarmInputRequestTypeDef",
+    {
+        "AlarmDescription": str,
+        "ActionsEnabled": bool,
+        "OKActions": Sequence[str],
+        "AlarmActions": Sequence[str],
+        "InsufficientDataActions": Sequence[str],
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+        "ExtendedStatistic": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Period": int,
+        "Unit": StandardUnitType,
+        "DatapointsToAlarm": int,
+        "Threshold": float,
+        "TreatMissingData": str,
+        "EvaluateLowSampleCountPercentile": str,
+        "Metrics": Sequence[MetricDataQueryTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "ThresholdMetricId": str,
+    },
+    total=False,
+)
+
+class PutMetricAlarmInputRequestTypeDef(
+    _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
+):
+    pass
+
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1582,146 +1562,123 @@
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
+_RequiredMetricStatAlarmTypeDef = TypedDict(
+    "_RequiredMetricStatAlarmTypeDef",
     {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
+        "Metric": MetricAlarmTypeDef,
+        "Period": int,
         "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
     },
 )
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
+_OptionalMetricStatAlarmTypeDef = TypedDict(
+    "_OptionalMetricStatAlarmTypeDef",
     {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Unit": StandardUnitType,
     },
     total=False,
 )
 
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
+class MetricStatAlarmTypeDef(_RequiredMetricStatAlarmTypeDef, _OptionalMetricStatAlarmTypeDef):
     pass
 
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
-    {
-        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-    },
-)
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
+AnomalyDetectorMetricTypeDef = TypedDict(
+    "AnomalyDetectorMetricTypeDef",
     {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorMetricTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorMetricTypeDef,
     },
     total=False,
 )
 
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
-):
-    pass
-
-_RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricAlarmInputRequestTypeDef",
-    {
-        "AlarmName": str,
-        "EvaluationPeriods": int,
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalPutMetricAlarmInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricAlarmInputRequestTypeDef",
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
     {
-        "AlarmDescription": str,
-        "ActionsEnabled": bool,
-        "OKActions": Sequence[str],
-        "AlarmActions": Sequence[str],
-        "InsufficientDataActions": Sequence[str],
-        "MetricName": str,
         "Namespace": str,
-        "Statistic": StatisticType,
-        "ExtendedStatistic": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Period": int,
-        "Unit": StandardUnitType,
-        "DatapointsToAlarm": int,
-        "Threshold": float,
-        "TreatMissingData": str,
-        "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "ThresholdMetricId": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
-class PutMetricAlarmInputRequestTypeDef(
-    _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
-):
-    pass
-
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
-MetricMathAnomalyDetectorUnionTypeDef = Union[
-    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "Configuration": AnomalyDetectorConfigurationTypeDef,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+_RequiredMetricDataQueryAlarmTypeDef = TypedDict(
+    "_RequiredMetricDataQueryAlarmTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryAlarmTypeDef = TypedDict(
+    "_OptionalMetricDataQueryAlarmTypeDef",
+    {
+        "MetricStat": MetricStatAlarmTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class MetricDataQueryAlarmTypeDef(
+    _RequiredMetricDataQueryAlarmTypeDef, _OptionalMetricDataQueryAlarmTypeDef
+):
+    pass
+
+DescribeAnomalyDetectorsOutputMetricTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsOutputMetricTypeDef",
+    {
+        "AnomalyDetectors": List[AnomalyDetectorMetricTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.py` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudwatch-2.5.2.post2/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

