# Comparing `tmp/types-aiobotocore-backup-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-backup-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-backup-2.5.2.post1.tar` & `types-aiobotocore-backup-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21415 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57881 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57787 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72090 2023-08-02 14:33:44.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72007 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.367227 types-aiobotocore-backup-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:52.000000 types-aiobotocore-backup-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-08-04 12:00:28.367227 types-aiobotocore-backup-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-04 11:40:52.000000 types-aiobotocore-backup-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.367227 types-aiobotocore-backup-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 11:40:52.000000 types-aiobotocore-backup-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.363227 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57816 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57722 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-08-04 11:40:54.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-08-04 11:40:54.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-04 11:40:54.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-08-04 11:40:56.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67599 2023-08-04 11:40:55.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:53.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.367227 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:28.000000 types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-2.5.2.post1/LICENSE` & `types-aiobotocore-backup-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/setup.py` & `types-aiobotocore-backup-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.pyi` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__main__.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Backup 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Backup 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionUnionTypeDef,
+    BackupSelectionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -60,15 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlUnionTypeDef,
+    FrameworkControlTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -88,17 +88,17 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionUnionTypeDef,
-    ReportDeliveryChannelUnionTypeDef,
-    ReportSettingUnionTypeDef,
+    RecoveryPointSelectionTypeDef,
+    ReportDeliveryChannelTypeDef,
+    ReportSettingTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
     TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
@@ -194,15 +194,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
 
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionUnionTypeDef,
+        BackupSelection: BackupSelectionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -224,15 +224,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
 
     async def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
+        FrameworkControls: Sequence[FrameworkControlTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -242,30 +242,30 @@
 
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
+        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
 
     async def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
-        ReportSetting: ReportSettingUnionTypeDef,
+        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
+        ReportSetting: ReportSettingTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -973,15 +973,15 @@
         """
 
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
+        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -1023,16 +1023,16 @@
         """
 
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
-        ReportSetting: ReportSettingUnionTypeDef = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
+        ReportSetting: ReportSettingTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.pyi` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionUnionTypeDef,
+    BackupSelectionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -60,15 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlUnionTypeDef,
+    FrameworkControlTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -88,17 +88,17 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionUnionTypeDef,
-    ReportDeliveryChannelUnionTypeDef,
-    ReportSettingUnionTypeDef,
+    RecoveryPointSelectionTypeDef,
+    ReportDeliveryChannelTypeDef,
+    ReportSettingTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
     TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
@@ -185,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionUnionTypeDef,
+        BackupSelection: BackupSelectionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -213,15 +213,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
     async def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
+        FrameworkControls: Sequence[FrameworkControlTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -230,29 +230,29 @@
         """
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
+        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
     async def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
-        ReportSetting: ReportSettingUnionTypeDef,
+        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
+        ReportSetting: ReportSettingTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -898,15 +898,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_backup_plan)
         """
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
+        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -944,16 +944,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_region_settings)
         """
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
-        ReportSetting: ReportSettingUnionTypeDef = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
+        ReportSetting: ReportSettingTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.pyi` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.pyi` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.py` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingOutputTypeDef
+    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingTypeDef
 
-    data: AdvancedBackupSettingOutputTypeDef = ...
+    data: AdvancedBackupSettingTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -32,33 +32,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
-    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "DateRangeOutputTypeDef",
     "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
@@ -103,17 +100,15 @@
     "RecoveryPointByResourceTypeDef",
     "ListReportPlansInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
-    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
-    "ReportSettingOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
     "StartRestoreJobInputRequestTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
@@ -121,17 +116,15 @@
     "BackupJobTypeDef",
     "CopyJobTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
-    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
     "CreateBackupPlanOutputTypeDef",
     "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultOutputTypeDef",
     "CreateFrameworkOutputTypeDef",
     "CreateReportPlanOutputTypeDef",
     "DeleteBackupPlanOutputTypeDef",
@@ -157,16 +150,16 @@
     "StartReportJobOutputTypeDef",
     "StartRestoreJobOutputTypeDef",
     "UpdateBackupPlanOutputTypeDef",
     "UpdateFrameworkOutputTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
+    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
-    "RecoveryPointSelectionOutputTypeDef",
     "DateRangeTypeDef",
     "ListBackupJobsInputRequestTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
@@ -184,62 +177,46 @@
     "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
-    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
-    "ReportPlanTypeDef",
-    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
-    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "FrameworkControlUnionTypeDef",
-    "CreateLegalHoldOutputTypeDef",
-    "GetLegalHoldOutputTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "GetBackupSelectionOutputTypeDef",
-    "BackupSelectionUnionTypeDef",
     "CreateBackupSelectionInputRequestTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
+    "GetBackupSelectionOutputTypeDef",
     "CreateLegalHoldInputRequestTypeDef",
-    "RecoveryPointSelectionUnionTypeDef",
+    "CreateLegalHoldOutputTypeDef",
+    "GetLegalHoldOutputTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
-AdvancedBackupSettingOutputTypeDef = TypedDict(
-    "AdvancedBackupSettingOutputTypeDef",
-    {
-        "ResourceType": str,
-        "BackupOptions": Dict[str, str],
-    },
-    total=False,
-)
-
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -358,24 +335,14 @@
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
-ControlScopeOutputTypeDef = TypedDict(
-    "ControlScopeOutputTypeDef",
-    {
-        "ComplianceResourceIds": List[str],
-        "ComplianceResourceTypes": List[str],
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
@@ -457,22 +424,14 @@
 )
 
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
 
-DateRangeOutputTypeDef = TypedDict(
-    "DateRangeOutputTypeDef",
-    {
-        "FromDate": datetime,
-        "ToDate": datetime,
-    },
-)
-
 TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
@@ -1019,70 +978,23 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
-_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
-    "_RequiredReportDeliveryChannelOutputTypeDef",
-    {
-        "S3BucketName": str,
-    },
-)
-_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
-    "_OptionalReportDeliveryChannelOutputTypeDef",
-    {
-        "S3KeyPrefix": str,
-        "Formats": List[str],
-    },
-    total=False,
-)
-
-
-class ReportDeliveryChannelOutputTypeDef(
-    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
-):
-    pass
-
-
 ReportDestinationTypeDef = TypedDict(
     "ReportDestinationTypeDef",
     {
         "S3BucketName": str,
         "S3Keys": List[str],
     },
     total=False,
 )
 
-_RequiredReportSettingOutputTypeDef = TypedDict(
-    "_RequiredReportSettingOutputTypeDef",
-    {
-        "ReportTemplate": str,
-    },
-)
-_OptionalReportSettingOutputTypeDef = TypedDict(
-    "_OptionalReportSettingOutputTypeDef",
-    {
-        "FrameworkArns": List[str],
-        "NumberOfFrameworks": int,
-        "Accounts": List[str],
-        "OrganizationUnits": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
-
-class ReportSettingOutputTypeDef(
-    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
-):
-    pass
-
-
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1172,15 +1084,15 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
@@ -1359,58 +1271,25 @@
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
     },
     total=False,
 )
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
-    {
-        "StringEquals": List[ConditionParameterTypeDef],
-        "StringNotEquals": List[ConditionParameterTypeDef],
-        "StringLike": List[ConditionParameterTypeDef],
-        "StringNotLike": List[ConditionParameterTypeDef],
-    },
-    total=False,
-)
-
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "StringEquals": Sequence[ConditionParameterTypeDef],
         "StringNotEquals": Sequence[ConditionParameterTypeDef],
         "StringLike": Sequence[ConditionParameterTypeDef],
         "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredFrameworkControlOutputTypeDef = TypedDict(
-    "_RequiredFrameworkControlOutputTypeDef",
-    {
-        "ControlName": str,
-    },
-)
-_OptionalFrameworkControlOutputTypeDef = TypedDict(
-    "_OptionalFrameworkControlOutputTypeDef",
-    {
-        "ControlInputParameters": List[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FrameworkControlOutputTypeDef(
-    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
-):
-    pass
-
-
 _RequiredFrameworkControlTypeDef = TypedDict(
     "_RequiredFrameworkControlTypeDef",
     {
         "ControlName": str,
     },
 )
 _OptionalFrameworkControlTypeDef = TypedDict(
@@ -1430,15 +1309,15 @@
 CreateBackupPlanOutputTypeDef = TypedDict(
     "CreateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBackupSelectionOutputTypeDef = TypedDict(
     "CreateBackupSelectionOutputTypeDef",
     {
@@ -1747,15 +1626,15 @@
 UpdateBackupPlanOutputTypeDef = TypedDict(
     "UpdateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFrameworkOutputTypeDef = TypedDict(
     "UpdateFrameworkOutputTypeDef",
     {
@@ -1808,14 +1687,30 @@
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -1832,24 +1727,14 @@
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
 
-RecoveryPointSelectionOutputTypeDef = TypedDict(
-    "RecoveryPointSelectionOutputTypeDef",
-    {
-        "VaultNames": List[str],
-        "ResourceIdentifiers": List[str],
-        "DateRange": DateRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": TimestampTypeDef,
         "ToDate": TimestampTypeDef,
     },
 )
@@ -2206,17 +2091,14 @@
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportDeliveryChannelUnionTypeDef = Union[
-    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2224,31 +2106,14 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingOutputTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
-ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2347,105 +2212,112 @@
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBackupSelectionOutputTypeDef = TypedDict(
-    "_RequiredBackupSelectionOutputTypeDef",
+_RequiredBackupSelectionTypeDef = TypedDict(
+    "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
-_OptionalBackupSelectionOutputTypeDef = TypedDict(
-    "_OptionalBackupSelectionOutputTypeDef",
+_OptionalBackupSelectionTypeDef = TypedDict(
+    "_OptionalBackupSelectionTypeDef",
     {
-        "Resources": List[str],
-        "ListOfTags": List[ConditionTypeDef],
-        "NotResources": List[str],
-        "Conditions": ConditionsOutputTypeDef,
+        "Resources": Sequence[str],
+        "ListOfTags": Sequence[ConditionTypeDef],
+        "NotResources": Sequence[str],
+        "Conditions": ConditionsTypeDef,
     },
     total=False,
 )
 
 
-class BackupSelectionOutputTypeDef(
-    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
-):
+class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
 
-_RequiredBackupSelectionTypeDef = TypedDict(
-    "_RequiredBackupSelectionTypeDef",
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
     {
-        "SelectionName": str,
-        "IamRoleArn": str,
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlTypeDef],
     },
 )
-_OptionalBackupSelectionTypeDef = TypedDict(
-    "_OptionalBackupSelectionTypeDef",
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
     {
-        "Resources": Sequence[str],
-        "ListOfTags": Sequence[ConditionTypeDef],
-        "NotResources": Sequence[str],
-        "Conditions": ConditionsTypeDef,
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
     pass
 
 
 DescribeFrameworkOutputTypeDef = TypedDict(
     "DescribeFrameworkOutputTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlOutputTypeDef],
+        "FrameworkControls": List[FrameworkControlTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-CreateLegalHoldOutputTypeDef = TypedDict(
-    "CreateLegalHoldOutputTypeDef",
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "FrameworkName": str,
+    },
+)
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
+    {
+        "ReportPlan": ReportPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetLegalHoldOutputTypeDef = TypedDict(
-    "GetLegalHoldOutputTypeDef",
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "CancelDescription": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "CancellationDate": datetime,
-        "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ReportPlans": List[ReportPlanTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryPointSelectionTypeDef = TypedDict(
     "RecoveryPointSelectionTypeDef",
     {
@@ -2469,31 +2341,14 @@
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
-    {
-        "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
-    {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
         "Rules": Sequence[BackupRuleInputTypeDef],
     },
 )
@@ -2516,37 +2371,24 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
-    {
-        "BackupSelection": BackupSelectionOutputTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2562,61 +2404,26 @@
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
-    },
-)
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
     {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
-        "IdempotencyToken": str,
+        "BackupSelection": BackupSelectionTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
         "Description": str,
     },
 )
@@ -2633,17 +2440,45 @@
 
 class CreateLegalHoldInputRequestTypeDef(
     _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
 ):
     pass
 
 
-RecoveryPointSelectionUnionTypeDef = Union[
-    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
-]
+CreateLegalHoldOutputTypeDef = TypedDict(
+    "CreateLegalHoldOutputTypeDef",
+    {
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLegalHoldOutputTypeDef = TypedDict(
+    "GetLegalHoldOutputTypeDef",
+    {
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "CancelDescription": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "CancellationDate": datetime,
+        "RetainRecordUntil": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2693,11 +2528,11 @@
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.pyi` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingOutputTypeDef
+    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingTypeDef
 
-    data: AdvancedBackupSettingOutputTypeDef = ...
+    data: AdvancedBackupSettingTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -31,33 +31,30 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
-    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "DateRangeOutputTypeDef",
     "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
@@ -102,17 +99,15 @@
     "RecoveryPointByResourceTypeDef",
     "ListReportPlansInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
-    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
-    "ReportSettingOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
     "StartRestoreJobInputRequestTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
@@ -120,17 +115,15 @@
     "BackupJobTypeDef",
     "CopyJobTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
-    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
     "CreateBackupPlanOutputTypeDef",
     "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultOutputTypeDef",
     "CreateFrameworkOutputTypeDef",
     "CreateReportPlanOutputTypeDef",
     "DeleteBackupPlanOutputTypeDef",
@@ -156,16 +149,16 @@
     "StartReportJobOutputTypeDef",
     "StartRestoreJobOutputTypeDef",
     "UpdateBackupPlanOutputTypeDef",
     "UpdateFrameworkOutputTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
+    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
-    "RecoveryPointSelectionOutputTypeDef",
     "DateRangeTypeDef",
     "ListBackupJobsInputRequestTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
@@ -183,62 +176,46 @@
     "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
-    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
-    "ReportPlanTypeDef",
-    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
-    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "FrameworkControlUnionTypeDef",
-    "CreateLegalHoldOutputTypeDef",
-    "GetLegalHoldOutputTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "GetBackupSelectionOutputTypeDef",
-    "BackupSelectionUnionTypeDef",
     "CreateBackupSelectionInputRequestTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
+    "GetBackupSelectionOutputTypeDef",
     "CreateLegalHoldInputRequestTypeDef",
-    "RecoveryPointSelectionUnionTypeDef",
+    "CreateLegalHoldOutputTypeDef",
+    "GetLegalHoldOutputTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
-AdvancedBackupSettingOutputTypeDef = TypedDict(
-    "AdvancedBackupSettingOutputTypeDef",
-    {
-        "ResourceType": str,
-        "BackupOptions": Dict[str, str],
-    },
-    total=False,
-)
-
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -355,24 +332,14 @@
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
-ControlScopeOutputTypeDef = TypedDict(
-    "ControlScopeOutputTypeDef",
-    {
-        "ComplianceResourceIds": List[str],
-        "ComplianceResourceTypes": List[str],
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
@@ -448,22 +415,14 @@
     },
     total=False,
 )
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
-DateRangeOutputTypeDef = TypedDict(
-    "DateRangeOutputTypeDef",
-    {
-        "FromDate": datetime,
-        "ToDate": datetime,
-    },
-)
-
 TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
@@ -994,66 +953,23 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
-_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
-    "_RequiredReportDeliveryChannelOutputTypeDef",
-    {
-        "S3BucketName": str,
-    },
-)
-_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
-    "_OptionalReportDeliveryChannelOutputTypeDef",
-    {
-        "S3KeyPrefix": str,
-        "Formats": List[str],
-    },
-    total=False,
-)
-
-class ReportDeliveryChannelOutputTypeDef(
-    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
-):
-    pass
-
 ReportDestinationTypeDef = TypedDict(
     "ReportDestinationTypeDef",
     {
         "S3BucketName": str,
         "S3Keys": List[str],
     },
     total=False,
 )
 
-_RequiredReportSettingOutputTypeDef = TypedDict(
-    "_RequiredReportSettingOutputTypeDef",
-    {
-        "ReportTemplate": str,
-    },
-)
-_OptionalReportSettingOutputTypeDef = TypedDict(
-    "_OptionalReportSettingOutputTypeDef",
-    {
-        "FrameworkArns": List[str],
-        "NumberOfFrameworks": int,
-        "Accounts": List[str],
-        "OrganizationUnits": List[str],
-        "Regions": List[str],
-    },
-    total=False,
-)
-
-class ReportSettingOutputTypeDef(
-    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
-):
-    pass
-
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1139,15 +1055,15 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
@@ -1318,56 +1234,25 @@
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
     },
     total=False,
 )
 
-ConditionsOutputTypeDef = TypedDict(
-    "ConditionsOutputTypeDef",
-    {
-        "StringEquals": List[ConditionParameterTypeDef],
-        "StringNotEquals": List[ConditionParameterTypeDef],
-        "StringLike": List[ConditionParameterTypeDef],
-        "StringNotLike": List[ConditionParameterTypeDef],
-    },
-    total=False,
-)
-
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "StringEquals": Sequence[ConditionParameterTypeDef],
         "StringNotEquals": Sequence[ConditionParameterTypeDef],
         "StringLike": Sequence[ConditionParameterTypeDef],
         "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredFrameworkControlOutputTypeDef = TypedDict(
-    "_RequiredFrameworkControlOutputTypeDef",
-    {
-        "ControlName": str,
-    },
-)
-_OptionalFrameworkControlOutputTypeDef = TypedDict(
-    "_OptionalFrameworkControlOutputTypeDef",
-    {
-        "ControlInputParameters": List[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeOutputTypeDef,
-    },
-    total=False,
-)
-
-class FrameworkControlOutputTypeDef(
-    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
-):
-    pass
-
 _RequiredFrameworkControlTypeDef = TypedDict(
     "_RequiredFrameworkControlTypeDef",
     {
         "ControlName": str,
     },
 )
 _OptionalFrameworkControlTypeDef = TypedDict(
@@ -1385,15 +1270,15 @@
 CreateBackupPlanOutputTypeDef = TypedDict(
     "CreateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBackupSelectionOutputTypeDef = TypedDict(
     "CreateBackupSelectionOutputTypeDef",
     {
@@ -1702,15 +1587,15 @@
 UpdateBackupPlanOutputTypeDef = TypedDict(
     "UpdateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFrameworkOutputTypeDef = TypedDict(
     "UpdateFrameworkOutputTypeDef",
     {
@@ -1761,14 +1646,30 @@
 )
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -1783,24 +1684,14 @@
 )
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
-RecoveryPointSelectionOutputTypeDef = TypedDict(
-    "RecoveryPointSelectionOutputTypeDef",
-    {
-        "VaultNames": List[str],
-        "ResourceIdentifiers": List[str],
-        "DateRange": DateRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": TimestampTypeDef,
         "ToDate": TimestampTypeDef,
     },
 )
@@ -2145,17 +2036,14 @@
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportDeliveryChannelUnionTypeDef = Union[
-    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2163,31 +2051,14 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingOutputTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
-ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2282,101 +2153,106 @@
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBackupSelectionOutputTypeDef = TypedDict(
-    "_RequiredBackupSelectionOutputTypeDef",
+_RequiredBackupSelectionTypeDef = TypedDict(
+    "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
-_OptionalBackupSelectionOutputTypeDef = TypedDict(
-    "_OptionalBackupSelectionOutputTypeDef",
+_OptionalBackupSelectionTypeDef = TypedDict(
+    "_OptionalBackupSelectionTypeDef",
     {
-        "Resources": List[str],
-        "ListOfTags": List[ConditionTypeDef],
-        "NotResources": List[str],
-        "Conditions": ConditionsOutputTypeDef,
+        "Resources": Sequence[str],
+        "ListOfTags": Sequence[ConditionTypeDef],
+        "NotResources": Sequence[str],
+        "Conditions": ConditionsTypeDef,
     },
     total=False,
 )
 
-class BackupSelectionOutputTypeDef(
-    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
-):
+class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
-_RequiredBackupSelectionTypeDef = TypedDict(
-    "_RequiredBackupSelectionTypeDef",
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
     {
-        "SelectionName": str,
-        "IamRoleArn": str,
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlTypeDef],
     },
 )
-_OptionalBackupSelectionTypeDef = TypedDict(
-    "_OptionalBackupSelectionTypeDef",
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
     {
-        "Resources": Sequence[str],
-        "ListOfTags": Sequence[ConditionTypeDef],
-        "NotResources": Sequence[str],
-        "Conditions": ConditionsTypeDef,
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
     },
     total=False,
 )
 
-class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
     pass
 
 DescribeFrameworkOutputTypeDef = TypedDict(
     "DescribeFrameworkOutputTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlOutputTypeDef],
+        "FrameworkControls": List[FrameworkControlTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-CreateLegalHoldOutputTypeDef = TypedDict(
-    "CreateLegalHoldOutputTypeDef",
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "FrameworkName": str,
+    },
+)
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
+    {
+        "ReportPlan": ReportPlanTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetLegalHoldOutputTypeDef = TypedDict(
-    "GetLegalHoldOutputTypeDef",
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "CancelDescription": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "CancellationDate": datetime,
-        "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ReportPlans": List[ReportPlanTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryPointSelectionTypeDef = TypedDict(
     "RecoveryPointSelectionTypeDef",
     {
@@ -2400,31 +2276,14 @@
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
-    {
-        "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
-    {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
         "Rules": Sequence[BackupRuleInputTypeDef],
     },
 )
@@ -2445,35 +2304,22 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
-    {
-        "BackupSelection": BackupSelectionOutputTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2487,57 +2333,26 @@
 
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
-    },
-)
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
-    pass
-
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
     {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
-        "IdempotencyToken": str,
+        "BackupSelection": BackupSelectionTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
         "Description": str,
     },
 )
@@ -2552,17 +2367,45 @@
 )
 
 class CreateLegalHoldInputRequestTypeDef(
     _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
 ):
     pass
 
-RecoveryPointSelectionUnionTypeDef = Union[
-    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
-]
+CreateLegalHoldOutputTypeDef = TypedDict(
+    "CreateLegalHoldOutputTypeDef",
+    {
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLegalHoldOutputTypeDef = TypedDict(
+    "GetLegalHoldOutputTypeDef",
+    {
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "CancelDescription": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "CancellationDate": datetime,
+        "RetainRecordUntil": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2610,11 +2453,11 @@
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/SOURCES.txt` & `types-aiobotocore-backup-2.5.2.post2/types_aiobotocore_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

