# Comparing `tmp/types-aiobotocore-forecast-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-forecast-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-forecast-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-forecast-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-forecast-2.5.2.post1.tar` & `types-aiobotocore-forecast-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.241582 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54527 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54441 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72389 2023-08-02 14:38:57.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72322 2023-08-02 14:38:56.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.660261 types-aiobotocore-forecast-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-04 12:00:55.660261 types-aiobotocore-forecast-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.660261 types-aiobotocore-forecast-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 11:46:23.000000 types-aiobotocore-forecast-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.660261 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54437 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54351 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65358 2023-08-04 11:46:27.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65305 2023-08-04 11:46:25.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:24.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.660261 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:55.000000 types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-forecast-2.5.2.post1/LICENSE` & `types-aiobotocore-forecast-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/setup.py` & `types-aiobotocore-forecast-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-forecast",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ForecastService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.pyi` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__main__.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ForecastService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigUnionTypeDef,
+    DataConfigTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -75,19 +75,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigUnionTypeDef,
+    FeaturizationConfigTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigUnionTypeDef,
-    InputDataConfigUnionTypeDef,
+    HyperParameterTuningJobConfigTypeDef,
+    InputDataConfigTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -96,20 +96,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaUnionTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceUnionTypeDef,
-    TimeSeriesSelectorUnionTypeDef,
-    TimeSeriesTransformationUnionTypeDef,
+    TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesSelectorTypeDef,
+    TimeSeriesTransformationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -172,15 +172,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigUnionTypeDef = ...,
+        DataConfig: DataConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -194,15 +194,15 @@
 
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaUnionTypeDef,
+        Schema: SchemaTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -249,15 +249,15 @@
     async def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...,
+        Schema: SchemaTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -286,15 +286,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_forecast)
@@ -328,24 +328,24 @@
         """
 
     async def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigUnionTypeDef,
-        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
+        FeaturizationConfig: FeaturizationConfigTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
+        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -371,15 +371,15 @@
         """
 
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -388,16 +388,16 @@
         """
 
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.pyi` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigUnionTypeDef,
+    DataConfigTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -75,19 +75,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigUnionTypeDef,
+    FeaturizationConfigTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigUnionTypeDef,
-    InputDataConfigUnionTypeDef,
+    HyperParameterTuningJobConfigTypeDef,
+    InputDataConfigTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -96,20 +96,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaUnionTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceUnionTypeDef,
-    TimeSeriesSelectorUnionTypeDef,
-    TimeSeriesTransformationUnionTypeDef,
+    TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesSelectorTypeDef,
+    TimeSeriesTransformationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -165,15 +165,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigUnionTypeDef = ...,
+        DataConfig: DataConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -186,15 +186,15 @@
         """
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaUnionTypeDef,
+        Schema: SchemaTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -238,15 +238,15 @@
     async def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaUnionTypeDef = ...,
+        Schema: SchemaTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -273,15 +273,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_forecast)
@@ -312,24 +312,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_monitor)
         """
     async def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigUnionTypeDef,
-        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
+        FeaturizationConfig: FeaturizationConfigTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
+        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -353,15 +353,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_predictor_backtest_export_job)
         """
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
+        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -369,16 +369,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_what_if_analysis)
         """
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.pyi` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.pyi` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.py` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_forecast.type_defs import ActionTypeDef
 
     data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -39,23 +39,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionTypeDef",
-    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
-    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
-    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
     "ResponseMetadataTypeDef",
@@ -93,15 +89,14 @@
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
     "ErrorMetricTypeDef",
-    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
     "PaginatorConfigTypeDef",
@@ -118,15 +113,14 @@
     "TestWindowSummaryTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
-    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAutoPredictorResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
@@ -147,32 +141,29 @@
     "ListTagsForResourceResponseTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
-    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
     "ListForecastsRequestRequestTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
     "ListMonitorsRequestRequestTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     "ListPredictorsRequestRequestTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
-    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
-    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
@@ -186,21 +177,18 @@
     "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
-    "SchemaOutputTypeDef",
     "SchemaTypeDef",
-    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
-    "DataConfigUnionTypeDef",
+    "DescribeAutoPredictorResponseTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -211,115 +199,72 @@
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
-    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
-    "InputDataConfigUnionTypeDef",
-    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "DescribeDatasetResponseTypeDef",
-    "DescribeExplainabilityResponseTypeDef",
-    "TimeSeriesIdentifiersOutputTypeDef",
-    "TimeSeriesReplacementsDataSourceOutputTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateExplainabilityRequestRequestTypeDef",
-    "SchemaUnionTypeDef",
+    "DescribeDatasetResponseTypeDef",
+    "DescribeExplainabilityResponseTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
-    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
-    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
-    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
-    "TimeSeriesSelectorOutputTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
-    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "DescribeForecastResponseTypeDef",
-    "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
-    "TimeSeriesSelectorUnionTypeDef",
+    "DescribeForecastResponseTypeDef",
+    "DescribeWhatIfAnalysisResponseTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
-_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
-    "_RequiredAdditionalDatasetOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
-    "_OptionalAdditionalDatasetOutputTypeDef",
-    {
-        "Configuration": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-
-class AdditionalDatasetOutputTypeDef(
-    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
-):
-    pass
-
-
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
-
-AttributeConfigOutputTypeDef = TypedDict(
-    "AttributeConfigOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Transformations": Dict[str, str],
-    },
-)
-
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
 )
@@ -329,22 +274,14 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
-CategoricalParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "Values": List[str],
-    },
-)
-
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -361,21 +298,19 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -445,19 +380,17 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -728,56 +661,33 @@
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
-_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationMethodOutputTypeDef",
-    {
-        "FeaturizationMethodName": Literal["filling"],
-    },
-)
-_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationMethodOutputTypeDef",
-    {
-        "FeaturizationMethodParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class FeaturizationMethodOutputTypeDef(
-    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
-):
-    pass
-
-
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -826,21 +736,19 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
-
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1005,34 +913,14 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
-_RequiredDataConfigOutputTypeDef = TypedDict(
-    "_RequiredDataConfigOutputTypeDef",
-    {
-        "DatasetGroupArn": str,
-    },
-)
-_OptionalDataConfigOutputTypeDef = TypedDict(
-    "_OptionalDataConfigOutputTypeDef",
-    {
-        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
-        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
-    pass
-
-
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1040,19 +928,17 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
-
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
-
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1069,22 +955,20 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1092,21 +976,19 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1311,54 +1193,31 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-_RequiredFeaturizationOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationOutputTypeDef",
-    {
-        "AttributeName": str,
-    },
-)
-_OptionalFeaturizationOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationOutputTypeDef",
-    {
-        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class FeaturizationOutputTypeDef(
-    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
-):
-    pass
-
-
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1417,22 +1276,20 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1494,64 +1351,31 @@
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
-    {
-        "DatasetGroupArn": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
-        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
-    },
-    total=False,
-)
-
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
-ParameterRangesOutputTypeDef = TypedDict(
-    "ParameterRangesOutputTypeDef",
-    {
-        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
-    },
-    total=False,
-)
-
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
@@ -1630,22 +1454,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
-
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1757,74 +1579,31 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
-SchemaOutputTypeDef = TypedDict(
-    "SchemaOutputTypeDef",
-    {
-        "Attributes": List[SchemaAttributeTypeDef],
-    },
-    total=False,
-)
-
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
-TimeSeriesTransformationOutputTypeDef = TypedDict(
-    "TimeSeriesTransformationOutputTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
-    },
-    total=False,
-)
-
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
         "Action": ActionTypeDef,
         "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
-DescribeAutoPredictorResponseTypeDef = TypedDict(
-    "DescribeAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "PredictorName": str,
-        "ForecastHorizon": int,
-        "ForecastTypes": List[str],
-        "ForecastFrequency": str,
-        "ForecastDimensions": List[str],
-        "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
-        "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
     },
 )
 _OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
@@ -1842,23 +1621,46 @@
         "Tags": Sequence[TagTypeDef],
         "MonitorConfig": MonitorConfigTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
-
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
+DescribeAutoPredictorResponseTypeDef = TypedDict(
+    "DescribeAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "PredictorName": str,
+        "ForecastHorizon": int,
+        "ForecastTypes": List[str],
+        "ForecastFrequency": str,
+        "ForecastDimensions": List[str],
+        "DatasetImportJobArns": List[str],
+        "DataConfig": DataConfigTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
+        "MonitorInfo": MonitorInfoTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -1885,22 +1687,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateExplainabilityExportRequestRequestTypeDef(
     _RequiredCreateExplainabilityExportRequestRequestTypeDef,
     _OptionalCreateExplainabilityExportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobName": str,
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1910,22 +1710,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateForecastExportJobRequestRequestTypeDef(
     _RequiredCreateForecastExportJobRequestRequestTypeDef,
     _OptionalCreateForecastExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
     {
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1935,22 +1733,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreatePredictorBacktestExportJobRequestRequestTypeDef(
     _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
     _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
     {
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": Sequence[str],
         "Destination": DataDestinationTypeDef,
     },
@@ -1960,22 +1756,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
-
 class CreateWhatIfForecastExportRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
@@ -2112,22 +1906,20 @@
         "Tags": Sequence[TagTypeDef],
         "Format": str,
         "ImportMode": ImportModeType,
     },
     total=False,
 )
 
-
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
         "DataSource": DataSourceTypeDef,
         "Status": str,
@@ -2168,36 +1960,14 @@
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationConfigOutputTypeDef",
-    {
-        "ForecastFrequency": str,
-    },
-)
-_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationConfigOutputTypeDef",
-    {
-        "ForecastDimensions": List[str],
-        "Featurizations": List[FeaturizationOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class FeaturizationConfigOutputTypeDef(
-    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2205,30 +1975,19 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
-
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
-
-InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
-HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "ParameterRanges": ParameterRangesOutputTypeDef,
-    },
-    total=False,
-)
-
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
 )
@@ -2258,86 +2017,14 @@
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaOutputTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TimeSeriesIdentifiersOutputTypeDef = TypedDict(
-    "TimeSeriesIdentifiersOutputTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaOutputTypeDef,
-        "Format": str,
-    },
-    total=False,
-)
-
-_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
-    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
-    {
-        "S3Config": S3ConfigTypeDef,
-        "Schema": SchemaOutputTypeDef,
-    },
-)
-_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
-    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
-    {
-        "Format": str,
-        "TimestampFormat": str,
-    },
-    total=False,
-)
-
-
-class TimeSeriesReplacementsDataSourceOutputTypeDef(
-    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
-    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2349,21 +2036,19 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2377,23 +2062,58 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2412,25 +2132,20 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
-
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
-
-TimeSeriesTransformationUnionTypeDef = Union[
-    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
-]
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2486,17 +2201,14 @@
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FeaturizationConfigUnionTypeDef = Union[
-    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
-]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2516,24 +2228,19 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
-
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
-
-HyperParameterTuningJobConfigUnionTypeDef = Union[
-    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-]
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2549,134 +2256,87 @@
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
         "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "FeaturizationConfig": FeaturizationConfigTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TimeSeriesSelectorOutputTypeDef = TypedDict(
-    "TimeSeriesSelectorOutputTypeDef",
-    {
-        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
-    },
-    total=False,
-)
-
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
-        "ForecastTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
-TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
-    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
-]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
-
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
-    {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
     {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
+        "ForecastTypes": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
     {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
@@ -2690,21 +2350,19 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
-
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2713,16 +2371,46 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
 
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.pyi` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_forecast.type_defs import ActionTypeDef
 
     data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -39,22 +39,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionTypeDef",
-    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
-    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
-    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
     "ResponseMetadataTypeDef",
@@ -92,15 +90,14 @@
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
     "ErrorMetricTypeDef",
-    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
     "PaginatorConfigTypeDef",
@@ -117,15 +114,14 @@
     "TestWindowSummaryTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
-    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAutoPredictorResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
@@ -146,32 +142,29 @@
     "ListTagsForResourceResponseTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
-    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
     "ListForecastsRequestRequestTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
     "ListMonitorsRequestRequestTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     "ListPredictorsRequestRequestTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
-    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
-    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
@@ -185,21 +178,18 @@
     "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
-    "SchemaOutputTypeDef",
     "SchemaTypeDef",
-    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
-    "DataConfigUnionTypeDef",
+    "DescribeAutoPredictorResponseTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -210,110 +200,73 @@
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
-    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
-    "InputDataConfigUnionTypeDef",
-    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "DescribeDatasetResponseTypeDef",
-    "DescribeExplainabilityResponseTypeDef",
-    "TimeSeriesIdentifiersOutputTypeDef",
-    "TimeSeriesReplacementsDataSourceOutputTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateExplainabilityRequestRequestTypeDef",
-    "SchemaUnionTypeDef",
+    "DescribeDatasetResponseTypeDef",
+    "DescribeExplainabilityResponseTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
-    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
-    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
-    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
-    "TimeSeriesSelectorOutputTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
-    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "DescribeForecastResponseTypeDef",
-    "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
-    "TimeSeriesSelectorUnionTypeDef",
+    "DescribeForecastResponseTypeDef",
+    "DescribeWhatIfAnalysisResponseTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
-_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
-    "_RequiredAdditionalDatasetOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
-    "_OptionalAdditionalDatasetOutputTypeDef",
-    {
-        "Configuration": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-class AdditionalDatasetOutputTypeDef(
-    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
-):
-    pass
-
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
     "_OptionalAdditionalDatasetTypeDef",
     {
         "Configuration": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
-AttributeConfigOutputTypeDef = TypedDict(
-    "AttributeConfigOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Transformations": Dict[str, str],
-    },
-)
 
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
@@ -324,22 +277,14 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
-CategoricalParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "Values": List[str],
-    },
-)
-
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -356,19 +301,21 @@
     "_OptionalContinuousParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class ContinuousParameterRangeTypeDef(
     _RequiredContinuousParameterRangeTypeDef, _OptionalContinuousParameterRangeTypeDef
 ):
     pass
 
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "RoleArn": str,
         "KMSKeyArn": str,
     },
 )
@@ -438,17 +385,19 @@
     "_OptionalS3ConfigTypeDef",
     {
         "KMSKeyArn": str,
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 DatasetGroupSummaryTypeDef = TypedDict(
     "DatasetGroupSummaryTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetGroupName": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
@@ -719,52 +668,35 @@
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
-_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationMethodOutputTypeDef",
-    {
-        "FeaturizationMethodName": Literal["filling"],
-    },
-)
-_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationMethodOutputTypeDef",
-    {
-        "FeaturizationMethodParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class FeaturizationMethodOutputTypeDef(
-    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
-):
-    pass
-
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
     "_OptionalFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodParameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FeaturizationMethodTypeDef(
     _RequiredFeaturizationMethodTypeDef, _OptionalFeaturizationMethodTypeDef
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Condition": FilterConditionStringType,
     },
@@ -813,19 +745,21 @@
     "_OptionalIntegerParameterRangeTypeDef",
     {
         "ScalingType": ScalingTypeType,
     },
     total=False,
 )
 
+
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -990,32 +924,14 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
-_RequiredDataConfigOutputTypeDef = TypedDict(
-    "_RequiredDataConfigOutputTypeDef",
-    {
-        "DatasetGroupArn": str,
-    },
-)
-_OptionalDataConfigOutputTypeDef = TypedDict(
-    "_OptionalDataConfigOutputTypeDef",
-    {
-        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
-        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
-    },
-    total=False,
-)
-
-class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
-    pass
-
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1023,17 +939,19 @@
     {
         "AttributeConfigs": Sequence[AttributeConfigTypeDef],
         "AdditionalDatasets": Sequence[AdditionalDatasetTypeDef],
     },
     total=False,
 )
 
+
 class DataConfigTypeDef(_RequiredDataConfigTypeDef, _OptionalDataConfigTypeDef):
     pass
 
+
 PredictorBaselineTypeDef = TypedDict(
     "PredictorBaselineTypeDef",
     {
         "BaselineMetrics": List[BaselineMetricTypeDef],
     },
     total=False,
 )
@@ -1050,20 +968,22 @@
     {
         "DatasetArns": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetGroupRequestRequestTypeDef(
     _RequiredCreateDatasetGroupRequestRequestTypeDef,
     _OptionalCreateDatasetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
         "ResourceArn": str,
     },
 )
@@ -1071,19 +991,21 @@
     "_OptionalCreateMonitorRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1288,50 +1210,33 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
-_RequiredFeaturizationOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationOutputTypeDef",
-    {
-        "AttributeName": str,
-    },
-)
-_OptionalFeaturizationOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationOutputTypeDef",
-    {
-        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
-    },
-    total=False,
-)
-
-class FeaturizationOutputTypeDef(
-    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
-):
-    pass
-
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
     "_OptionalFeaturizationTypeDef",
     {
         "FeaturizationPipeline": Sequence[FeaturizationMethodTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
+
 ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetImportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1390,20 +1295,22 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestRequestTypeDef(
     _RequiredListMonitorEvaluationsRequestRequestTypeDef,
     _OptionalListMonitorEvaluationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListMonitorsRequestRequestTypeDef = TypedDict(
     "ListMonitorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
@@ -1465,59 +1372,32 @@
     {
         "Forecasts": List[ForecastSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
-    {
-        "DatasetGroupArn": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
-        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
-    },
-    total=False,
-)
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
     "_OptionalInputDataConfigTypeDef",
     {
         "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-ParameterRangesOutputTypeDef = TypedDict(
-    "ParameterRangesOutputTypeDef",
-    {
-        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
-    },
-    total=False,
-)
 
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
@@ -1597,20 +1477,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
     _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
 ):
     pass
 
+
 ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1722,74 +1604,31 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
-SchemaOutputTypeDef = TypedDict(
-    "SchemaOutputTypeDef",
-    {
-        "Attributes": List[SchemaAttributeTypeDef],
-    },
-    total=False,
-)
-
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
-TimeSeriesTransformationOutputTypeDef = TypedDict(
-    "TimeSeriesTransformationOutputTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
-    },
-    total=False,
-)
-
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
         "Action": ActionTypeDef,
         "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
-DescribeAutoPredictorResponseTypeDef = TypedDict(
-    "DescribeAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "PredictorName": str,
-        "ForecastHorizon": int,
-        "ForecastTypes": List[str],
-        "ForecastFrequency": str,
-        "ForecastDimensions": List[str],
-        "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
-        "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
     },
 )
 _OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
@@ -1807,21 +1646,48 @@
         "Tags": Sequence[TagTypeDef],
         "MonitorConfig": MonitorConfigTypeDef,
         "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
     },
     total=False,
 )
 
+
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
-DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
+
+DescribeAutoPredictorResponseTypeDef = TypedDict(
+    "DescribeAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "PredictorName": str,
+        "ForecastHorizon": int,
+        "ForecastTypes": List[str],
+        "ForecastFrequency": str,
+        "ForecastDimensions": List[str],
+        "DatasetImportJobArns": List[str],
+        "DataConfig": DataConfigTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
+        "MonitorInfo": MonitorInfoTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -1848,20 +1714,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateExplainabilityExportRequestRequestTypeDef(
     _RequiredCreateExplainabilityExportRequestRequestTypeDef,
     _OptionalCreateExplainabilityExportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateForecastExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastExportJobRequestRequestTypeDef",
     {
         "ForecastExportJobName": str,
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1871,20 +1739,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateForecastExportJobRequestRequestTypeDef(
     _RequiredCreateForecastExportJobRequestRequestTypeDef,
     _OptionalCreateForecastExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef",
     {
         "PredictorBacktestExportJobName": str,
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
     },
@@ -1894,20 +1764,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreatePredictorBacktestExportJobRequestRequestTypeDef(
     _RequiredCreatePredictorBacktestExportJobRequestRequestTypeDef,
     _OptionalCreatePredictorBacktestExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateWhatIfForecastExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastExportRequestRequestTypeDef",
     {
         "WhatIfForecastExportName": str,
         "WhatIfForecastArns": Sequence[str],
         "Destination": DataDestinationTypeDef,
     },
@@ -1917,20 +1789,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "Format": str,
     },
     total=False,
 )
 
+
 class CreateWhatIfForecastExportRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastExportRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastExportRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeExplainabilityExportResponseTypeDef = TypedDict(
     "DescribeExplainabilityExportResponseTypeDef",
     {
         "ExplainabilityExportArn": str,
         "ExplainabilityExportName": str,
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
@@ -2067,20 +1941,22 @@
         "Tags": Sequence[TagTypeDef],
         "Format": str,
         "ImportMode": ImportModeType,
     },
     total=False,
 )
 
+
 class CreateDatasetImportJobRequestRequestTypeDef(
     _RequiredCreateDatasetImportJobRequestRequestTypeDef,
     _OptionalCreateDatasetImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DatasetImportJobSummaryTypeDef = TypedDict(
     "DatasetImportJobSummaryTypeDef",
     {
         "DatasetImportJobArn": str,
         "DatasetImportJobName": str,
         "DataSource": DataSourceTypeDef,
         "Status": str,
@@ -2121,34 +1997,14 @@
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
-    "_RequiredFeaturizationConfigOutputTypeDef",
-    {
-        "ForecastFrequency": str,
-    },
-)
-_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
-    "_OptionalFeaturizationConfigOutputTypeDef",
-    {
-        "ForecastDimensions": List[str],
-        "Featurizations": List[FeaturizationOutputTypeDef],
-    },
-    total=False,
-)
-
-class FeaturizationConfigOutputTypeDef(
-    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
-):
-    pass
-
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2156,27 +2012,20 @@
     {
         "ForecastDimensions": Sequence[str],
         "Featurizations": Sequence[FeaturizationTypeDef],
     },
     total=False,
 )
 
+
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
-InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
-HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "ParameterRanges": ParameterRangesOutputTypeDef,
-    },
-    total=False,
-)
 
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
@@ -2207,84 +2056,14 @@
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaOutputTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaOutputTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TimeSeriesIdentifiersOutputTypeDef = TypedDict(
-    "TimeSeriesIdentifiersOutputTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaOutputTypeDef,
-        "Format": str,
-    },
-    total=False,
-)
-
-_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
-    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
-    {
-        "S3Config": S3ConfigTypeDef,
-        "Schema": SchemaOutputTypeDef,
-    },
-)
-_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
-    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
-    {
-        "Format": str,
-        "TimestampFormat": str,
-    },
-    total=False,
-)
-
-class TimeSeriesReplacementsDataSourceOutputTypeDef(
-    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
-    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
-):
-    pass
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2296,19 +2075,21 @@
         "DataFrequency": str,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateExplainabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityRequestRequestTypeDef",
     {
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
     },
@@ -2322,21 +2103,60 @@
         "StartDateTime": str,
         "EndDateTime": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
-SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2355,23 +2175,22 @@
     {
         "Format": str,
         "TimestampFormat": str,
     },
     total=False,
 )
 
+
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
-TimeSeriesTransformationUnionTypeDef = Union[
-    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
-]
+
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2427,17 +2246,14 @@
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FeaturizationConfigUnionTypeDef = Union[
-    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
-]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2457,22 +2273,21 @@
         "EncryptionConfig": EncryptionConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OptimizationMetric": OptimizationMetricType,
     },
     total=False,
 )
 
+
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
-HyperParameterTuningJobConfigUnionTypeDef = Union[
-    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-]
+
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2488,132 +2303,89 @@
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
         "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "FeaturizationConfig": FeaturizationConfigTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TimeSeriesSelectorOutputTypeDef = TypedDict(
-    "TimeSeriesSelectorOutputTypeDef",
-    {
-        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
-    },
-    total=False,
-)
-
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
-        "ForecastTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
-TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
-    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
-]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
-    {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
     {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
+        "ForecastTypes": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
     {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
@@ -2627,19 +2399,21 @@
         "ForecastTypes": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
     },
     total=False,
 )
 
+
 class CreateForecastRequestRequestTypeDef(
     _RequiredCreateForecastRequestRequestTypeDef, _OptionalCreateForecastRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateWhatIfAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfAnalysisRequestRequestTypeDef",
     {
         "WhatIfAnalysisName": str,
         "ForecastArn": str,
     },
 )
@@ -2648,14 +2422,48 @@
     {
         "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
 
-TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
+
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/SOURCES.txt` & `types-aiobotocore-forecast-2.5.2.post2/types_aiobotocore_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

