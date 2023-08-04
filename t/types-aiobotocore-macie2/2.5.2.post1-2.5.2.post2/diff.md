# Comparing `tmp/types-aiobotocore-macie2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-macie2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-macie2-2.5.2.post1.tar` & `types-aiobotocore-macie2-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:42:42.000000 types-aiobotocore-macie2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.293532 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63190 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    63085 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94186 2023-08-02 14:42:47.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94131 2023-08-02 14:42:46.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16082 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14568 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:43:41.000000 types-aiobotocore-macie2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.286643 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4413 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4412 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63125 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63020 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17444 2023-08-04 13:43:44.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17442 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20353 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20335 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    88777 2023-08-04 13:43:47.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    88722 2023-08-04 13:43:45.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1516 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1515 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16082 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/LICENSE` & `types-aiobotocore-macie2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post1/setup.py` & `types-aiobotocore-macie2-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__main__.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Macie2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -88,15 +88,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyUnionTypeDef,
+    JobScheduleFrequencyTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,21 +108,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionUnionTypeDef,
+    S3JobDefinitionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesUnionTypeDef,
-    SensitivityInspectionTemplateIncludesUnionTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -232,23 +232,23 @@
 
     async def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: S3JobDefinitionUnionTypeDef,
+        s3JobDefinition: S3JobDefinitionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
+        scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
@@ -275,15 +275,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
         """
 
     async def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: FindingCriteriaUnionTypeDef,
+        findingCriteria: FindingCriteriaTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -565,15 +565,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_custom_data_identifier)
         """
 
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -760,15 +760,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_custom_data_identifiers)
         """
 
     async def list_findings(
         self,
         *,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -990,15 +990,15 @@
     async def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -1072,16 +1072,16 @@
         """
 
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
+        excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -88,15 +88,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyUnionTypeDef,
+    JobScheduleFrequencyTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,21 +108,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionUnionTypeDef,
+    S3JobDefinitionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesUnionTypeDef,
-    SensitivityInspectionTemplateIncludesUnionTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -222,23 +222,23 @@
         """
     async def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: S3JobDefinitionUnionTypeDef,
+        s3JobDefinition: S3JobDefinitionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
+        scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
@@ -263,15 +263,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
         """
     async def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: FindingCriteriaUnionTypeDef,
+        findingCriteria: FindingCriteriaTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -525,15 +525,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_custom_data_identifier)
         """
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -701,15 +701,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_custom_data_identifiers)
         """
     async def list_findings(
         self,
         *,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -911,15 +911,15 @@
     async def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -986,16 +986,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_reveal_configuration)
         """
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
+        excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 ListManagedDataIdentifiersPaginatorName = Literal["list_managed_data_identifiers"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
 ListResourceProfileArtifactsPaginatorName = Literal["list_resource_profile_artifacts"]
 ListResourceProfileDetectionsPaginatorName = Literal["list_resource_profile_detections"]
 ListSensitivityInspectionTemplatesPaginatorName = Literal["list_sensitivity_inspection_templates"]
 MacieStatusType = Literal["ENABLED", "PAUSED"]
-ManagedDataIdentifierSelectorType = Literal["ALL", "EXCLUDE", "INCLUDE", "NONE"]
+ManagedDataIdentifierSelectorType = Literal["ALL", "EXCLUDE", "INCLUDE", "NONE", "RECOMMENDED"]
 OrderByType = Literal["ASC", "DESC"]
 OriginTypeType = Literal["AUTOMATED_SENSITIVE_DATA_DISCOVERY", "SENSITIVE_DATA_DISCOVERY_JOB"]
 RelationshipStatusType = Literal[
     "AccountSuspended",
     "Created",
     "EmailVerificationFailed",
     "EmailVerificationInProgress",
@@ -256,14 +256,15 @@
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
@@ -359,14 +360,15 @@
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
@@ -445,26 +447,28 @@
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

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 ListManagedDataIdentifiersPaginatorName = Literal["list_managed_data_identifiers"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
 ListResourceProfileArtifactsPaginatorName = Literal["list_resource_profile_artifacts"]
 ListResourceProfileDetectionsPaginatorName = Literal["list_resource_profile_detections"]
 ListSensitivityInspectionTemplatesPaginatorName = Literal["list_sensitivity_inspection_templates"]
 MacieStatusType = Literal["ENABLED", "PAUSED"]
-ManagedDataIdentifierSelectorType = Literal["ALL", "EXCLUDE", "INCLUDE", "NONE"]
+ManagedDataIdentifierSelectorType = Literal["ALL", "EXCLUDE", "INCLUDE", "NONE", "RECOMMENDED"]
 OrderByType = Literal["ASC", "DESC"]
 OriginTypeType = Literal["AUTOMATED_SENSITIVE_DATA_DISCOVERY", "SENSITIVE_DATA_DISCOVERY_JOB"]
 RelationshipStatusType = Literal[
     "AccountSuspended",
     "Created",
     "EmailVerificationFailed",
     "EmailVerificationInProgress",
@@ -254,14 +254,15 @@
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
@@ -357,14 +358,15 @@
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
@@ -443,26 +445,28 @@
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

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -224,15 +224,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -215,15 +215,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: FindingCriteriaUnionTypeDef = ...,
+        findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
     data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -111,17 +111,15 @@
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
     "SeverityLevelTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
-    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
-    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
@@ -154,30 +152,29 @@
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
     "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesOutputTypeDef",
-    "SensitivityInspectionTemplateIncludesOutputTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
-    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobOutputTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
@@ -190,24 +187,21 @@
     "ResourceProfileArtifactTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagValuePairTypeDef",
@@ -250,15 +244,14 @@
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
     "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
-    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
     "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
@@ -281,105 +274,90 @@
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
     "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
-    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
-    "SensitivityInspectionTemplateExcludesUnionTypeDef",
-    "SensitivityInspectionTemplateIncludesUnionTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
-    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
-    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
     "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
-    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
-    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
-    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
-    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
-    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
-    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
-    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
-    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
-    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "DescribeClassificationJobResponseTypeDef",
     "CreateClassificationJobRequestRequestTypeDef",
-    "S3JobDefinitionUnionTypeDef",
+    "DescribeClassificationJobResponseTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -779,48 +757,24 @@
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
 
-SimpleCriterionForJobOutputTypeDef = TypedDict(
-    "SimpleCriterionForJobOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": SimpleCriterionKeyForJobType,
-        "values": List[str],
-    },
-    total=False,
-)
-
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
-    "CriterionAdditionalPropertiesOutputTypeDef",
-    {
-        "eq": List[str],
-        "eqExactMatch": List[str],
-        "gt": int,
-        "gte": int,
-        "lt": int,
-        "lte": int,
-        "neq": List[str],
-    },
-    total=False,
-)
-
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -1197,24 +1151,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesOutputTypeDef",
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1316,39 +1270,29 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-SimpleScopeTermOutputTypeDef = TypedDict(
-    "SimpleScopeTermOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": ScopeFilterKeyType,
-        "values": List[str],
-    },
-    total=False,
-)
-
 SimpleScopeTermTypeDef = TypedDict(
     "SimpleScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobOutputTypeDef = TypedDict(
-    "S3BucketDefinitionForJobOutputTypeDef",
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
     {
         "accountId": str,
-        "buckets": List[str],
+        "buckets": Sequence[str],
     },
 )
 
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1571,22 +1515,14 @@
     {
         "jsonPath": str,
         "recordIndex": int,
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
-    {
-        "accountId": str,
-        "buckets": Sequence[str],
-    },
-)
-
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
         "id": str,
     },
     total=False,
@@ -1640,32 +1576,14 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    {
-        "managedDataIdentifierIds": Sequence[str],
-    },
-    total=False,
-)
-
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
-    {
-        "allowListIds": Sequence[str],
-        "customDataIdentifierIds": Sequence[str],
-        "managedDataIdentifierIds": Sequence[str],
-    },
-    total=False,
-)
-
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -2198,22 +2116,14 @@
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FindingCriteriaOutputTypeDef = TypedDict(
-    "FindingCriteriaOutputTypeDef",
-    {
-        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
-    },
-    total=False,
-)
-
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
     total=False,
 )
@@ -2514,22 +2424,46 @@
     pass
 
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
+
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2566,24 +2500,14 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
-JobScheduleFrequencyOutputTypeDef = TypedDict(
-    "JobScheduleFrequencyOutputTypeDef",
-    {
-        "dailySchedule": Dict[str, Any],
-        "monthlySchedule": MonthlyScheduleTypeDef,
-        "weeklySchedule": WeeklyScheduleTypeDef,
-    },
-    total=False,
-)
-
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2683,44 +2607,14 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
-    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
-]
-SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
-    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
-]
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
-
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2755,43 +2649,23 @@
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
 
-TagCriterionForJobOutputTypeDef = TypedDict(
-    "TagCriterionForJobOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "tagValues": List[TagCriterionPairForJobTypeDef],
-    },
-    total=False,
-)
-
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
-TagScopeTermOutputTypeDef = TypedDict(
-    "TagScopeTermOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": str,
-        "tagValues": List[TagValuePairTypeDef],
-        "target": Literal["S3_OBJECT"],
-    },
-    total=False,
-)
-
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
@@ -2921,29 +2795,14 @@
     "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaOutputTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
         "findingCriteria": FindingCriteriaTypeDef,
         "name": str,
     },
@@ -2963,15 +2822,14 @@
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
-FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -2988,14 +2846,29 @@
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
 
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
+    {
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3036,17 +2909,14 @@
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
-JobScheduleFrequencyUnionTypeDef = Union[
-    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
-]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3148,41 +3018,23 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
-CriteriaForJobOutputTypeDef = TypedDict(
-    "CriteriaForJobOutputTypeDef",
-    {
-        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
-        "tagCriterion": TagCriterionForJobOutputTypeDef,
-    },
-    total=False,
-)
-
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
-JobScopeTermOutputTypeDef = TypedDict(
-    "JobScopeTermOutputTypeDef",
-    {
-        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
-        "tagScopeTerm": TagScopeTermOutputTypeDef,
-    },
-    total=False,
-)
-
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -3255,38 +3107,22 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
-CriteriaBlockForJobOutputTypeDef = TypedDict(
-    "CriteriaBlockForJobOutputTypeDef",
-    {
-        "and": List[CriteriaForJobOutputTypeDef],
-    },
-    total=False,
-)
-
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
-JobScopingBlockOutputTypeDef = TypedDict(
-    "JobScopingBlockOutputTypeDef",
-    {
-        "and": List[JobScopeTermOutputTypeDef],
-    },
-    total=False,
-)
-
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3373,41 +3209,23 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
-S3BucketCriteriaForJobOutputTypeDef = TypedDict(
-    "S3BucketCriteriaForJobOutputTypeDef",
-    {
-        "excludes": CriteriaBlockForJobOutputTypeDef,
-        "includes": CriteriaBlockForJobOutputTypeDef,
-    },
-    total=False,
-)
-
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
-ScopingOutputTypeDef = TypedDict(
-    "ScopingOutputTypeDef",
-    {
-        "excludes": JobScopingBlockOutputTypeDef,
-        "includes": JobScopingBlockOutputTypeDef,
-    },
-    total=False,
-)
-
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
@@ -3473,37 +3291,27 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
-S3JobDefinitionOutputTypeDef = TypedDict(
-    "S3JobDefinitionOutputTypeDef",
-    {
-        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
-        "scoping": ScopingOutputTypeDef,
-    },
-    total=False,
-)
-
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3527,42 +3335,14 @@
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
         "jobType": JobTypeType,
         "name": str,
         "s3JobDefinition": S3JobDefinitionTypeDef,
@@ -3588,15 +3368,42 @@
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
 
-S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
     data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -110,17 +110,15 @@
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
     "SeverityLevelTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
-    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
-    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
@@ -153,30 +151,29 @@
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
     "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesOutputTypeDef",
-    "SensitivityInspectionTemplateIncludesOutputTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
-    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobOutputTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
@@ -189,24 +186,21 @@
     "ResourceProfileArtifactTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagValuePairTypeDef",
@@ -249,15 +243,14 @@
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
     "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
-    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
     "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
@@ -280,105 +273,90 @@
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
     "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
-    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
-    "SensitivityInspectionTemplateExcludesUnionTypeDef",
-    "SensitivityInspectionTemplateIncludesUnionTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
-    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
-    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
     "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
-    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
-    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
-    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
-    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
-    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
-    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
-    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
-    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
-    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "DescribeClassificationJobResponseTypeDef",
     "CreateClassificationJobRequestRequestTypeDef",
-    "S3JobDefinitionUnionTypeDef",
+    "DescribeClassificationJobResponseTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -770,48 +748,24 @@
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
 
-SimpleCriterionForJobOutputTypeDef = TypedDict(
-    "SimpleCriterionForJobOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": SimpleCriterionKeyForJobType,
-        "values": List[str],
-    },
-    total=False,
-)
-
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
-    "CriterionAdditionalPropertiesOutputTypeDef",
-    {
-        "eq": List[str],
-        "eqExactMatch": List[str],
-        "gt": int,
-        "gte": int,
-        "lt": int,
-        "lte": int,
-        "neq": List[str],
-    },
-    total=False,
-)
-
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -1182,24 +1136,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesOutputTypeDef",
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1301,39 +1255,29 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-SimpleScopeTermOutputTypeDef = TypedDict(
-    "SimpleScopeTermOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": ScopeFilterKeyType,
-        "values": List[str],
-    },
-    total=False,
-)
-
 SimpleScopeTermTypeDef = TypedDict(
     "SimpleScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobOutputTypeDef = TypedDict(
-    "S3BucketDefinitionForJobOutputTypeDef",
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
     {
         "accountId": str,
-        "buckets": List[str],
+        "buckets": Sequence[str],
     },
 )
 
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
@@ -1550,22 +1494,14 @@
     {
         "jsonPath": str,
         "recordIndex": int,
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
-    {
-        "accountId": str,
-        "buckets": Sequence[str],
-    },
-)
-
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
         "id": str,
     },
     total=False,
@@ -1619,32 +1555,14 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    {
-        "managedDataIdentifierIds": Sequence[str],
-    },
-    total=False,
-)
-
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
-    {
-        "allowListIds": Sequence[str],
-        "customDataIdentifierIds": Sequence[str],
-        "managedDataIdentifierIds": Sequence[str],
-    },
-    total=False,
-)
-
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -2169,22 +2087,14 @@
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FindingCriteriaOutputTypeDef = TypedDict(
-    "FindingCriteriaOutputTypeDef",
-    {
-        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
-    },
-    total=False,
-)
-
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
     total=False,
 )
@@ -2477,22 +2387,44 @@
 ):
     pass
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2529,24 +2461,14 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
-JobScheduleFrequencyOutputTypeDef = TypedDict(
-    "JobScheduleFrequencyOutputTypeDef",
-    {
-        "dailySchedule": Dict[str, Any],
-        "monthlySchedule": MonthlyScheduleTypeDef,
-        "weeklySchedule": WeeklyScheduleTypeDef,
-    },
-    total=False,
-)
-
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2646,42 +2568,14 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
-    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
-]
-SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
-    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
-]
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2714,43 +2608,23 @@
 
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
-TagCriterionForJobOutputTypeDef = TypedDict(
-    "TagCriterionForJobOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "tagValues": List[TagCriterionPairForJobTypeDef],
-    },
-    total=False,
-)
-
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
-TagScopeTermOutputTypeDef = TypedDict(
-    "TagScopeTermOutputTypeDef",
-    {
-        "comparator": JobComparatorType,
-        "key": str,
-        "tagValues": List[TagValuePairTypeDef],
-        "target": Literal["S3_OBJECT"],
-    },
-    total=False,
-)
-
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
@@ -2876,29 +2750,14 @@
     "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaOutputTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
         "findingCriteria": FindingCriteriaTypeDef,
         "name": str,
     },
@@ -2916,15 +2775,14 @@
 
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
-FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -2939,14 +2797,29 @@
 
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
+    {
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -2985,17 +2858,14 @@
 
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
-JobScheduleFrequencyUnionTypeDef = Union[
-    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
-]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3095,41 +2965,23 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
-CriteriaForJobOutputTypeDef = TypedDict(
-    "CriteriaForJobOutputTypeDef",
-    {
-        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
-        "tagCriterion": TagCriterionForJobOutputTypeDef,
-    },
-    total=False,
-)
-
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
-JobScopeTermOutputTypeDef = TypedDict(
-    "JobScopeTermOutputTypeDef",
-    {
-        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
-        "tagScopeTerm": TagScopeTermOutputTypeDef,
-    },
-    total=False,
-)
-
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -3202,38 +3054,22 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
-CriteriaBlockForJobOutputTypeDef = TypedDict(
-    "CriteriaBlockForJobOutputTypeDef",
-    {
-        "and": List[CriteriaForJobOutputTypeDef],
-    },
-    total=False,
-)
-
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
-JobScopingBlockOutputTypeDef = TypedDict(
-    "JobScopingBlockOutputTypeDef",
-    {
-        "and": List[JobScopeTermOutputTypeDef],
-    },
-    total=False,
-)
-
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3320,41 +3156,23 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
-S3BucketCriteriaForJobOutputTypeDef = TypedDict(
-    "S3BucketCriteriaForJobOutputTypeDef",
-    {
-        "excludes": CriteriaBlockForJobOutputTypeDef,
-        "includes": CriteriaBlockForJobOutputTypeDef,
-    },
-    total=False,
-)
-
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
-ScopingOutputTypeDef = TypedDict(
-    "ScopingOutputTypeDef",
-    {
-        "excludes": JobScopingBlockOutputTypeDef,
-        "includes": JobScopingBlockOutputTypeDef,
-    },
-    total=False,
-)
-
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
@@ -3420,37 +3238,27 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
-S3JobDefinitionOutputTypeDef = TypedDict(
-    "S3JobDefinitionOutputTypeDef",
-    {
-        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
-        "scoping": ScopingOutputTypeDef,
-    },
-    total=False,
-)
-
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3474,42 +3282,14 @@
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
         "jobType": JobTypeType,
         "name": str,
         "s3JobDefinition": S3JobDefinitionTypeDef,
@@ -3533,15 +3313,42 @@
 
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
-S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
```

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.py` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.pyi` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/SOURCES.txt` & `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

