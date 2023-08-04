# Comparing `tmp/types-aiobotocore-personalize-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-personalize-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-personalize-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-personalize-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-personalize-2.5.2.post1.tar` & `types-aiobotocore-personalize-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.561499 types-aiobotocore-personalize-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24507 2023-08-02 14:52:47.557499 types-aiobotocore-personalize-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.561499 types-aiobotocore-personalize-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.549499 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53915 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65728 2023-08-02 14:44:43.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65693 2023-08-02 14:44:40.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:39.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.557499 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24507 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15392 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13858 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3887 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3886 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54521 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54429 2023-08-04 13:46:31.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10451 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10449 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19533 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19514 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63287 2023-08-04 13:46:34.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63252 2023-08-04 13:46:33.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15392 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-personalize-2.5.2.post1/LICENSE` & `types-aiobotocore-personalize-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post1/setup.py` & `types-aiobotocore-personalize-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-personalize",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Personalize 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__init__.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__init__.pyi` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/__main__.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Personalize 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Personalize 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
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

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/client.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,20 @@
     ListRecipesPaginator,
     ListRecommendersPaginator,
     ListSchemasPaginator,
     ListSolutionsPaginator,
     ListSolutionVersionsPaginator,
 )
 from .type_defs import (
-    BatchInferenceJobConfigUnionTypeDef,
+    BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
-    CampaignConfigUnionTypeDef,
+    CampaignConfigTypeDef,
     CreateBatchInferenceJobResponseTypeDef,
     CreateBatchSegmentJobResponseTypeDef,
     CreateCampaignResponseTypeDef,
     CreateDatasetExportJobResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
     CreateDatasetImportJobResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -96,20 +96,21 @@
     ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
-    RecommenderConfigUnionTypeDef,
-    SolutionConfigUnionTypeDef,
+    RecommenderConfigTypeDef,
+    SolutionConfigTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -178,15 +179,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        batchInferenceJobConfig: BatchInferenceJobConfigUnionTypeDef = ...,
+        batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_batch_inference_job)
@@ -213,15 +214,15 @@
 
     async def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigUnionTypeDef = ...,
+        campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_campaign)
@@ -340,15 +341,15 @@
 
     async def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
-        recommenderConfig: RecommenderConfigUnionTypeDef = ...,
+        recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
@@ -370,15 +371,15 @@
         *,
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
-        solutionConfig: SolutionConfigUnionTypeDef = ...,
+        solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution)
@@ -885,24 +886,34 @@
 
     async def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigUnionTypeDef = ...
+        campaignConfig: CampaignConfigTypeDef = ...
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_campaign)
         """
 
+    async def update_dataset(
+        self, *, datasetArn: str, schemaArn: str
+    ) -> UpdateDatasetResponseTypeDef:
+        """
+        Update a dataset to replace its schema with a new or existing one.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_dataset)
+        """
+
     async def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
@@ -911,15 +922,15 @@
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_metric_attribution)
         """
 
     async def update_recommender(
-        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigUnionTypeDef
+        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
     ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_recommender)
         """
```

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/client.pyi` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,20 @@
     ListRecipesPaginator,
     ListRecommendersPaginator,
     ListSchemasPaginator,
     ListSolutionsPaginator,
     ListSolutionVersionsPaginator,
 )
 from .type_defs import (
-    BatchInferenceJobConfigUnionTypeDef,
+    BatchInferenceJobConfigTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
-    CampaignConfigUnionTypeDef,
+    CampaignConfigTypeDef,
     CreateBatchInferenceJobResponseTypeDef,
     CreateBatchSegmentJobResponseTypeDef,
     CreateCampaignResponseTypeDef,
     CreateDatasetExportJobResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
     CreateDatasetImportJobResponseTypeDef,
     CreateDatasetResponseTypeDef,
@@ -96,20 +96,21 @@
     ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
-    RecommenderConfigUnionTypeDef,
-    SolutionConfigUnionTypeDef,
+    RecommenderConfigTypeDef,
+    SolutionConfigTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     UpdateCampaignResponseTypeDef,
+    UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
     UpdateRecommenderResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -171,15 +172,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        batchInferenceJobConfig: BatchInferenceJobConfigUnionTypeDef = ...,
+        batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Creates a batch inference job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_batch_inference_job)
@@ -204,15 +205,15 @@
         """
     async def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigUnionTypeDef = ...,
+        campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_campaign)
@@ -323,15 +324,15 @@
         """
     async def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
-        recommenderConfig: RecommenderConfigUnionTypeDef = ...,
+        recommenderConfig: RecommenderConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
@@ -351,15 +352,15 @@
         *,
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
-        solutionConfig: SolutionConfigUnionTypeDef = ...,
+        solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution)
@@ -814,23 +815,32 @@
         """
     async def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigUnionTypeDef = ...
+        campaignConfig: CampaignConfigTypeDef = ...
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign by either deploying a new solution or changing the value of
         the campaign's `minProvisionedTPS` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_campaign)
         """
+    async def update_dataset(
+        self, *, datasetArn: str, schemaArn: str
+    ) -> UpdateDatasetResponseTypeDef:
+        """
+        Update a dataset to replace its schema with a new or existing one.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_dataset)
+        """
     async def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
         metricAttributionArn: str = ...
@@ -838,15 +848,15 @@
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_metric_attribution)
         """
     async def update_recommender(
-        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigUnionTypeDef
+        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
     ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_recommender)
         """
```

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/literals.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
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
@@ -187,14 +188,15 @@
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
@@ -273,26 +275,28 @@
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

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/literals.pyi` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
@@ -185,14 +186,15 @@
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
@@ -271,26 +273,28 @@
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

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/paginator.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/paginator.pyi` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/type_defs.py` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_personalize.type_defs import AlgorithmImageTypeDef
 
     data: AlgorithmImageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
     TrainingModeType,
@@ -31,41 +31,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlgorithmImageTypeDef",
-    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
-    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
-    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
-    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
-    "DatasetTypeDef",
+    "DatasetUpdateSummaryTypeDef",
     "DefaultCategoricalHyperParameterRangeTypeDef",
     "DefaultContinuousHyperParameterRangeTypeDef",
     "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
@@ -120,30 +116,28 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
-    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchInferenceJobConfigUnionTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
     "CampaignUpdateSummaryTypeDef",
-    "CampaignConfigUnionTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
@@ -167,35 +161,35 @@
     "ListBatchInferenceJobsResponseTypeDef",
     "ListBatchSegmentJobsResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
+    "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
+    "DatasetTypeDef",
     "DefaultHyperParameterRangesTypeDef",
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
-    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
@@ -209,49 +203,45 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
-    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
-    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderConfigUnionTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
-    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
     "ListRecommendersResponseTypeDef",
     "RecommenderTypeDef",
+    "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
-    "CreateSolutionRequestRequestTypeDef",
-    "SolutionConfigUnionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 _RequiredAlgorithmImageTypeDef = TypedDict(
     "_RequiredAlgorithmImageTypeDef",
@@ -268,23 +258,14 @@
 )
 
 
 class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
     pass
 
 
-AutoMLConfigOutputTypeDef = TypedDict(
-    "AutoMLConfigOutputTypeDef",
-    {
-        "metricName": str,
-        "recipeList": List[str],
-    },
-    total=False,
-)
-
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
@@ -294,22 +275,14 @@
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
     total=False,
 )
 
-BatchInferenceJobConfigOutputTypeDef = TypedDict(
-    "BatchInferenceJobConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-    },
-    total=False,
-)
-
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
@@ -357,22 +330,14 @@
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
     total=False,
 )
 
-CampaignConfigOutputTypeDef = TypedDict(
-    "CampaignConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-    },
-    total=False,
-)
-
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
@@ -386,23 +351,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
-CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalHyperParameterRangeOutputTypeDef",
-    {
-        "name": str,
-        "values": List[str],
-    },
-    total=False,
-)
-
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
@@ -567,23 +523,20 @@
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
         "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
 DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
@@ -1153,22 +1106,14 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
 )
 
-TrainingDataConfigOutputTypeDef = TypedDict(
-    "TrainingDataConfigOutputTypeDef",
-    {
-        "excludedDatasetColumns": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
     },
     total=False,
 )
@@ -1206,17 +1151,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchInferenceJobConfigUnionTypeDef = Union[
-    BatchInferenceJobConfigTypeDef, BatchInferenceJobConfigOutputTypeDef
-]
+UpdateDatasetRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetRequestRequestTypeDef",
+    {
+        "datasetArn": str,
+        "schemaArn": str,
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1270,24 +1220,23 @@
 
 
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigOutputTypeDef,
+        "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-CampaignConfigUnionTypeDef = Union[CampaignConfigTypeDef, CampaignConfigOutputTypeDef]
 _RequiredUpdateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
 )
 _OptionalUpdateCampaignRequestRequestTypeDef = TypedDict(
@@ -1643,14 +1592,22 @@
     "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMetricAttributionResponseTypeDef = TypedDict(
     "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1774,20 +1731,28 @@
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
+    total=False,
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
@@ -1842,24 +1807,14 @@
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterRangesOutputTypeDef = TypedDict(
-    "HyperParameterRangesOutputTypeDef",
-    {
-        "integerHyperParameterRanges": List[IntegerHyperParameterRangeTypeDef],
-        "continuousHyperParameterRanges": List[ContinuousHyperParameterRangeTypeDef],
-        "categoricalHyperParameterRanges": List[CategoricalHyperParameterRangeOutputTypeDef],
-    },
-    total=False,
-)
-
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
@@ -2041,24 +1996,14 @@
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecommenderConfigOutputTypeDef = TypedDict(
-    "RecommenderConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-        "minRecommendationRequestsPerSecond": int,
-        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
@@ -2072,15 +2017,15 @@
         "batchInferenceJobArn": str,
         "filterArn": str,
         "failureReason": str,
         "solutionVersionArn": str,
         "numResults": int,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
-        "batchInferenceJobConfig": BatchInferenceJobConfigOutputTypeDef,
+        "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
@@ -2243,15 +2188,15 @@
 CampaignTypeDef = TypedDict(
     "CampaignTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigOutputTypeDef,
+        "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
     total=False,
@@ -2261,14 +2206,22 @@
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
@@ -2278,86 +2231,75 @@
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-HPOConfigOutputTypeDef = TypedDict(
-    "HPOConfigOutputTypeDef",
+HPOConfigTypeDef = TypedDict(
+    "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
-        "algorithmHyperParameterRanges": HyperParameterRangesOutputTypeDef,
+        "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
-HPOConfigTypeDef = TypedDict(
-    "HPOConfigTypeDef",
+_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecommenderRequestRequestTypeDef",
     {
-        "hpoObjective": HPOObjectiveTypeDef,
-        "hpoResourceConfig": HPOResourceConfigTypeDef,
-        "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+    },
+)
+_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
+class CreateRecommenderRequestRequestTypeDef(
+    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
+):
+    pass
+
+
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
     total=False,
 )
 
-_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecommenderRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-    },
-)
-_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateRecommenderRequestRequestTypeDef(
-    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
-):
-    pass
-
-
-RecommenderConfigUnionTypeDef = Union[RecommenderConfigTypeDef, RecommenderConfigOutputTypeDef]
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
@@ -2406,28 +2348,14 @@
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SolutionConfigOutputTypeDef = TypedDict(
-    "SolutionConfigOutputTypeDef",
-    {
-        "eventValueThreshold": str,
-        "hpoConfig": HPOConfigOutputTypeDef,
-        "algorithmHyperParameters": Dict[str, str],
-        "featureTransformationParameters": Dict[str, str],
-        "autoMLConfig": AutoMLConfigOutputTypeDef,
-        "optimizationObjective": OptimizationObjectiveTypeDef,
-        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
         "hpoConfig": HPOConfigTypeDef,
         "algorithmHyperParameters": Mapping[str, str],
         "featureTransformationParameters": Mapping[str, str],
@@ -2450,36 +2378,63 @@
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
         "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
     total=False,
 )
 
+_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+    },
+)
+_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSolutionRequestRequestTypeDef",
+    {
+        "performHPO": bool,
+        "performAutoML": bool,
+        "recipeArn": str,
+        "eventType": str,
+        "solutionConfig": SolutionConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSolutionRequestRequestTypeDef(
+    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
+):
+    pass
+
+
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
-        "solutionConfig": SolutionConfigOutputTypeDef,
+        "solutionConfig": SolutionConfigTypeDef,
         "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
     total=False,
@@ -2492,54 +2447,26 @@
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
-        "solutionConfig": SolutionConfigOutputTypeDef,
+        "solutionConfig": SolutionConfigTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
         "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-    },
-)
-_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSolutionRequestRequestTypeDef",
-    {
-        "performHPO": bool,
-        "performAutoML": bool,
-        "recipeArn": str,
-        "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSolutionRequestRequestTypeDef(
-    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
-):
-    pass
-
-
-SolutionConfigUnionTypeDef = Union[SolutionConfigTypeDef, SolutionConfigOutputTypeDef]
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize/type_defs.pyi` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_personalize.type_defs import AlgorithmImageTypeDef
 
     data: AlgorithmImageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
     TrainingModeType,
@@ -30,41 +30,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlgorithmImageTypeDef",
-    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
-    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
-    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
-    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
-    "DatasetTypeDef",
+    "DatasetUpdateSummaryTypeDef",
     "DefaultCategoricalHyperParameterRangeTypeDef",
     "DefaultContinuousHyperParameterRangeTypeDef",
     "DefaultIntegerHyperParameterRangeTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteEventTrackerRequestRequestTypeDef",
@@ -119,30 +115,28 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
-    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchInferenceJobConfigUnionTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
     "CampaignUpdateSummaryTypeDef",
-    "CampaignConfigUnionTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
@@ -166,35 +160,35 @@
     "ListBatchInferenceJobsResponseTypeDef",
     "ListBatchSegmentJobsResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
+    "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DescribeDatasetResponseTypeDef",
+    "DatasetTypeDef",
     "DefaultHyperParameterRangesTypeDef",
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ListFiltersResponseTypeDef",
-    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
@@ -208,49 +202,45 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
-    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
+    "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
-    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
-    "RecommenderConfigUnionTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
-    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
     "ListRecommendersResponseTypeDef",
     "RecommenderTypeDef",
+    "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
-    "CreateSolutionRequestRequestTypeDef",
-    "SolutionConfigUnionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 _RequiredAlgorithmImageTypeDef = TypedDict(
     "_RequiredAlgorithmImageTypeDef",
@@ -265,23 +255,14 @@
     },
     total=False,
 )
 
 class AlgorithmImageTypeDef(_RequiredAlgorithmImageTypeDef, _OptionalAlgorithmImageTypeDef):
     pass
 
-AutoMLConfigOutputTypeDef = TypedDict(
-    "AutoMLConfigOutputTypeDef",
-    {
-        "metricName": str,
-        "recipeList": List[str],
-    },
-    total=False,
-)
-
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": str,
         "recipeList": Sequence[str],
     },
     total=False,
@@ -291,22 +272,14 @@
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": str,
     },
     total=False,
 )
 
-BatchInferenceJobConfigOutputTypeDef = TypedDict(
-    "BatchInferenceJobConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-    },
-    total=False,
-)
-
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
@@ -352,22 +325,14 @@
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
         "solutionVersionArn": str,
     },
     total=False,
 )
 
-CampaignConfigOutputTypeDef = TypedDict(
-    "CampaignConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-    },
-    total=False,
-)
-
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
     },
     total=False,
 )
@@ -381,23 +346,14 @@
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "failureReason": str,
     },
     total=False,
 )
 
-CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalHyperParameterRangeOutputTypeDef",
-    {
-        "name": str,
-        "values": List[str],
-    },
-    total=False,
-)
-
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
@@ -560,23 +516,20 @@
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
+DatasetUpdateSummaryTypeDef = TypedDict(
+    "DatasetUpdateSummaryTypeDef",
     {
-        "name": str,
-        "datasetArn": str,
-        "datasetGroupArn": str,
-        "datasetType": str,
         "schemaArn": str,
         "status": str,
+        "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
 DefaultCategoricalHyperParameterRangeTypeDef = TypedDict(
@@ -1146,22 +1099,14 @@
     {
         "itemAttribute": str,
         "objectiveSensitivity": ObjectiveSensitivityType,
     },
     total=False,
 )
 
-TrainingDataConfigOutputTypeDef = TypedDict(
-    "TrainingDataConfigOutputTypeDef",
-    {
-        "excludedDatasetColumns": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
         "excludedDatasetColumns": Mapping[str, Sequence[str]],
     },
     total=False,
 )
@@ -1199,17 +1144,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchInferenceJobConfigUnionTypeDef = Union[
-    BatchInferenceJobConfigTypeDef, BatchInferenceJobConfigOutputTypeDef
-]
+UpdateDatasetRequestRequestTypeDef = TypedDict(
+    "UpdateDatasetRequestRequestTypeDef",
+    {
+        "datasetArn": str,
+        "schemaArn": str,
+    },
+)
+
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 
@@ -1261,24 +1211,23 @@
     pass
 
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigOutputTypeDef,
+        "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-CampaignConfigUnionTypeDef = Union[CampaignConfigTypeDef, CampaignConfigOutputTypeDef]
 _RequiredUpdateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
 )
 _OptionalUpdateCampaignRequestRequestTypeDef = TypedDict(
@@ -1620,14 +1569,22 @@
     "UpdateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMetricAttributionResponseTypeDef = TypedDict(
     "UpdateMetricAttributionResponseTypeDef",
     {
         "metricAttributionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1749,20 +1706,28 @@
     {
         "datasets": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
     {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "datasetArn": str,
+        "datasetGroupArn": str,
+        "datasetType": str,
+        "schemaArn": str,
+        "status": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "latestDatasetUpdate": DatasetUpdateSummaryTypeDef,
     },
+    total=False,
 )
 
 DefaultHyperParameterRangesTypeDef = TypedDict(
     "DefaultHyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": List[DefaultIntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": List[DefaultContinuousHyperParameterRangeTypeDef],
@@ -1817,24 +1782,14 @@
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterRangesOutputTypeDef = TypedDict(
-    "HyperParameterRangesOutputTypeDef",
-    {
-        "integerHyperParameterRanges": List[IntegerHyperParameterRangeTypeDef],
-        "continuousHyperParameterRanges": List[ContinuousHyperParameterRangeTypeDef],
-        "categoricalHyperParameterRanges": List[CategoricalHyperParameterRangeOutputTypeDef],
-    },
-    total=False,
-)
-
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": Sequence[IntegerHyperParameterRangeTypeDef],
         "continuousHyperParameterRanges": Sequence[ContinuousHyperParameterRangeTypeDef],
         "categoricalHyperParameterRanges": Sequence[CategoricalHyperParameterRangeTypeDef],
     },
@@ -2016,24 +1971,14 @@
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecommenderConfigOutputTypeDef = TypedDict(
-    "RecommenderConfigOutputTypeDef",
-    {
-        "itemExplorationConfig": Dict[str, str],
-        "minRecommendationRequestsPerSecond": int,
-        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": Mapping[str, str],
         "minRecommendationRequestsPerSecond": int,
         "trainingDataConfig": TrainingDataConfigTypeDef,
     },
@@ -2047,15 +1992,15 @@
         "batchInferenceJobArn": str,
         "filterArn": str,
         "failureReason": str,
         "solutionVersionArn": str,
         "numResults": int,
         "jobInput": BatchInferenceJobInputTypeDef,
         "jobOutput": BatchInferenceJobOutputTypeDef,
-        "batchInferenceJobConfig": BatchInferenceJobConfigOutputTypeDef,
+        "batchInferenceJobConfig": BatchInferenceJobConfigTypeDef,
         "roleArn": str,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
@@ -2212,15 +2157,15 @@
 CampaignTypeDef = TypedDict(
     "CampaignTypeDef",
     {
         "name": str,
         "campaignArn": str,
         "solutionVersionArn": str,
         "minProvisionedTPS": int,
-        "campaignConfig": CampaignConfigOutputTypeDef,
+        "campaignConfig": CampaignConfigTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestCampaignUpdate": CampaignUpdateSummaryTypeDef,
     },
     total=False,
@@ -2230,14 +2175,22 @@
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AlgorithmTypeDef = TypedDict(
     "AlgorithmTypeDef",
     {
         "name": str,
         "algorithmArn": str,
         "algorithmImage": AlgorithmImageTypeDef,
         "defaultHyperParameters": Dict[str, str],
@@ -2247,84 +2200,73 @@
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-HPOConfigOutputTypeDef = TypedDict(
-    "HPOConfigOutputTypeDef",
+HPOConfigTypeDef = TypedDict(
+    "HPOConfigTypeDef",
     {
         "hpoObjective": HPOObjectiveTypeDef,
         "hpoResourceConfig": HPOResourceConfigTypeDef,
-        "algorithmHyperParameterRanges": HyperParameterRangesOutputTypeDef,
+        "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
     },
     total=False,
 )
 
-HPOConfigTypeDef = TypedDict(
-    "HPOConfigTypeDef",
+_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecommenderRequestRequestTypeDef",
     {
-        "hpoObjective": HPOObjectiveTypeDef,
-        "hpoResourceConfig": HPOResourceConfigTypeDef,
-        "algorithmHyperParameterRanges": HyperParameterRangesTypeDef,
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+    },
+)
+_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecommenderRequestRequestTypeDef",
+    {
+        "recommenderConfig": RecommenderConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+class CreateRecommenderRequestRequestTypeDef(
+    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
+):
+    pass
+
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": str,
         "recommenderArn": str,
         "datasetGroupArn": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
     },
     total=False,
 )
 
-_RequiredCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecommenderRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-    },
-)
-_OptionalCreateRecommenderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecommenderRequestRequestTypeDef",
-    {
-        "recommenderConfig": RecommenderConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateRecommenderRequestRequestTypeDef(
-    _RequiredCreateRecommenderRequestRequestTypeDef, _OptionalCreateRecommenderRequestRequestTypeDef
-):
-    pass
-
-RecommenderConfigUnionTypeDef = Union[RecommenderConfigTypeDef, RecommenderConfigOutputTypeDef]
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
@@ -2373,28 +2315,14 @@
     "DescribeAlgorithmResponseTypeDef",
     {
         "algorithm": AlgorithmTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SolutionConfigOutputTypeDef = TypedDict(
-    "SolutionConfigOutputTypeDef",
-    {
-        "eventValueThreshold": str,
-        "hpoConfig": HPOConfigOutputTypeDef,
-        "algorithmHyperParameters": Dict[str, str],
-        "featureTransformationParameters": Dict[str, str],
-        "autoMLConfig": AutoMLConfigOutputTypeDef,
-        "optimizationObjective": OptimizationObjectiveTypeDef,
-        "trainingDataConfig": TrainingDataConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": str,
         "hpoConfig": HPOConfigTypeDef,
         "algorithmHyperParameters": Mapping[str, str],
         "featureTransformationParameters": Mapping[str, str],
@@ -2417,36 +2345,61 @@
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": str,
         "datasetGroupArn": str,
         "name": str,
         "recipeArn": str,
-        "recommenderConfig": RecommenderConfigOutputTypeDef,
+        "recommenderConfig": RecommenderConfigTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "status": str,
         "failureReason": str,
         "latestRecommenderUpdate": RecommenderUpdateSummaryTypeDef,
         "modelMetrics": Dict[str, float],
     },
     total=False,
 )
 
+_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+    },
+)
+_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSolutionRequestRequestTypeDef",
+    {
+        "performHPO": bool,
+        "performAutoML": bool,
+        "recipeArn": str,
+        "eventType": str,
+        "solutionConfig": SolutionConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSolutionRequestRequestTypeDef(
+    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
+):
+    pass
+
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "datasetGroupArn": str,
         "eventType": str,
-        "solutionConfig": SolutionConfigOutputTypeDef,
+        "solutionConfig": SolutionConfigTypeDef,
         "autoMLResult": AutoMLResultTypeDef,
         "status": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "latestSolutionVersion": SolutionVersionSummaryTypeDef,
     },
     total=False,
@@ -2459,52 +2412,26 @@
         "solutionVersionArn": str,
         "solutionArn": str,
         "performHPO": bool,
         "performAutoML": bool,
         "recipeArn": str,
         "eventType": str,
         "datasetGroupArn": str,
-        "solutionConfig": SolutionConfigOutputTypeDef,
+        "solutionConfig": SolutionConfigTypeDef,
         "trainingHours": float,
         "trainingMode": TrainingModeType,
         "tunedHPOParams": TunedHPOParamsTypeDef,
         "status": str,
         "failureReason": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-    },
-)
-_OptionalCreateSolutionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSolutionRequestRequestTypeDef",
-    {
-        "performHPO": bool,
-        "performAutoML": bool,
-        "recipeArn": str,
-        "eventType": str,
-        "solutionConfig": SolutionConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSolutionRequestRequestTypeDef(
-    _RequiredCreateSolutionRequestRequestTypeDef, _OptionalCreateSolutionRequestRequestTypeDef
-):
-    pass
-
-SolutionConfigUnionTypeDef = Union[SolutionConfigTypeDef, SolutionConfigOutputTypeDef]
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-personalize-2.5.2.post1/types_aiobotocore_personalize.egg-info/SOURCES.txt` & `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

