# Comparing `tmp/types-aiobotocore-devops-guru-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-devops-guru-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devops-guru-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-devops-guru-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-devops-guru-2.5.2.post1.tar` & `types-aiobotocore-devops-guru-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.813607 types-aiobotocore-devops-guru-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-08-02 14:52:09.809607 types-aiobotocore-devops-guru-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.813607 types-aiobotocore-devops-guru-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.805607 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33147 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65266 2023-08-02 14:36:23.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65199 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.809607 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.859856 types-aiobotocore-devops-guru-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-08-04 12:00:44.859856 types-aiobotocore-devops-guru-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.859856 types-aiobotocore-devops-guru-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.859856 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33127 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62053 2023-08-04 11:43:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61988 2023-08-04 11:43:42.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:41.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.859856 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:00:44.000000 types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/LICENSE` & `types-aiobotocore-devops-guru-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/setup.py` & `types-aiobotocore-devops-guru-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devops-guru",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.pyi` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__main__.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DevOpsGuru 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DevOpsGuru 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterUnionTypeDef,
+    CostEstimationResourceCollectionFilterTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -69,15 +69,15 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigUnionTypeDef,
+    NotificationChannelConfigTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
     TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
@@ -126,15 +126,15 @@
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#exceptions)
         """
 
     async def add_notification_channel(
-        self, *, Config: NotificationChannelConfigUnionTypeDef
+        self, *, Config: NotificationChannelConfigTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#add_notification_channel)
         """
@@ -487,15 +487,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
 
     async def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
+        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.pyi` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterUnionTypeDef,
+    CostEstimationResourceCollectionFilterTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -69,15 +69,15 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigUnionTypeDef,
+    NotificationChannelConfigTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
     TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
@@ -121,15 +121,15 @@
         """
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#exceptions)
         """
     async def add_notification_channel(
-        self, *, Config: NotificationChannelConfigUnionTypeDef
+        self, *, Config: NotificationChannelConfigTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#add_notification_channel)
         """
@@ -452,15 +452,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
     async def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
+        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.pyi` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.pyi` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.py` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,32 +44,28 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInsightHealthTypeDef",
     "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
-    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
-    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
-    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
@@ -90,45 +86,41 @@
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
-    "NotificationFilterConfigOutputTypeDef",
-    "SnsChannelConfigTypeDef",
     "NotificationFilterConfigTypeDef",
+    "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
-    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
-    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
     "AddNotificationChannelResponseTypeDef",
     "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewResponseTypeDef",
     "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
-    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventTimeRangeTypeDef",
     "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
@@ -140,73 +132,69 @@
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
-    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
-    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
-    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
     "AnomalousLogGroupTypeDef",
-    "NotificationChannelTypeDef",
     "AddNotificationChannelRequestRequestTypeDef",
-    "NotificationChannelConfigUnionTypeDef",
+    "NotificationChannelTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
+    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
-    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
     "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     "ListInsightsRequestListInsightsPaginateTypeDef",
     "ListInsightsRequestRequestTypeDef",
     "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
@@ -261,21 +249,19 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
-
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -301,55 +287,37 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
-
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
-CloudFormationCollectionOutputTypeDef = TypedDict(
-    "CloudFormationCollectionOutputTypeDef",
-    {
-        "StackNames": List[str],
-    },
-    total=False,
-)
-
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
-        "StackNames": Sequence[str],
-    },
-    total=False,
-)
-
-CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
-    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": Sequence[str],
+        "StackNames": List[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -374,27 +342,19 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
-    {
-        "AppBoundaryKey": str,
-        "TagValues": List[str],
-    },
-)
-
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": Sequence[str],
+        "TagValues": List[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -421,21 +381,19 @@
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
-
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
@@ -459,21 +417,19 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
-
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
@@ -502,44 +458,40 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
@@ -576,41 +528,37 @@
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
-
 KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     {
         "KMSKeyId": str,
         "OptInStatus": OptInStatusType,
         "Type": ServerSideEncryptionTypeType,
     },
@@ -646,22 +594,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -693,22 +639,20 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -731,40 +675,31 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-NotificationFilterConfigOutputTypeDef = TypedDict(
-    "NotificationFilterConfigOutputTypeDef",
+NotificationFilterConfigTypeDef = TypedDict(
+    "NotificationFilterConfigTypeDef",
     {
-        "Severities": List[InsightSeverityType],
-        "MessageTypes": List[NotificationMessageTypeType],
+        "Severities": Sequence[InsightSeverityType],
+        "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
 SnsChannelConfigTypeDef = TypedDict(
     "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-NotificationFilterConfigTypeDef = TypedDict(
-    "NotificationFilterConfigTypeDef",
-    {
-        "Severities": Sequence[InsightSeverityType],
-        "MessageTypes": Sequence[NotificationMessageTypeType],
-    },
-    total=False,
-)
-
 OpsCenterIntegrationConfigTypeDef = TypedDict(
     "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
@@ -814,29 +749,19 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
-
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
-
-ServiceCollectionOutputTypeDef = TypedDict(
-    "ServiceCollectionOutputTypeDef",
-    {
-        "ServiceNames": List[ServiceNameType],
-    },
-    total=False,
-)
-
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -871,27 +796,19 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-TagCollectionOutputTypeDef = TypedDict(
-    "TagCollectionOutputTypeDef",
-    {
-        "AppBoundaryKey": str,
-        "TagValues": List[str],
-    },
-)
-
 TagCollectionTypeDef = TypedDict(
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": Sequence[str],
+        "TagValues": List[str],
     },
 )
 
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
@@ -1009,28 +926,19 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
-CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "CostEstimationResourceCollectionFilterOutputTypeDef",
-    {
-        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
@@ -1041,22 +949,20 @@
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": TimestampTypeDef,
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -1065,22 +971,20 @@
         "ToTime": TimestampTypeDef,
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
-
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": TimestampTypeDef,
         "ToTime": TimestampTypeDef,
     },
     total=False,
@@ -1132,44 +1036,40 @@
         "OrganizationalUnitIds": Sequence[str],
         "MaxResults": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
-
 GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1184,44 +1084,40 @@
     "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
     _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
     "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
     _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
 ):
     pass
 
-
 ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1238,22 +1134,20 @@
         "Locale": LocaleType,
         "AccountId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
-
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1281,56 +1175,33 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
-_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
-    "_RequiredNotificationChannelConfigOutputTypeDef",
-    {
-        "Sns": SnsChannelConfigTypeDef,
-    },
-)
-_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
-    "_OptionalNotificationChannelConfigOutputTypeDef",
-    {
-        "Filters": NotificationFilterConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class NotificationChannelConfigOutputTypeDef(
-    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
-
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
-
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
         "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
@@ -1379,28 +1250,19 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
-ResourceCollectionOutputTypeDef = TypedDict(
-    "ResourceCollectionOutputTypeDef",
-    {
-        "CloudFormation": CloudFormationCollectionOutputTypeDef,
-        "Tags": List[TagCollectionOutputTypeDef],
-    },
-    total=False,
-)
-
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": Sequence[TagCollectionTypeDef],
+        "Tags": List[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1449,50 +1311,44 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CostEstimationResourceCollectionFilterUnionTypeDef = Union[
-    CostEstimationResourceCollectionFilterTypeDef,
-    CostEstimationResourceCollectionFilterOutputTypeDef,
-]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
-
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
@@ -1518,22 +1374,20 @@
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1544,53 +1398,48 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
-
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
-
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
-        "Config": NotificationChannelConfigOutputTypeDef,
+        "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
+        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelConfigUnionTypeDef = Union[
-    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
-]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
@@ -1628,64 +1477,77 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
+        "ResourceCollection": ResourceCollectionTypeDef,
+    },
+    total=False,
+)
+
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1695,44 +1557,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1741,29 +1603,16 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
-    },
-    total=False,
-)
-
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1874,14 +1723,56 @@
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1932,60 +1823,14 @@
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1995,21 +1840,19 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -2018,22 +1861,20 @@
     {
         "Filters": SearchInsightsFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2044,22 +1885,20 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2069,44 +1908,40 @@
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -2114,21 +1949,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
@@ -2137,22 +1970,20 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -2162,22 +1993,20 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
-
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
@@ -2222,15 +2051,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2243,15 +2072,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2262,15 +2091,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2282,15 +2111,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
```

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.pyi` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,29 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountInsightHealthTypeDef",
     "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
-    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
-    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
-    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
@@ -89,45 +87,41 @@
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
-    "NotificationFilterConfigOutputTypeDef",
-    "SnsChannelConfigTypeDef",
     "NotificationFilterConfigTypeDef",
+    "SnsChannelConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
-    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
-    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
     "AddNotificationChannelResponseTypeDef",
     "DescribeAccountHealthResponseTypeDef",
     "DescribeAccountOverviewResponseTypeDef",
     "DescribeOrganizationHealthResponseTypeDef",
     "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
-    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
     "DescribeAccountOverviewRequestRequestTypeDef",
     "DescribeOrganizationOverviewRequestRequestTypeDef",
     "EndTimeRangeTypeDef",
     "EventTimeRangeTypeDef",
     "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
@@ -139,73 +133,69 @@
     "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
-    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
-    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
-    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
     "ListInsightsClosedStatusFilterTypeDef",
     "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
     "AnomalousLogGroupTypeDef",
-    "NotificationChannelTypeDef",
     "AddNotificationChannelRequestRequestTypeDef",
-    "NotificationChannelConfigUnionTypeDef",
+    "NotificationChannelTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
+    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
-    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
     "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     "ListInsightsRequestListInsightsPaginateTypeDef",
     "ListInsightsRequestRequestTypeDef",
     "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
@@ -260,19 +250,21 @@
     "_OptionalAnomalyReportedTimeRangeTypeDef",
     {
         "CloseTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyReportedTimeRangeTypeDef(
     _RequiredAnomalyReportedTimeRangeTypeDef, _OptionalAnomalyReportedTimeRangeTypeDef
 ):
     pass
 
+
 AnomalyResourceTypeDef = TypedDict(
     "AnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -298,53 +290,39 @@
     "_OptionalAnomalyTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class AnomalyTimeRangeTypeDef(_RequiredAnomalyTimeRangeTypeDef, _OptionalAnomalyTimeRangeTypeDef):
     pass
 
+
 CloudFormationCollectionFilterTypeDef = TypedDict(
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
-CloudFormationCollectionOutputTypeDef = TypedDict(
-    "CloudFormationCollectionOutputTypeDef",
-    {
-        "StackNames": List[str],
-    },
-    total=False,
-)
-
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
-        "StackNames": Sequence[str],
-    },
-    total=False,
-)
-
-CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
-    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": Sequence[str],
+        "StackNames": List[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -369,27 +347,19 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
-    {
-        "AppBoundaryKey": str,
-        "TagValues": List[str],
-    },
-)
-
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": Sequence[str],
+        "TagValues": List[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -416,19 +386,21 @@
     "_OptionalDescribeAnomalyRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeAnomalyRequestRequestTypeDef(
     _RequiredDescribeAnomalyRequestRequestTypeDef, _OptionalDescribeAnomalyRequestRequestTypeDef
 ):
     pass
 
+
 DescribeFeedbackRequestRequestTypeDef = TypedDict(
     "DescribeFeedbackRequestRequestTypeDef",
     {
         "InsightId": str,
     },
     total=False,
 )
@@ -452,19 +424,21 @@
     "_OptionalDescribeInsightRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DescribeInsightRequestRequestTypeDef(
     _RequiredDescribeInsightRequestRequestTypeDef, _OptionalDescribeInsightRequestRequestTypeDef
 ):
     pass
 
+
 DescribeOrganizationHealthRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationHealthRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
@@ -493,40 +467,44 @@
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
+
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
@@ -563,37 +541,41 @@
     "_OptionalGetResourceCollectionRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetResourceCollectionRequestRequestTypeDef(
     _RequiredGetResourceCollectionRequestRequestTypeDef,
     _OptionalGetResourceCollectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredInsightTimeRangeTypeDef = TypedDict(
     "_RequiredInsightTimeRangeTypeDef",
     {
         "StartTime": datetime,
     },
 )
 _OptionalInsightTimeRangeTypeDef = TypedDict(
     "_OptionalInsightTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class InsightTimeRangeTypeDef(_RequiredInsightTimeRangeTypeDef, _OptionalInsightTimeRangeTypeDef):
     pass
 
+
 KMSServerSideEncryptionIntegrationConfigTypeDef = TypedDict(
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     {
         "KMSKeyId": str,
         "OptInStatus": OptInStatusType,
         "Type": ServerSideEncryptionTypeType,
     },
@@ -629,20 +611,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAnomalousLogGroupsRequestRequestTypeDef(
     _RequiredListAnomalousLogGroupsRequestRequestTypeDef,
     _OptionalListAnomalousLogGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsOngoingStatusFilterTypeDef = TypedDict(
     "ListInsightsOngoingStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
     },
 )
 
@@ -674,20 +658,22 @@
         "NextToken": str,
         "Locale": LocaleType,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 LogAnomalyClassTypeDef = TypedDict(
     "LogAnomalyClassTypeDef",
     {
         "LogStreamName": str,
         "LogAnomalyType": LogAnomalyTypeType,
         "LogAnomalyToken": str,
         "LogEventId": str,
@@ -710,40 +696,31 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-NotificationFilterConfigOutputTypeDef = TypedDict(
-    "NotificationFilterConfigOutputTypeDef",
+NotificationFilterConfigTypeDef = TypedDict(
+    "NotificationFilterConfigTypeDef",
     {
-        "Severities": List[InsightSeverityType],
-        "MessageTypes": List[NotificationMessageTypeType],
+        "Severities": Sequence[InsightSeverityType],
+        "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
 SnsChannelConfigTypeDef = TypedDict(
     "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-NotificationFilterConfigTypeDef = TypedDict(
-    "NotificationFilterConfigTypeDef",
-    {
-        "Severities": Sequence[InsightSeverityType],
-        "MessageTypes": Sequence[NotificationMessageTypeType],
-    },
-    total=False,
-)
-
 OpsCenterIntegrationConfigTypeDef = TypedDict(
     "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
@@ -793,26 +770,20 @@
     "_OptionalPredictionTimeRangeTypeDef",
     {
         "EndTime": datetime,
     },
     total=False,
 )
 
+
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
-ServiceCollectionOutputTypeDef = TypedDict(
-    "ServiceCollectionOutputTypeDef",
-    {
-        "ServiceNames": List[ServiceNameType],
-    },
-    total=False,
-)
 
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
@@ -848,27 +819,19 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-TagCollectionOutputTypeDef = TypedDict(
-    "TagCollectionOutputTypeDef",
-    {
-        "AppBoundaryKey": str,
-        "TagValues": List[str],
-    },
-)
-
 TagCollectionTypeDef = TypedDict(
     "TagCollectionTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": Sequence[str],
+        "TagValues": List[str],
     },
 )
 
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
@@ -986,28 +949,19 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
-CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
-    "CostEstimationResourceCollectionFilterOutputTypeDef",
-    {
-        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
     {
@@ -1018,20 +972,22 @@
     "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
     {
         "ToTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAccountOverviewRequestRequestTypeDef(
     _RequiredDescribeAccountOverviewRequestRequestTypeDef,
     _OptionalDescribeAccountOverviewRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
     {
         "FromTime": TimestampTypeDef,
     },
 )
 _OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
@@ -1040,20 +996,22 @@
         "ToTime": TimestampTypeDef,
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeOrganizationOverviewRequestRequestTypeDef(
     _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
     _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
 ):
     pass
 
+
 EndTimeRangeTypeDef = TypedDict(
     "EndTimeRangeTypeDef",
     {
         "FromTime": TimestampTypeDef,
         "ToTime": TimestampTypeDef,
     },
     total=False,
@@ -1105,40 +1063,44 @@
         "OrganizationalUnitIds": Sequence[str],
         "MaxResults": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
     "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
 ):
     pass
 
+
 GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
     "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1153,40 +1115,44 @@
     "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
     _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
     "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
     _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
 ):
     pass
 
+
 ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
     "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1203,20 +1169,22 @@
         "Locale": LocaleType,
         "AccountId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
     _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
     _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
 ):
     pass
 
+
 ListAnomaliesForInsightFiltersTypeDef = TypedDict(
     "ListAnomaliesForInsightFiltersTypeDef",
     {
         "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
@@ -1244,52 +1212,35 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
-_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
-    "_RequiredNotificationChannelConfigOutputTypeDef",
-    {
-        "Sns": SnsChannelConfigTypeDef,
-    },
-)
-_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
-    "_OptionalNotificationChannelConfigOutputTypeDef",
-    {
-        "Filters": NotificationFilterConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class NotificationChannelConfigOutputTypeDef(
-    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
-):
-    pass
-
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
     "_OptionalNotificationChannelConfigTypeDef",
     {
         "Filters": NotificationFilterConfigTypeDef,
     },
     total=False,
 )
 
+
 class NotificationChannelConfigTypeDef(
     _RequiredNotificationChannelConfigTypeDef, _OptionalNotificationChannelConfigTypeDef
 ):
     pass
 
+
 UpdateServiceIntegrationConfigTypeDef = TypedDict(
     "UpdateServiceIntegrationConfigTypeDef",
     {
         "OpsCenter": OpsCenterIntegrationConfigTypeDef,
         "LogsAnomalyDetection": LogsAnomalyDetectionIntegrationConfigTypeDef,
         "KMSServerSideEncryption": KMSServerSideEncryptionIntegrationConfigTypeDef,
     },
@@ -1338,28 +1289,19 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
-ResourceCollectionOutputTypeDef = TypedDict(
-    "ResourceCollectionOutputTypeDef",
-    {
-        "CloudFormation": CloudFormationCollectionOutputTypeDef,
-        "Tags": List[TagCollectionOutputTypeDef],
-    },
-    total=False,
-)
-
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": Sequence[TagCollectionTypeDef],
+        "Tags": List[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1408,48 +1350,46 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CostEstimationResourceCollectionFilterUnionTypeDef = Union[
-    CostEstimationResourceCollectionFilterTypeDef,
-    CostEstimationResourceCollectionFilterOutputTypeDef,
-]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_OptionalStartCostEstimationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
+
 ListInsightsClosedStatusFilterTypeDef = TypedDict(
     "ListInsightsClosedStatusFilterTypeDef",
     {
         "Type": InsightTypeType,
         "EndTimeRange": EndTimeRangeTypeDef,
     },
 )
@@ -1475,20 +1415,22 @@
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestRequestTypeDef = TypedDict(
@@ -1499,51 +1441,50 @@
         "NextToken": str,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
     },
     total=False,
 )
 
+
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
+
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
-        "Config": NotificationChannelConfigOutputTypeDef,
+        "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
+        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelConfigUnionTypeDef = Union[
-    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
-]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
@@ -1581,64 +1522,77 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
+        "ResourceCollection": ResourceCollectionTypeDef,
+    },
+    total=False,
+)
+
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1648,44 +1602,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1694,29 +1648,16 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
-        "ServiceCollection": ServiceCollectionOutputTypeDef,
-    },
-    total=False,
-)
-
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
+        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1827,14 +1768,60 @@
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
+
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1885,56 +1872,14 @@
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1944,19 +1889,21 @@
         "Filters": SearchInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchInsightsRequestRequestTypeDef(
     _RequiredSearchInsightsRequestRequestTypeDef, _OptionalSearchInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1965,20 +1912,22 @@
     {
         "Filters": SearchInsightsFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestRequestTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -1989,20 +1938,22 @@
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestRequestTypeDef(
     _RequiredSearchOrganizationInsightsRequestRequestTypeDef,
     _OptionalSearchOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "AccountIds": Sequence[str],
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -2012,40 +1963,44 @@
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
     "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListInsightsRequestListInsightsPaginateTypeDef(
     _RequiredListInsightsRequestListInsightsPaginateTypeDef,
     _OptionalListInsightsRequestListInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListInsightsRequestRequestTypeDef = TypedDict(
@@ -2053,19 +2008,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListInsightsRequestRequestTypeDef(
     _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
@@ -2074,20 +2031,22 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
     _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
     _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredListOrganizationInsightsRequestRequestTypeDef",
     {
         "StatusFilter": ListInsightsStatusFilterTypeDef,
     },
 )
 _OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
@@ -2097,20 +2056,22 @@
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListOrganizationInsightsRequestRequestTypeDef(
     _RequiredListOrganizationInsightsRequestRequestTypeDef,
     _OptionalListOrganizationInsightsRequestRequestTypeDef,
 ):
     pass
 
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
@@ -2155,15 +2116,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2176,15 +2137,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2195,15 +2156,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2215,15 +2176,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ResourceCollection": ResourceCollectionTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
```

### Comparing `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt` & `types-aiobotocore-devops-guru-2.5.2.post2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

