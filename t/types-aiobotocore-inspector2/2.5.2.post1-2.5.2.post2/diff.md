# Comparing `tmp/types-aiobotocore-inspector2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-inspector2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-inspector2-2.5.2.post1.tar` & `types-aiobotocore-inspector2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38060 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13204 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75995 2023-08-02 14:40:19.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75914 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.276642 types-aiobotocore-inspector2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14455 2023-08-04 13:59:11.276642 types-aiobotocore-inspector2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12925 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.276642 types-aiobotocore-inspector2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.266642 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2627 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2626 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38607 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38542 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17830 2023-08-04 13:40:23.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17828 2023-08-04 13:40:23.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13194 2023-08-04 13:40:23.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13182 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    73813 2023-08-04 13:40:26.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    73732 2023-08-04 13:40:24.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:22.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.276642 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14455 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:11.000000 types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/LICENSE` & `types-aiobotocore-inspector2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/setup.py` & `types-aiobotocore-inspector2-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Inspector2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.pyi` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__main__.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Inspector2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
     CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
@@ -63,15 +64,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,15 +83,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaUnionTypeDef,
+    ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -169,14 +170,24 @@
         Retrieves code snippets from findings that Amazon Inspector detected code
         vulnerabilities in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#batch_get_code_snippet)
         """
 
+    async def batch_get_finding_details(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetFindingDetailsResponseTypeDef:
+        """
+        Gets vulnerability details for findings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_finding_details)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#batch_get_finding_details)
+        """
+
     async def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
@@ -237,15 +248,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#close)
         """
 
     async def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaUnionTypeDef,
+        filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -255,29 +266,29 @@
         """
 
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...
+        filterCriteria: FilterCriteriaTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
 
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -514,15 +525,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
 
     async def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -630,15 +641,15 @@
 
     async def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.pyi` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
+    BatchGetFindingDetailsResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
     CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
@@ -63,15 +64,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,15 +83,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaUnionTypeDef,
+    ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -161,14 +162,23 @@
         """
         Retrieves code snippets from findings that Amazon Inspector detected code
         vulnerabilities in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#batch_get_code_snippet)
         """
+    async def batch_get_finding_details(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetFindingDetailsResponseTypeDef:
+        """
+        Gets vulnerability details for findings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_finding_details)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#batch_get_finding_details)
+        """
     async def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
@@ -222,15 +232,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#close)
         """
     async def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaUnionTypeDef,
+        filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -239,28 +249,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_filter)
         """
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...
+        filterCriteria: FilterCriteriaTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -475,15 +485,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
     async def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -580,15 +590,15 @@
         """
     async def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
@@ -39,14 +38,15 @@
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
     "FilterActionType",
+    "FindingDetailsErrorCodeType",
     "FindingStatusType",
     "FindingTypeSortByType",
     "FindingTypeType",
     "FixAvailableType",
     "FreeTrialInfoErrorCodeType",
     "FreeTrialStatusType",
     "FreeTrialTypeType",
@@ -95,15 +95,14 @@
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 AggregationFindingTypeType = Literal[
     "CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"
 ]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
@@ -154,14 +153,17 @@
     "SSM_THROTTLED",
     "SSM_UNAVAILABLE",
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
+FindingDetailsErrorCodeType = Literal[
+    "ACCESS_DENIED", "FINDING_DETAILS_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
 FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
@@ -328,14 +330,15 @@
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
@@ -431,14 +434,15 @@
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
@@ -517,26 +521,28 @@
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

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.pyi` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/literals.py`

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
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
@@ -38,14 +39,15 @@
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
     "FilterActionType",
+    "FindingDetailsErrorCodeType",
     "FindingStatusType",
     "FindingTypeSortByType",
     "FindingTypeType",
     "FixAvailableType",
     "FreeTrialInfoErrorCodeType",
     "FreeTrialStatusType",
     "FreeTrialTypeType",
@@ -94,14 +96,15 @@
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 AggregationFindingTypeType = Literal[
     "CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"
 ]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
@@ -152,14 +155,17 @@
     "SSM_THROTTLED",
     "SSM_UNAVAILABLE",
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
+FindingDetailsErrorCodeType = Literal[
+    "ACCESS_DENIED", "FINDING_DETAILS_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
 FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
@@ -326,14 +332,15 @@
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
@@ -429,14 +436,15 @@
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
@@ -515,26 +523,28 @@
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

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -199,15 +199,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.pyi` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaUnionTypeDef,
+    FilterCriteriaTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -190,15 +190,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaUnionTypeDef = ...,
+        filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.py` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -98,14 +99,16 @@
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    "FindingDetailsErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
@@ -120,15 +123,14 @@
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
-    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "MapFilterTypeDef",
@@ -137,14 +139,15 @@
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
+    "EvidenceTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -226,14 +229,15 @@
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
@@ -241,53 +245,50 @@
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
-    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "GetSbomExportResponseTypeDef",
     "CreateSbomExportRequestRequestTypeDef",
-    "ResourceFilterCriteriaUnionTypeDef",
+    "GetSbomExportResponseTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "FilterTypeDef",
-    "GetFindingsReportStatusResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateFindingsReportRequestRequestTypeDef",
-    "FilterCriteriaUnionTypeDef",
+    "FilterTypeDef",
+    "GetFindingsReportStatusResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -488,14 +489,30 @@
     {
         "errorCode": CodeSnippetErrorCodeType,
         "errorMessage": str,
         "findingArn": str,
     },
 )
 
+BatchGetFindingDetailsRequestRequestTypeDef = TypedDict(
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+FindingDetailsErrorTypeDef = TypedDict(
+    "FindingDetailsErrorTypeDef",
+    {
+        "errorCode": FindingDetailsErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -721,23 +738,14 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
-DateFilterOutputTypeDef = TypedDict(
-    "DateFilterOutputTypeDef",
-    {
-        "endInclusive": datetime,
-        "startInclusive": datetime,
-    },
-    total=False,
-)
-
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
         "accountId": str,
         "status": DelegatedAdminStatusType,
     },
     total=False,
@@ -902,14 +910,24 @@
     "EpssTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+EvidenceTypeDef = TypedDict(
+    "EvidenceTypeDef",
+    {
+        "evidenceDetail": str,
+        "evidenceRule": str,
+        "severity": str,
+    },
+    total=False,
+)
+
 ExploitObservedTypeDef = TypedDict(
     "ExploitObservedTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
     },
     total=False,
@@ -1956,14 +1974,31 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+FindingDetailTypeDef = TypedDict(
+    "FindingDetailTypeDef",
+    {
+        "cisaData": CisaDataTypeDef,
+        "cwes": List[str],
+        "epssScore": float,
+        "evidences": List[EvidenceTypeDef],
+        "exploitObserved": ExploitObservedTypeDef,
+        "findingArn": str,
+        "referenceUrls": List[str],
+        "riskScore": int,
+        "tools": List[str],
+        "ttps": List[str],
+    },
+    total=False,
+)
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -2139,29 +2174,14 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-ResourceFilterCriteriaOutputTypeDef = TypedDict(
-    "ResourceFilterCriteriaOutputTypeDef",
-    {
-        "accountId": List[ResourceStringFilterTypeDef],
-        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
-        "ecrImageTags": List[ResourceStringFilterTypeDef],
-        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
-        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
-        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
-        "resourceId": List[ResourceStringFilterTypeDef],
-        "resourceType": List[ResourceStringFilterTypeDef],
-    },
-    total=False,
-)
-
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2340,70 +2360,30 @@
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchVulnerabilitiesResponseTypeDef = TypedDict(
-    "SearchVulnerabilitiesResponseTypeDef",
+BatchGetFindingDetailsResponseTypeDef = TypedDict(
+    "BatchGetFindingDetailsResponseTypeDef",
     {
-        "nextToken": str,
-        "vulnerabilities": List[VulnerabilityTypeDef],
+        "errors": List[FindingDetailsErrorTypeDef],
+        "findingDetails": List[FindingDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FilterCriteriaOutputTypeDef = TypedDict(
-    "FilterCriteriaOutputTypeDef",
+SearchVulnerabilitiesResponseTypeDef = TypedDict(
+    "SearchVulnerabilitiesResponseTypeDef",
     {
-        "awsAccountId": List[StringFilterTypeDef],
-        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
-        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
-        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
-        "componentId": List[StringFilterTypeDef],
-        "componentType": List[StringFilterTypeDef],
-        "ec2InstanceImageId": List[StringFilterTypeDef],
-        "ec2InstanceSubnetId": List[StringFilterTypeDef],
-        "ec2InstanceVpcId": List[StringFilterTypeDef],
-        "ecrImageArchitecture": List[StringFilterTypeDef],
-        "ecrImageHash": List[StringFilterTypeDef],
-        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
-        "ecrImageRegistry": List[StringFilterTypeDef],
-        "ecrImageRepositoryName": List[StringFilterTypeDef],
-        "ecrImageTags": List[StringFilterTypeDef],
-        "epssScore": List[NumberFilterTypeDef],
-        "exploitAvailable": List[StringFilterTypeDef],
-        "findingArn": List[StringFilterTypeDef],
-        "findingStatus": List[StringFilterTypeDef],
-        "findingType": List[StringFilterTypeDef],
-        "firstObservedAt": List[DateFilterOutputTypeDef],
-        "fixAvailable": List[StringFilterTypeDef],
-        "inspectorScore": List[NumberFilterTypeDef],
-        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
-        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
-        "lambdaFunctionLayers": List[StringFilterTypeDef],
-        "lambdaFunctionName": List[StringFilterTypeDef],
-        "lambdaFunctionRuntime": List[StringFilterTypeDef],
-        "lastObservedAt": List[DateFilterOutputTypeDef],
-        "networkProtocol": List[StringFilterTypeDef],
-        "portRange": List[PortRangeFilterTypeDef],
-        "relatedVulnerabilities": List[StringFilterTypeDef],
-        "resourceId": List[StringFilterTypeDef],
-        "resourceTags": List[MapFilterTypeDef],
-        "resourceType": List[StringFilterTypeDef],
-        "severity": List[StringFilterTypeDef],
-        "title": List[StringFilterTypeDef],
-        "updatedAt": List[DateFilterOutputTypeDef],
-        "vendorSeverity": List[StringFilterTypeDef],
-        "vulnerabilityId": List[StringFilterTypeDef],
-        "vulnerabilitySource": List[StringFilterTypeDef],
-        "vulnerablePackages": List[PackageFilterTypeDef],
+        "nextToken": str,
+        "vulnerabilities": List[VulnerabilityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
@@ -2489,28 +2469,14 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2525,17 +2491,28 @@
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
 
-ResourceFilterCriteriaUnionTypeDef = Union[
-    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
-]
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2667,54 +2644,14 @@
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaOutputTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaOutputTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2755,15 +2692,54 @@
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
 
-FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.pyi` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
     FilterActionType,
+    FindingDetailsErrorCodeType,
     FindingStatusType,
     FindingTypeSortByType,
     FindingTypeType,
     FixAvailableType,
     FreeTrialInfoErrorCodeType,
     FreeTrialStatusType,
     FreeTrialTypeType,
@@ -97,14 +98,16 @@
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
     "CodeSnippetErrorTypeDef",
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    "FindingDetailsErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
@@ -119,15 +122,14 @@
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
-    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "MapFilterTypeDef",
@@ -136,14 +138,15 @@
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
+    "EvidenceTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
@@ -225,14 +228,15 @@
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
@@ -240,53 +244,50 @@
     "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
-    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "GetSbomExportResponseTypeDef",
     "CreateSbomExportRequestRequestTypeDef",
-    "ResourceFilterCriteriaUnionTypeDef",
+    "GetSbomExportResponseTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "FilterTypeDef",
-    "GetFindingsReportStatusResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateFindingsReportRequestRequestTypeDef",
-    "FilterCriteriaUnionTypeDef",
+    "FilterTypeDef",
+    "GetFindingsReportStatusResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -481,14 +482,30 @@
     {
         "errorCode": CodeSnippetErrorCodeType,
         "errorMessage": str,
         "findingArn": str,
     },
 )
 
+BatchGetFindingDetailsRequestRequestTypeDef = TypedDict(
+    "BatchGetFindingDetailsRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+FindingDetailsErrorTypeDef = TypedDict(
+    "FindingDetailsErrorTypeDef",
+    {
+        "errorCode": FindingDetailsErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -706,23 +723,14 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
-DateFilterOutputTypeDef = TypedDict(
-    "DateFilterOutputTypeDef",
-    {
-        "endInclusive": datetime,
-        "startInclusive": datetime,
-    },
-    total=False,
-)
-
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
         "accountId": str,
         "status": DelegatedAdminStatusType,
     },
     total=False,
@@ -881,14 +889,24 @@
     "EpssTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
+EvidenceTypeDef = TypedDict(
+    "EvidenceTypeDef",
+    {
+        "evidenceDetail": str,
+        "evidenceRule": str,
+        "severity": str,
+    },
+    total=False,
+)
+
 ExploitObservedTypeDef = TypedDict(
     "ExploitObservedTypeDef",
     {
         "firstSeen": datetime,
         "lastSeen": datetime,
     },
     total=False,
@@ -1903,14 +1921,31 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+FindingDetailTypeDef = TypedDict(
+    "FindingDetailTypeDef",
+    {
+        "cisaData": CisaDataTypeDef,
+        "cwes": List[str],
+        "epssScore": float,
+        "evidences": List[EvidenceTypeDef],
+        "exploitObserved": ExploitObservedTypeDef,
+        "findingArn": str,
+        "referenceUrls": List[str],
+        "riskScore": int,
+        "tools": List[str],
+        "ttps": List[str],
+    },
+    total=False,
+)
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -2082,29 +2117,14 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-ResourceFilterCriteriaOutputTypeDef = TypedDict(
-    "ResourceFilterCriteriaOutputTypeDef",
-    {
-        "accountId": List[ResourceStringFilterTypeDef],
-        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
-        "ecrImageTags": List[ResourceStringFilterTypeDef],
-        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
-        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
-        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
-        "resourceId": List[ResourceStringFilterTypeDef],
-        "resourceType": List[ResourceStringFilterTypeDef],
-    },
-    total=False,
-)
-
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2279,70 +2299,30 @@
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchVulnerabilitiesResponseTypeDef = TypedDict(
-    "SearchVulnerabilitiesResponseTypeDef",
+BatchGetFindingDetailsResponseTypeDef = TypedDict(
+    "BatchGetFindingDetailsResponseTypeDef",
     {
-        "nextToken": str,
-        "vulnerabilities": List[VulnerabilityTypeDef],
+        "errors": List[FindingDetailsErrorTypeDef],
+        "findingDetails": List[FindingDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FilterCriteriaOutputTypeDef = TypedDict(
-    "FilterCriteriaOutputTypeDef",
+SearchVulnerabilitiesResponseTypeDef = TypedDict(
+    "SearchVulnerabilitiesResponseTypeDef",
     {
-        "awsAccountId": List[StringFilterTypeDef],
-        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
-        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
-        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
-        "componentId": List[StringFilterTypeDef],
-        "componentType": List[StringFilterTypeDef],
-        "ec2InstanceImageId": List[StringFilterTypeDef],
-        "ec2InstanceSubnetId": List[StringFilterTypeDef],
-        "ec2InstanceVpcId": List[StringFilterTypeDef],
-        "ecrImageArchitecture": List[StringFilterTypeDef],
-        "ecrImageHash": List[StringFilterTypeDef],
-        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
-        "ecrImageRegistry": List[StringFilterTypeDef],
-        "ecrImageRepositoryName": List[StringFilterTypeDef],
-        "ecrImageTags": List[StringFilterTypeDef],
-        "epssScore": List[NumberFilterTypeDef],
-        "exploitAvailable": List[StringFilterTypeDef],
-        "findingArn": List[StringFilterTypeDef],
-        "findingStatus": List[StringFilterTypeDef],
-        "findingType": List[StringFilterTypeDef],
-        "firstObservedAt": List[DateFilterOutputTypeDef],
-        "fixAvailable": List[StringFilterTypeDef],
-        "inspectorScore": List[NumberFilterTypeDef],
-        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
-        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
-        "lambdaFunctionLayers": List[StringFilterTypeDef],
-        "lambdaFunctionName": List[StringFilterTypeDef],
-        "lambdaFunctionRuntime": List[StringFilterTypeDef],
-        "lastObservedAt": List[DateFilterOutputTypeDef],
-        "networkProtocol": List[StringFilterTypeDef],
-        "portRange": List[PortRangeFilterTypeDef],
-        "relatedVulnerabilities": List[StringFilterTypeDef],
-        "resourceId": List[StringFilterTypeDef],
-        "resourceTags": List[MapFilterTypeDef],
-        "resourceType": List[StringFilterTypeDef],
-        "severity": List[StringFilterTypeDef],
-        "title": List[StringFilterTypeDef],
-        "updatedAt": List[DateFilterOutputTypeDef],
-        "vendorSeverity": List[StringFilterTypeDef],
-        "vulnerabilityId": List[StringFilterTypeDef],
-        "vulnerabilitySource": List[StringFilterTypeDef],
-        "vulnerablePackages": List[PackageFilterTypeDef],
+        "nextToken": str,
+        "vulnerabilities": List[VulnerabilityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
@@ -2426,28 +2406,14 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2460,17 +2426,28 @@
 )
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
-ResourceFilterCriteriaUnionTypeDef = Union[
-    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
-]
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2596,52 +2573,14 @@
 
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaOutputTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaOutputTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2678,15 +2617,52 @@
 
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
-FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
```

### Comparing `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/SOURCES.txt` & `types-aiobotocore-inspector2-2.5.2.post2/types_aiobotocore_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

