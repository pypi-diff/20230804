# Comparing `tmp/types-aiobotocore-lookoutmetrics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lookoutmetrics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1.tar` & `types-aiobotocore-lookoutmetrics-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15615 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40126 2023-08-02 14:42:34.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40093 2023-08-02 14:42:34.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.186643 types-aiobotocore-lookoutmetrics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12579 2023-08-04 13:59:16.186643 types-aiobotocore-lookoutmetrics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11033 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.186643 types-aiobotocore-lookoutmetrics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.186643 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      498 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      497 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24304 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24266 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9711 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9709 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36521 2023-08-04 13:43:28.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36488 2023-08-04 13:43:28.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:27.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.186643 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12579 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/LICENSE` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutmetrics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__main__.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LookoutMetrics 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersUnionTypeDef,
+    AlertFiltersTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -42,16 +42,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterUnionTypeDef,
-    MetricSourceUnionTypeDef,
+    MetricSetDimensionFilterTypeDef,
+    MetricSourceTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -132,15 +132,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersUnionTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -163,23 +163,23 @@
 
     async def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceUnionTypeDef,
+        MetricSource: MetricSourceTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -445,15 +445,15 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersUnionTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
@@ -479,16 +479,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceUnionTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
+        MetricSource: MetricSourceTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersUnionTypeDef,
+    AlertFiltersTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -42,16 +42,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterUnionTypeDef,
-    MetricSourceUnionTypeDef,
+    MetricSetDimensionFilterTypeDef,
+    MetricSourceTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -124,15 +124,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersUnionTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -153,23 +153,23 @@
         """
     async def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceUnionTypeDef,
+        MetricSource: MetricSourceTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -411,15 +411,15 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersUnionTypeDef = ...
+        AlertFilters: AlertFiltersTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
@@ -443,16 +443,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceUnionTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
+        MetricSource: MetricSourceTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -197,14 +198,15 @@
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
@@ -283,26 +285,28 @@
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

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -195,14 +196,15 @@
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
@@ -281,26 +283,28 @@
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

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
     data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -41,15 +41,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
-    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
@@ -59,15 +58,14 @@
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -86,20 +84,18 @@
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActionTypeDef",
-    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
@@ -117,52 +113,43 @@
     "UpdateAlertResponseTypeDef",
     "UpdateAnomalyDetectorResponseTypeDef",
     "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
-    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
-    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
-    "RDSSourceConfigOutputTypeDef",
-    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
-    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
-    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
-    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
-    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "DescribeMetricSetResponseTypeDef",
     "CreateMetricSetRequestRequestTypeDef",
-    "MetricSourceUnionTypeDef",
+    "DescribeMetricSetResponseTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -197,23 +184,14 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-DimensionFilterOutputTypeDef = TypedDict(
-    "DimensionFilterOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueList": List[str],
-    },
-    total=False,
-)
-
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -397,27 +375,14 @@
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CsvFormatDescriptorOutputTypeDef = TypedDict(
-    "CsvFormatDescriptorOutputTypeDef",
-    {
-        "FileCompression": CSVFileCompressionType,
-        "Charset": str,
-        "ContainsHeader": bool,
-        "Delimiter": str,
-        "HeaderList": List[str],
-        "QuoteSymbol": str,
-    },
-    total=False,
-)
-
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -719,22 +684,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "SubnetIdList": List[str],
-        "SecurityGroupIdList": List[str],
-    },
-)
-
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
     },
 )
@@ -760,23 +717,14 @@
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
-AlertFiltersOutputTypeDef = TypedDict(
-    "AlertFiltersOutputTypeDef",
-    {
-        "MetricList": List[str],
-        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 AlertFiltersTypeDef = TypedDict(
     "AlertFiltersTypeDef",
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
@@ -1045,41 +993,23 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
-FileFormatDescriptorOutputTypeDef = TypedDict(
-    "FileFormatDescriptorOutputTypeDef",
-    {
-        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
-        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
-    },
-    total=False,
-)
-
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
-MetricSetDimensionFilterOutputTypeDef = TypedDict(
-    "MetricSetDimensionFilterOutputTypeDef",
-    {
-        "Name": str,
-        "FilterList": List[FilterTypeDef],
-    },
-    total=False,
-)
-
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
@@ -1108,44 +1038,14 @@
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RDSSourceConfigOutputTypeDef = TypedDict(
-    "RDSSourceConfigOutputTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "SecretManagerArn": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "RoleArn": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-RedshiftSourceConfigOutputTypeDef = TypedDict(
-    "RedshiftSourceConfigOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "SecretManagerArn": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "RoleArn": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
         "DatabasePort": int,
         "SecretManagerArn": str,
@@ -1181,20 +1081,19 @@
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersOutputTypeDef,
+        "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1306,25 +1205,14 @@
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3SourceConfigOutputTypeDef = TypedDict(
-    "S3SourceConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "TemplatedPathList": List[str],
-        "HistoricalDataPathList": List[str],
-        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
-    },
-    total=False,
-)
-
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1351,17 +1239,14 @@
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
 
-MetricSetDimensionFilterUnionTypeDef = Union[
-    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
-]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1389,27 +1274,14 @@
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
-MetricSourceOutputTypeDef = TypedDict(
-    "MetricSourceOutputTypeDef",
-    {
-        "S3SourceConfig": S3SourceConfigOutputTypeDef,
-        "AppFlowConfig": AppFlowConfigTypeDef,
-        "CloudWatchConfig": CloudWatchConfigTypeDef,
-        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
-        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
-        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
-    },
-    total=False,
-)
-
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1444,35 +1316,14 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceOutputTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1484,27 +1335,47 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
 
-MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1513,15 +1384,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
     data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
-    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
@@ -58,15 +57,14 @@
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -85,20 +83,18 @@
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActionTypeDef",
-    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
@@ -116,52 +112,43 @@
     "UpdateAlertResponseTypeDef",
     "UpdateAnomalyDetectorResponseTypeDef",
     "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
-    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
-    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
-    "RDSSourceConfigOutputTypeDef",
-    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
-    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
-    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
-    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
-    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "DescribeMetricSetResponseTypeDef",
     "CreateMetricSetRequestRequestTypeDef",
-    "MetricSourceUnionTypeDef",
+    "DescribeMetricSetResponseTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -194,23 +181,14 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-DimensionFilterOutputTypeDef = TypedDict(
-    "DimensionFilterOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueList": List[str],
-    },
-    total=False,
-)
-
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -390,27 +368,14 @@
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CsvFormatDescriptorOutputTypeDef = TypedDict(
-    "CsvFormatDescriptorOutputTypeDef",
-    {
-        "FileCompression": CSVFileCompressionType,
-        "Charset": str,
-        "ContainsHeader": bool,
-        "Delimiter": str,
-        "HeaderList": List[str],
-        "QuoteSymbol": str,
-    },
-    total=False,
-)
-
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
         "ContainsHeader": bool,
         "Delimiter": str,
@@ -702,22 +667,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "SubnetIdList": List[str],
-        "SecurityGroupIdList": List[str],
-    },
-)
-
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
     },
 )
@@ -743,23 +700,14 @@
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
-AlertFiltersOutputTypeDef = TypedDict(
-    "AlertFiltersOutputTypeDef",
-    {
-        "MetricList": List[str],
-        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 AlertFiltersTypeDef = TypedDict(
     "AlertFiltersTypeDef",
     {
         "MetricList": Sequence[str],
         "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
     total=False,
@@ -1022,41 +970,23 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
-FileFormatDescriptorOutputTypeDef = TypedDict(
-    "FileFormatDescriptorOutputTypeDef",
-    {
-        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
-        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
-    },
-    total=False,
-)
-
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
-MetricSetDimensionFilterOutputTypeDef = TypedDict(
-    "MetricSetDimensionFilterOutputTypeDef",
-    {
-        "Name": str,
-        "FilterList": List[FilterTypeDef],
-    },
-    total=False,
-)
-
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
@@ -1085,44 +1015,14 @@
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RDSSourceConfigOutputTypeDef = TypedDict(
-    "RDSSourceConfigOutputTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "SecretManagerArn": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "RoleArn": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-RedshiftSourceConfigOutputTypeDef = TypedDict(
-    "RedshiftSourceConfigOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DatabaseHost": str,
-        "DatabasePort": int,
-        "SecretManagerArn": str,
-        "DatabaseName": str,
-        "TableName": str,
-        "RoleArn": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
         "DatabasePort": int,
         "SecretManagerArn": str,
@@ -1158,20 +1058,19 @@
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersOutputTypeDef,
+        "AlertFilters": AlertFiltersTypeDef,
     },
     total=False,
 )
 
-AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1279,25 +1178,14 @@
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3SourceConfigOutputTypeDef = TypedDict(
-    "S3SourceConfigOutputTypeDef",
-    {
-        "RoleArn": str,
-        "TemplatedPathList": List[str],
-        "HistoricalDataPathList": List[str],
-        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
-    },
-    total=False,
-)
-
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1322,17 +1210,14 @@
 )
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
-MetricSetDimensionFilterUnionTypeDef = Union[
-    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
-]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1360,27 +1245,14 @@
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
-MetricSourceOutputTypeDef = TypedDict(
-    "MetricSourceOutputTypeDef",
-    {
-        "S3SourceConfig": S3SourceConfigOutputTypeDef,
-        "AppFlowConfig": AppFlowConfigTypeDef,
-        "CloudWatchConfig": CloudWatchConfigTypeDef,
-        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
-        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
-        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
-    },
-    total=False,
-)
-
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1415,35 +1287,14 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceOutputTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1455,25 +1306,45 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
-MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1482,15 +1353,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
     },
     total=False,
 )
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutmetrics-2.5.2.post2/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

