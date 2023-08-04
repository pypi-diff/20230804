# Comparing `tmp/types-aiobotocore-guardduty-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-guardduty-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-guardduty-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-guardduty-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-guardduty-2.5.2.post1.tar` & `types-aiobotocore-guardduty-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.913575 types-aiobotocore-guardduty-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24838 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.913575 types-aiobotocore-guardduty-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52674 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94451 2023-08-02 14:39:53.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94364 2023-08-02 14:39:51.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.836378 types-aiobotocore-guardduty-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-08-04 12:00:58.836378 types-aiobotocore-guardduty-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.836378 types-aiobotocore-guardduty-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.828378 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52639 2023-08-04 11:47:22.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-08-04 11:47:22.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-04 11:47:22.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-08-04 11:47:22.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-08-04 11:47:22.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93001 2023-08-04 11:47:24.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92914 2023-08-04 11:47:23.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:47:20.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.836378 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:00:58.000000 types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/LICENSE` & `types-aiobotocore-guardduty-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/setup.py` & `types-aiobotocore-guardduty-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-guardduty",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.py` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.pyi` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.py` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -91,15 +91,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaUnionTypeDef,
+    ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -212,15 +212,15 @@
         """
 
     async def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef,
+        FindingCriteria: FindingCriteriaTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -531,15 +531,15 @@
         """
 
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -692,15 +692,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_filters)
         """
 
     async def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
+        FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -860,15 +860,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
@@ -904,15 +904,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
 
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
+        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.pyi` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -91,15 +91,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaUnionTypeDef,
+    ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -201,15 +201,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_detector)
         """
     async def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef,
+        FindingCriteria: FindingCriteriaTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -492,15 +492,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings)
         """
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -639,15 +639,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_filters)
         """
     async def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
+        FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -792,15 +792,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...
+        FindingCriteria: FindingCriteriaTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
@@ -833,15 +833,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
+        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.py` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.pyi` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.py` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -162,15 +162,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
+        FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.pyi` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaUnionTypeDef,
+    FindingCriteriaTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -155,15 +155,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
+        FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.py` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
     data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -73,15 +73,14 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
@@ -194,15 +193,14 @@
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
     "BucketLevelPermissionsTypeDef",
-    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
     "CreateFilterResponseTypeDef",
     "CreateIPSetResponseTypeDef",
     "CreatePublishingDestinationResponseTypeDef",
     "CreateThreatIntelSetResponseTypeDef",
@@ -269,27 +267,25 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
-    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "GetFilterResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
-    "FindingCriteriaUnionTypeDef",
+    "GetFilterResponseTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -303,15 +299,14 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
-    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -328,15 +323,14 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
-    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -503,33 +497,14 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Eq": List[str],
-        "Neq": List[str],
-        "Gt": int,
-        "Gte": int,
-        "Lt": int,
-        "Lte": int,
-        "Equals": List[str],
-        "NotEquals": List[str],
-        "GreaterThan": int,
-        "GreaterThanOrEqual": int,
-        "LessThan": int,
-        "LessThanOrEqual": int,
-    },
-    total=False,
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -1805,22 +1780,14 @@
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-FindingCriteriaOutputTypeDef = TypedDict(
-    "FindingCriteriaOutputTypeDef",
-    {
-        "Criterion": Dict[str, ConditionOutputTypeDef],
-    },
-    total=False,
-)
-
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2604,25 +2571,18 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
-ScanConditionOutputTypeDef = TypedDict(
-    "ScanConditionOutputTypeDef",
-    {
-        "MapEquals": List[ScanConditionPairTypeDef],
-    },
-)
-
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": Sequence[ScanConditionPairTypeDef],
+        "MapEquals": List[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2705,27 +2665,14 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2745,15 +2692,27 @@
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
 
-FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -3063,28 +3022,19 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
-ScanResourceCriteriaOutputTypeDef = TypedDict(
-    "ScanResourceCriteriaOutputTypeDef",
-    {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
-    },
-    total=False,
-)
-
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -3450,23 +3400,20 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScanResourceCriteriaUnionTypeDef = Union[
-    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
-]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.pyi` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
     data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -72,15 +72,14 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
-    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
@@ -193,15 +192,14 @@
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
     "BucketLevelPermissionsTypeDef",
-    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
     "CreateFilterResponseTypeDef",
     "CreateIPSetResponseTypeDef",
     "CreatePublishingDestinationResponseTypeDef",
     "CreateThreatIntelSetResponseTypeDef",
@@ -268,27 +266,25 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
-    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "GetFilterResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
-    "FindingCriteriaUnionTypeDef",
+    "GetFilterResponseTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -302,15 +298,14 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
-    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -327,15 +322,14 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
-    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -502,33 +496,14 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
-ConditionOutputTypeDef = TypedDict(
-    "ConditionOutputTypeDef",
-    {
-        "Eq": List[str],
-        "Neq": List[str],
-        "Gt": int,
-        "Gte": int,
-        "Lt": int,
-        "Lte": int,
-        "Equals": List[str],
-        "NotEquals": List[str],
-        "GreaterThan": int,
-        "GreaterThanOrEqual": int,
-        "LessThan": int,
-        "LessThanOrEqual": int,
-    },
-    total=False,
-)
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -1772,22 +1747,14 @@
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-FindingCriteriaOutputTypeDef = TypedDict(
-    "FindingCriteriaOutputTypeDef",
-    {
-        "Criterion": Dict[str, ConditionOutputTypeDef],
-    },
-    total=False,
-)
-
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2555,25 +2522,18 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
-ScanConditionOutputTypeDef = TypedDict(
-    "ScanConditionOutputTypeDef",
-    {
-        "MapEquals": List[ScanConditionPairTypeDef],
-    },
-)
-
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": Sequence[ScanConditionPairTypeDef],
+        "MapEquals": List[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2656,27 +2616,14 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2694,15 +2641,27 @@
 )
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
-FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -3004,28 +2963,19 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
-ScanResourceCriteriaOutputTypeDef = TypedDict(
-    "ScanResourceCriteriaOutputTypeDef",
-    {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
-    },
-    total=False,
-)
-
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -3371,23 +3321,20 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScanResourceCriteriaUnionTypeDef = Union[
-    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
-]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/SOURCES.txt` & `types-aiobotocore-guardduty-2.5.2.post2/types_aiobotocore_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

