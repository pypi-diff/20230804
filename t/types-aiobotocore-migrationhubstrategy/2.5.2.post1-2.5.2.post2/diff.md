# Comparing `tmp/types-aiobotocore-migrationhubstrategy-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-migrationhubstrategy-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhubstrategy-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhubstrategy-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1.tar` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.585514 types-aiobotocore-migrationhubstrategy-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-08-02 14:52:42.585514 types-aiobotocore-migrationhubstrategy-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:42.585514 types-aiobotocore-migrationhubstrategy-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.585514 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-08-02 14:43:46.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-08-02 14:43:46.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34973 2023-08-02 14:43:47.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34962 2023-08-02 14:43:47.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:44.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.585514 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:42.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.106643 types-aiobotocore-migrationhubstrategy-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14458 2023-08-04 13:59:19.106643 types-aiobotocore-migrationhubstrategy-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12873 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.106643 types-aiobotocore-migrationhubstrategy-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2170 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.106643 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1702 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1701 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1025 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22477 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22442 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15759 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15757 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7600 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7593 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31728 2023-08-04 13:45:12.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31717 2023-08-04 13:45:12.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:11.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.106643 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14458 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1060 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       39 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/LICENSE` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/setup.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migrationhubstrategy",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MigrationHubStrategyRecommendations 2.5.2 service"
-        " generated with mypy-boto3-builder 7.17.1"
+        " generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__init__.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__init__.pyi` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/__main__.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MigrationHubStrategyRecommendations 2.5.2\nVersion:      "
-        "   2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        "   2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhubstrategy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
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

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/client.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
-    ApplicationPreferencesUnionTypeDef,
-    AssessmentTargetUnionTypeDef,
-    DatabasePreferencesUnionTypeDef,
+    ApplicationPreferencesTypeDef,
+    AssessmentTargetTypeDef,
+    DatabasePreferencesTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
     GetPortfolioSummaryResponseTypeDef,
@@ -285,29 +285,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhubstrategy/client/#list_servers)
         """
 
     async def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: ApplicationPreferencesUnionTypeDef = ...,
-        databasePreferences: DatabasePreferencesUnionTypeDef = ...,
+        applicationPreferences: ApplicationPreferencesTypeDef = ...,
+        databasePreferences: DatabasePreferencesTypeDef = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhubstrategy/client/#put_portfolio_preferences)
         """
 
     async def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[AssessmentTargetUnionTypeDef] = ...,
+        assessmentTargets: Sequence[AssessmentTargetTypeDef] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/client.pyi` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
-    ApplicationPreferencesUnionTypeDef,
-    AssessmentTargetUnionTypeDef,
-    DatabasePreferencesUnionTypeDef,
+    ApplicationPreferencesTypeDef,
+    AssessmentTargetTypeDef,
+    DatabasePreferencesTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
     GetPortfolioSummaryResponseTypeDef,
@@ -263,28 +263,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.list_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhubstrategy/client/#list_servers)
         """
     async def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: ApplicationPreferencesUnionTypeDef = ...,
-        databasePreferences: DatabasePreferencesUnionTypeDef = ...,
+        applicationPreferences: ApplicationPreferencesTypeDef = ...,
+        databasePreferences: DatabasePreferencesTypeDef = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhubstrategy/client/#put_portfolio_preferences)
         """
     async def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[AssessmentTargetUnionTypeDef] = ...,
+        assessmentTargets: Sequence[AssessmentTargetTypeDef] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/literals.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "AntipatternReportStatusType",
     "AppTypeType",
     "AppUnitErrorCategoryType",
     "ApplicationComponentCriteriaType",
     "ApplicationModeType",
@@ -71,15 +70,14 @@
     "MigrationHubStrategyRecommendationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalysisTypeType = Literal[
     "BINARY_ANALYSIS", "DATABASE_ANALYSIS", "RUNTIME_ANALYSIS", "SOURCE_CODE_ANALYSIS"
 ]
 AntipatternReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 AppTypeType = Literal[
     "Cassandra",
     "DB2",
@@ -281,14 +279,15 @@
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
@@ -384,14 +383,15 @@
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
@@ -470,26 +470,28 @@
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

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/literals.pyi` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisTypeType",
     "AntipatternReportStatusType",
     "AppTypeType",
     "AppUnitErrorCategoryType",
     "ApplicationComponentCriteriaType",
     "ApplicationModeType",
@@ -70,14 +71,15 @@
     "MigrationHubStrategyRecommendationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AnalysisTypeType = Literal[
     "BINARY_ANALYSIS", "DATABASE_ANALYSIS", "RUNTIME_ANALYSIS", "SOURCE_CODE_ANALYSIS"
 ]
 AntipatternReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 AppTypeType = Literal[
     "Cassandra",
     "DB2",
@@ -279,14 +281,15 @@
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
@@ -382,14 +385,15 @@
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
@@ -468,26 +472,28 @@
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

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/paginator.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/paginator.pyi` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/type_defs.py` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
     data: AnalysisStatusUnionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AnalysisTypeType,
     AntipatternReportStatusType,
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -78,29 +78,24 @@
     "DatabaseConfigDetailTypeDef",
     "SourceCodeRepositoryTypeDef",
     "ApplicationComponentStatusSummaryTypeDef",
     "ApplicationComponentSummaryTypeDef",
     "ServerStatusSummaryTypeDef",
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
-    "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
-    "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
-    "HeterogeneousOutputTypeDef",
-    "HomogeneousOutputTypeDef",
-    "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
@@ -110,31 +105,28 @@
     "PaginatorConfigTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
     "ListCollectorsRequestRequestTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
-    "NoManagementPreferenceOutputTypeDef",
-    "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
     "TransformationToolTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
-    "AssessmentTargetUnionTypeDef",
+    "StartAssessmentRequestRequestTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
     "GetImportFileTaskResponseTypeDef",
     "GetLatestAssessmentIdResponseTypeDef",
     "StartAssessmentResponseTypeDef",
     "StartImportFileTaskResponseTypeDef",
     "StartRecommendationReportGenerationResponseTypeDef",
@@ -145,36 +137,30 @@
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
-    "ManagementPreferenceOutputTypeDef",
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
-    "StartAssessmentRequestRequestTypeDef",
     "CollectorTypeDef",
-    "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
-    "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
-    "DatabasePreferencesUnionTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
-    "ApplicationPreferencesUnionTypeDef",
     "PutPortfolioPreferencesRequestRequestTypeDef",
     "GetApplicationComponentStrategiesResponseTypeDef",
     "GetServerDetailsResponseTypeDef",
     "ListServersResponseTypeDef",
     "GetServerStrategiesResponseTypeDef",
     "GetApplicationComponentDetailsResponseTypeDef",
     "ListApplicationComponentsResponseTypeDef",
@@ -285,52 +271,36 @@
     {
         "count": int,
         "strategy": StrategyType,
     },
     total=False,
 )
 
-AssessmentTargetOutputTypeDef = TypedDict(
-    "AssessmentTargetOutputTypeDef",
-    {
-        "condition": ConditionType,
-        "name": str,
-        "values": List[str],
-    },
-)
-
 AssessmentTargetTypeDef = TypedDict(
     "AssessmentTargetTypeDef",
     {
         "condition": ConditionType,
         "name": str,
-        "values": Sequence[str],
+        "values": List[str],
     },
 )
 
 AssociatedApplicationTypeDef = TypedDict(
     "AssociatedApplicationTypeDef",
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-AwsManagedResourcesOutputTypeDef = TypedDict(
-    "AwsManagedResourcesOutputTypeDef",
-    {
-        "targetDestination": List[AwsManagedTargetDestinationType],
-    },
-)
-
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
-        "targetDestination": Sequence[AwsManagedTargetDestinationType],
+        "targetDestination": List[AwsManagedTargetDestinationType],
     },
 )
 
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
@@ -397,55 +367,33 @@
         "status": AssessmentStatusType,
         "statusMessage": str,
         "success": int,
     },
     total=False,
 )
 
-HeterogeneousOutputTypeDef = TypedDict(
-    "HeterogeneousOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
-    },
-)
-
-HomogeneousOutputTypeDef = TypedDict(
-    "HomogeneousOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[Literal["None specified"]],
-    },
-    total=False,
-)
-
-NoDatabaseMigrationPreferenceOutputTypeDef = TypedDict(
-    "NoDatabaseMigrationPreferenceOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[TargetDatabaseEngineType],
-    },
-)
-
 HeterogeneousTypeDef = TypedDict(
     "HeterogeneousTypeDef",
     {
-        "targetDatabaseEngine": Sequence[HeterogeneousTargetDatabaseEngineType],
+        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
     },
 )
 
 HomogeneousTypeDef = TypedDict(
     "HomogeneousTypeDef",
     {
-        "targetDatabaseEngine": Sequence[Literal["None specified"]],
+        "targetDatabaseEngine": List[Literal["None specified"]],
     },
     total=False,
 )
 
 NoDatabaseMigrationPreferenceTypeDef = TypedDict(
     "NoDatabaseMigrationPreferenceTypeDef",
     {
-        "targetDatabaseEngine": Sequence[TargetDatabaseEngineType],
+        "targetDatabaseEngine": List[TargetDatabaseEngineType],
     },
 )
 
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
@@ -584,39 +532,25 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-NoManagementPreferenceOutputTypeDef = TypedDict(
-    "NoManagementPreferenceOutputTypeDef",
-    {
-        "targetDestination": List[NoPreferenceTargetDestinationType],
-    },
-)
-
-SelfManageResourcesOutputTypeDef = TypedDict(
-    "SelfManageResourcesOutputTypeDef",
-    {
-        "targetDestination": List[SelfManageTargetDestinationType],
-    },
-)
-
 NoManagementPreferenceTypeDef = TypedDict(
     "NoManagementPreferenceTypeDef",
     {
-        "targetDestination": Sequence[NoPreferenceTargetDestinationType],
+        "targetDestination": List[NoPreferenceTargetDestinationType],
     },
 )
 
 SelfManageResourcesTypeDef = TypedDict(
     "SelfManageResourcesTypeDef",
     {
-        "targetDestination": Sequence[SelfManageTargetDestinationType],
+        "targetDestination": List[SelfManageTargetDestinationType],
     },
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "interfaceName": str,
@@ -707,15 +641,24 @@
         "listServerStatusSummary": List[ServerStatusSummaryTypeDef],
         "listServerStrategySummary": List[StrategySummaryTypeDef],
         "listServerSummary": List[ServerSummaryTypeDef],
     },
     total=False,
 )
 
-AssessmentTargetUnionTypeDef = Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+StartAssessmentRequestRequestTypeDef = TypedDict(
+    "StartAssessmentRequestRequestTypeDef",
+    {
+        "assessmentTargets": Sequence[AssessmentTargetTypeDef],
+        "s3bucketForAnalysisData": str,
+        "s3bucketForReportData": str,
+    },
+    total=False,
+)
+
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -728,38 +671,28 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
-    "DatabaseMigrationPreferenceOutputTypeDef",
-    {
-        "heterogeneous": HeterogeneousOutputTypeDef,
-        "homogeneous": HomogeneousOutputTypeDef,
-        "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 DatabaseMigrationPreferenceTypeDef = TypedDict(
     "DatabaseMigrationPreferenceTypeDef",
     {
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
-        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
+        "assessmentTargets": List[AssessmentTargetTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportFileTaskResponseTypeDef = TypedDict(
@@ -949,24 +882,14 @@
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ManagementPreferenceOutputTypeDef = TypedDict(
-    "ManagementPreferenceOutputTypeDef",
-    {
-        "awsManagedResources": AwsManagedResourcesOutputTypeDef,
-        "noPreference": NoManagementPreferenceOutputTypeDef,
-        "selfManageResources": SelfManageResourcesOutputTypeDef,
-    },
-    total=False,
-)
-
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
         "noPreference": NoManagementPreferenceTypeDef,
         "selfManageResources": SelfManageResourcesTypeDef,
     },
@@ -1058,24 +981,14 @@
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentRequestRequestTypeDef = TypedDict(
-    "StartAssessmentRequestRequestTypeDef",
-    {
-        "assessmentTargets": Sequence[AssessmentTargetUnionTypeDef],
-        "s3bucketForAnalysisData": str,
-        "s3bucketForReportData": str,
-    },
-    total=False,
-)
-
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
         "collectorId": str,
         "collectorVersion": str,
         "configurationSummary": ConfigurationSummaryTypeDef,
@@ -1083,40 +996,23 @@
         "ipAddress": str,
         "lastActivityTimeStamp": str,
         "registeredTimeStamp": str,
     },
     total=False,
 )
 
-DatabasePreferencesOutputTypeDef = TypedDict(
-    "DatabasePreferencesOutputTypeDef",
-    {
-        "databaseManagementPreference": DatabaseManagementPreferenceType,
-        "databaseMigrationPreference": DatabaseMigrationPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 DatabasePreferencesTypeDef = TypedDict(
     "DatabasePreferencesTypeDef",
     {
         "databaseManagementPreference": DatabaseManagementPreferenceType,
         "databaseMigrationPreference": DatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
-ApplicationPreferencesOutputTypeDef = TypedDict(
-    "ApplicationPreferencesOutputTypeDef",
-    {
-        "managementPreference": ManagementPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationPreferencesTypeDef = TypedDict(
     "ApplicationPreferencesTypeDef",
     {
         "managementPreference": ManagementPreferenceTypeDef,
     },
     total=False,
 )
@@ -1198,31 +1094,25 @@
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabasePreferencesUnionTypeDef = Union[
-    DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
-]
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
-        "applicationPreferences": ApplicationPreferencesOutputTypeDef,
-        "databasePreferences": DatabasePreferencesOutputTypeDef,
+        "applicationPreferences": ApplicationPreferencesTypeDef,
+        "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApplicationPreferencesUnionTypeDef = Union[
-    ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
-]
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy/type_defs.pyi` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
     data: AnalysisStatusUnionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AnalysisTypeType,
     AntipatternReportStatusType,
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -77,29 +77,24 @@
     "DatabaseConfigDetailTypeDef",
     "SourceCodeRepositoryTypeDef",
     "ApplicationComponentStatusSummaryTypeDef",
     "ApplicationComponentSummaryTypeDef",
     "ServerStatusSummaryTypeDef",
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
-    "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
-    "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
-    "HeterogeneousOutputTypeDef",
-    "HomogeneousOutputTypeDef",
-    "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
@@ -109,31 +104,28 @@
     "PaginatorConfigTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
     "ListCollectorsRequestRequestTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
-    "NoManagementPreferenceOutputTypeDef",
-    "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
     "TransformationToolTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
-    "AssessmentTargetUnionTypeDef",
+    "StartAssessmentRequestRequestTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
     "GetImportFileTaskResponseTypeDef",
     "GetLatestAssessmentIdResponseTypeDef",
     "StartAssessmentResponseTypeDef",
     "StartImportFileTaskResponseTypeDef",
     "StartRecommendationReportGenerationResponseTypeDef",
@@ -144,36 +136,30 @@
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
-    "ManagementPreferenceOutputTypeDef",
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
-    "StartAssessmentRequestRequestTypeDef",
     "CollectorTypeDef",
-    "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
-    "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
-    "DatabasePreferencesUnionTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
-    "ApplicationPreferencesUnionTypeDef",
     "PutPortfolioPreferencesRequestRequestTypeDef",
     "GetApplicationComponentStrategiesResponseTypeDef",
     "GetServerDetailsResponseTypeDef",
     "ListServersResponseTypeDef",
     "GetServerStrategiesResponseTypeDef",
     "GetApplicationComponentDetailsResponseTypeDef",
     "ListApplicationComponentsResponseTypeDef",
@@ -284,52 +270,36 @@
     {
         "count": int,
         "strategy": StrategyType,
     },
     total=False,
 )
 
-AssessmentTargetOutputTypeDef = TypedDict(
-    "AssessmentTargetOutputTypeDef",
-    {
-        "condition": ConditionType,
-        "name": str,
-        "values": List[str],
-    },
-)
-
 AssessmentTargetTypeDef = TypedDict(
     "AssessmentTargetTypeDef",
     {
         "condition": ConditionType,
         "name": str,
-        "values": Sequence[str],
+        "values": List[str],
     },
 )
 
 AssociatedApplicationTypeDef = TypedDict(
     "AssociatedApplicationTypeDef",
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-AwsManagedResourcesOutputTypeDef = TypedDict(
-    "AwsManagedResourcesOutputTypeDef",
-    {
-        "targetDestination": List[AwsManagedTargetDestinationType],
-    },
-)
-
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
-        "targetDestination": Sequence[AwsManagedTargetDestinationType],
+        "targetDestination": List[AwsManagedTargetDestinationType],
     },
 )
 
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
@@ -396,55 +366,33 @@
         "status": AssessmentStatusType,
         "statusMessage": str,
         "success": int,
     },
     total=False,
 )
 
-HeterogeneousOutputTypeDef = TypedDict(
-    "HeterogeneousOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
-    },
-)
-
-HomogeneousOutputTypeDef = TypedDict(
-    "HomogeneousOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[Literal["None specified"]],
-    },
-    total=False,
-)
-
-NoDatabaseMigrationPreferenceOutputTypeDef = TypedDict(
-    "NoDatabaseMigrationPreferenceOutputTypeDef",
-    {
-        "targetDatabaseEngine": List[TargetDatabaseEngineType],
-    },
-)
-
 HeterogeneousTypeDef = TypedDict(
     "HeterogeneousTypeDef",
     {
-        "targetDatabaseEngine": Sequence[HeterogeneousTargetDatabaseEngineType],
+        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
     },
 )
 
 HomogeneousTypeDef = TypedDict(
     "HomogeneousTypeDef",
     {
-        "targetDatabaseEngine": Sequence[Literal["None specified"]],
+        "targetDatabaseEngine": List[Literal["None specified"]],
     },
     total=False,
 )
 
 NoDatabaseMigrationPreferenceTypeDef = TypedDict(
     "NoDatabaseMigrationPreferenceTypeDef",
     {
-        "targetDatabaseEngine": Sequence[TargetDatabaseEngineType],
+        "targetDatabaseEngine": List[TargetDatabaseEngineType],
     },
 )
 
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
@@ -581,39 +529,25 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-NoManagementPreferenceOutputTypeDef = TypedDict(
-    "NoManagementPreferenceOutputTypeDef",
-    {
-        "targetDestination": List[NoPreferenceTargetDestinationType],
-    },
-)
-
-SelfManageResourcesOutputTypeDef = TypedDict(
-    "SelfManageResourcesOutputTypeDef",
-    {
-        "targetDestination": List[SelfManageTargetDestinationType],
-    },
-)
-
 NoManagementPreferenceTypeDef = TypedDict(
     "NoManagementPreferenceTypeDef",
     {
-        "targetDestination": Sequence[NoPreferenceTargetDestinationType],
+        "targetDestination": List[NoPreferenceTargetDestinationType],
     },
 )
 
 SelfManageResourcesTypeDef = TypedDict(
     "SelfManageResourcesTypeDef",
     {
-        "targetDestination": Sequence[SelfManageTargetDestinationType],
+        "targetDestination": List[SelfManageTargetDestinationType],
     },
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "interfaceName": str,
@@ -704,15 +638,24 @@
         "listServerStatusSummary": List[ServerStatusSummaryTypeDef],
         "listServerStrategySummary": List[StrategySummaryTypeDef],
         "listServerSummary": List[ServerSummaryTypeDef],
     },
     total=False,
 )
 
-AssessmentTargetUnionTypeDef = Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
+StartAssessmentRequestRequestTypeDef = TypedDict(
+    "StartAssessmentRequestRequestTypeDef",
+    {
+        "assessmentTargets": Sequence[AssessmentTargetTypeDef],
+        "s3bucketForAnalysisData": str,
+        "s3bucketForReportData": str,
+    },
+    total=False,
+)
+
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -725,38 +668,28 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
-    "DatabaseMigrationPreferenceOutputTypeDef",
-    {
-        "heterogeneous": HeterogeneousOutputTypeDef,
-        "homogeneous": HomogeneousOutputTypeDef,
-        "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 DatabaseMigrationPreferenceTypeDef = TypedDict(
     "DatabaseMigrationPreferenceTypeDef",
     {
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
-        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
+        "assessmentTargets": List[AssessmentTargetTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImportFileTaskResponseTypeDef = TypedDict(
@@ -942,24 +875,14 @@
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ManagementPreferenceOutputTypeDef = TypedDict(
-    "ManagementPreferenceOutputTypeDef",
-    {
-        "awsManagedResources": AwsManagedResourcesOutputTypeDef,
-        "noPreference": NoManagementPreferenceOutputTypeDef,
-        "selfManageResources": SelfManageResourcesOutputTypeDef,
-    },
-    total=False,
-)
-
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
         "noPreference": NoManagementPreferenceTypeDef,
         "selfManageResources": SelfManageResourcesTypeDef,
     },
@@ -1047,24 +970,14 @@
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentRequestRequestTypeDef = TypedDict(
-    "StartAssessmentRequestRequestTypeDef",
-    {
-        "assessmentTargets": Sequence[AssessmentTargetUnionTypeDef],
-        "s3bucketForAnalysisData": str,
-        "s3bucketForReportData": str,
-    },
-    total=False,
-)
-
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
         "collectorId": str,
         "collectorVersion": str,
         "configurationSummary": ConfigurationSummaryTypeDef,
@@ -1072,40 +985,23 @@
         "ipAddress": str,
         "lastActivityTimeStamp": str,
         "registeredTimeStamp": str,
     },
     total=False,
 )
 
-DatabasePreferencesOutputTypeDef = TypedDict(
-    "DatabasePreferencesOutputTypeDef",
-    {
-        "databaseManagementPreference": DatabaseManagementPreferenceType,
-        "databaseMigrationPreference": DatabaseMigrationPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 DatabasePreferencesTypeDef = TypedDict(
     "DatabasePreferencesTypeDef",
     {
         "databaseManagementPreference": DatabaseManagementPreferenceType,
         "databaseMigrationPreference": DatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
-ApplicationPreferencesOutputTypeDef = TypedDict(
-    "ApplicationPreferencesOutputTypeDef",
-    {
-        "managementPreference": ManagementPreferenceOutputTypeDef,
-    },
-    total=False,
-)
-
 ApplicationPreferencesTypeDef = TypedDict(
     "ApplicationPreferencesTypeDef",
     {
         "managementPreference": ManagementPreferenceTypeDef,
     },
     total=False,
 )
@@ -1187,31 +1083,25 @@
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabasePreferencesUnionTypeDef = Union[
-    DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
-]
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
-        "applicationPreferences": ApplicationPreferencesOutputTypeDef,
-        "databasePreferences": DatabasePreferencesOutputTypeDef,
+        "applicationPreferences": ApplicationPreferencesTypeDef,
+        "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApplicationPreferencesUnionTypeDef = Union[
-    ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
-]
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
```

### Comparing `types-aiobotocore-migrationhubstrategy-2.5.2.post1/types_aiobotocore_migrationhubstrategy.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhubstrategy-2.5.2.post2/types_aiobotocore_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

