# Comparing `tmp/types-aiobotocore-ssm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ssm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-ssm-2.5.2.post1.tar` & `types-aiobotocore-ssm-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.073449 types-aiobotocore-ssm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48263 2023-08-02 14:53:04.069448 types-aiobotocore-ssm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46761 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.073449 types-aiobotocore-ssm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.065448 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136861 2023-08-02 14:50:04.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   136666 2023-08-02 14:50:01.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28097 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    61436 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    61387 2023-08-02 14:50:04.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   215372 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   215130 2023-08-02 14:50:07.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.069448 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48263 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21973 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20471 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12771 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12770 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   136556 2023-08-04 13:54:08.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   136361 2023-08-04 13:54:07.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28212 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28210 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61421 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61372 2023-08-04 13:54:08.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   204193 2023-08-04 13:54:17.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   203965 2023-08-04 13:54:15.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1571 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1570 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21973 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/LICENSE` & `types-aiobotocore-ssm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post1/setup.py` & `types-aiobotocore-ssm-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__main__.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -91,31 +91,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationUnionTypeDef,
+    AlarmConfigurationTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusUnionTypeDef,
+    AssociationStatusTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryUnionTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryUnionTypeDef,
+    CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -210,57 +210,57 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigUnionTypeDef,
+    NotificationConfigTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupUnionTypeDef,
+    PatchFilterGroupTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupUnionTypeDef,
-    PatchSourceUnionTypeDef,
+    PatchRuleGroupTypeDef,
+    PatchSourceTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookUnionTypeDef,
+    RunbookTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationUnionTypeDef,
-    TargetUnionTypeDef,
+    TargetLocationTypeDef,
+    TargetTypeDef,
     TerminateSessionResponseTypeDef,
     TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -273,26 +273,23 @@
 from .waiter import CommandExecutedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     AssociatedInstances: Type[BotocoreClientError]
     AssociationAlreadyExists: Type[BotocoreClientError]
     AssociationDoesNotExist: Type[BotocoreClientError]
     AssociationExecutionDoesNotExist: Type[BotocoreClientError]
     AssociationLimitExceeded: Type[BotocoreClientError]
@@ -416,15 +413,14 @@
     UnsupportedFeatureRequiredException: Type[BotocoreClientError]
     UnsupportedInventoryItemContextException: Type[BotocoreClientError]
     UnsupportedInventorySchemaVersionException: Type[BotocoreClientError]
     UnsupportedOperatingSystem: Type[BotocoreClientError]
     UnsupportedParameterType: Type[BotocoreClientError]
     UnsupportedPlatformType: Type[BotocoreClientError]
 
-
 class SSMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
     """
 
     meta: ClientMeta
@@ -433,76 +429,69 @@
     def exceptions(self) -> Exceptions:
         """
         SSMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#exceptions)
         """
-
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
         Tags: Sequence[TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
-
     async def associate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationType: str, ResourceType: str, ResourceUri: str
     ) -> AssociateOpsItemRelatedItemResponseTypeDef:
         """
         Associates a related item to a Systems Manager OpsCenter OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.associate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#associate_ops_item_related_item)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#can_paginate)
         """
-
     async def cancel_command(
         self, *, CommandId: str, InstanceIds: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Attempts to cancel the command specified by the Command ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_command)
         """
-
     async def cancel_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> CancelMaintenanceWindowExecutionResultTypeDef:
         """
         Stops a maintenance window execution that is already in progress and cancels any
         tasks in the window that haven't already starting running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_maintenance_window_execution)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#close)
         """
-
     async def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
@@ -514,58 +503,55 @@
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_activation)
         """
-
     async def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association)
         """
-
     async def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association_batch)
         """
-
     async def create_document(
         self,
         *,
         Content: str,
         Name: str,
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
@@ -578,15 +564,14 @@
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
-
     async def create_maintenance_window(
         self,
         *,
         Name: str,
         Schedule: str,
         Duration: int,
         Cutoff: int,
@@ -601,15 +586,14 @@
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
-
     async def create_ops_item(
         self,
         *,
         Description: str,
         Source: str,
         Title: str,
         OpsItemType: str = ...,
@@ -628,15 +612,14 @@
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
-
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateOpsMetadataResultTypeDef:
@@ -644,39 +627,37 @@
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_metadata)
         """
-
     async def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
-        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
+        GlobalFilters: PatchFilterGroupTypeDef = ...,
+        ApprovalRules: PatchRuleGroupTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
+        Sources: Sequence[PatchSourceTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
-
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
         SyncSource: ResourceDataSyncSourceTypeDef = ...
@@ -684,45 +665,41 @@
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
         """
-
     async def delete_activation(self, *, ActivationId: str) -> Dict[str, Any]:
         """
         Deletes an activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_activation)
         """
-
     async def delete_association(
         self, *, Name: str = ..., InstanceId: str = ..., AssociationId: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociates the specified Amazon Web Services Systems Manager document (SSM
         document) from the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_association)
         """
-
     async def delete_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ..., Force: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon Web Services Systems Manager document (SSM document) and all
         managed node associations to the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_document)
         """
-
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
@@ -730,115 +707,103 @@
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
         """
-
     async def delete_maintenance_window(
         self, *, WindowId: str
     ) -> DeleteMaintenanceWindowResultTypeDef:
         """
         Deletes a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_maintenance_window)
         """
-
     async def delete_ops_metadata(self, *, OpsMetadataArn: str) -> Dict[str, Any]:
         """
         Delete OpsMetadata related to an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_ops_metadata)
         """
-
     async def delete_parameter(self, *, Name: str) -> Dict[str, Any]:
         """
         Delete a parameter from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameter)
         """
-
     async def delete_parameters(self, *, Names: Sequence[str]) -> DeleteParametersResultTypeDef:
         """
         Delete a list of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameters)
         """
-
     async def delete_patch_baseline(self, *, BaselineId: str) -> DeletePatchBaselineResultTypeDef:
         """
         Deletes a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_patch_baseline)
         """
-
     async def delete_resource_data_sync(
         self, *, SyncName: str, SyncType: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource data sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_data_sync)
         """
-
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyId: str, PolicyHash: str
     ) -> Dict[str, Any]:
         """
         Deletes a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_policy)
         """
-
     async def deregister_managed_instance(self, *, InstanceId: str) -> Dict[str, Any]:
         """
         Removes the server or virtual machine from the list of registered servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_managed_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_managed_instance)
         """
-
     async def deregister_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> DeregisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Removes a patch group from a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_patch_baseline_for_patch_group)
         """
-
     async def deregister_target_from_maintenance_window(
         self, *, WindowId: str, WindowTargetId: str, Safe: bool = ...
     ) -> DeregisterTargetFromMaintenanceWindowResultTypeDef:
         """
         Removes a target from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_target_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_target_from_maintenance_window)
         """
-
     async def deregister_task_from_maintenance_window(
         self, *, WindowId: str, WindowTaskId: str
     ) -> DeregisterTaskFromMaintenanceWindowResultTypeDef:
         """
         Removes a task from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_task_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_task_from_maintenance_window)
         """
-
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeActivationsResultTypeDef:
@@ -847,30 +812,28 @@
         was created, its expiration date, the Identity and Access Management (IAM) role
         assigned to the managed nodes in the activation, and the number of nodes
         registered by using this activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_activations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_activations)
         """
-
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
         AssociationVersion: str = ...
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
-
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -878,44 +841,41 @@
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
-
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
-
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
-
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -924,40 +884,37 @@
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
-
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
-
     async def describe_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ...
     ) -> DescribeDocumentResultTypeDef:
         """
         Describes the specified Amazon Web Services Systems Manager document (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document)
         """
-
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
         NextToken: str = ...
@@ -965,73 +922,67 @@
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document_permission)
         """
-
     async def describe_effective_instance_associations(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectiveInstanceAssociationsResultTypeDef:
         """
         All associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_instance_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_instance_associations)
         """
-
     async def describe_effective_patches_for_patch_baseline(
         self, *, BaselineId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:
         """
         Retrieves the current effective patches (the patch and the approval state) for
         the specified patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_patches_for_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_patches_for_patch_baseline)
         """
-
     async def describe_instance_associations_status(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeInstanceAssociationsStatusResultTypeDef:
         """
         The status of the associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_associations_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_associations_status)
         """
-
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeInstanceInformationResultTypeDef:
         """
-        Describes one or more of your managed nodes, including information about the
-        operating system platform, the version of SSM Agent installed on the managed
-        node, node status, and so on.
+        Provides information about one or more of your managed nodes, including the
+        operating system platform, SSM Agent version, association status, and IP
+        address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_information)
         """
-
     async def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInstancePatchStatesResultTypeDef:
         """
         Retrieves the high-level patch state of one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states)
         """
-
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1039,15 +990,14 @@
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states_for_patch_group)
         """
-
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1055,25 +1005,23 @@
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patches)
         """
-
     async def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_inventory_deletions)
         """
-
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -1082,190 +1030,177 @@
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_task_invocations)
         """
-
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
-
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
-
     async def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
-
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
-
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
-
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
-
     async def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows_for_target)
         """
-
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
-
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
-
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
-
     async def describe_patch_group_state(
         self, *, PatchGroup: str
     ) -> DescribePatchGroupStateResultTypeDef:
         """
         Returns high-level aggregated patch compliance state information for a patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_group_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_group_state)
         """
-
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
-
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
@@ -1274,15 +1209,14 @@
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_properties)
         """
-
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[SessionFilterTypeDef] = ...
@@ -1290,100 +1224,91 @@
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_sessions)
         """
-
     async def disassociate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationId: str
     ) -> Dict[str, Any]:
         """
         Deletes the association between an OpsItem and a related item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.disassociate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#disassociate_ops_item_related_item)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#generate_presigned_url)
         """
-
     async def get_automation_execution(
         self, *, AutomationExecutionId: str
     ) -> GetAutomationExecutionResultTypeDef:
         """
         Get detailed information about a particular Automation execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_automation_execution)
         """
-
     async def get_calendar_state(
         self, *, CalendarNames: Sequence[str], AtTime: str = ...
     ) -> GetCalendarStateResponseTypeDef:
         """
         Gets the state of a Amazon Web Services Systems Manager change calendar at the
         current time or a specified time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_calendar_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_calendar_state)
         """
-
     async def get_command_invocation(
         self, *, CommandId: str, InstanceId: str, PluginName: str = ...
     ) -> GetCommandInvocationResultTypeDef:
         """
         Returns detailed information about command execution for an invocation or
         plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_command_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_command_invocation)
         """
-
     async def get_connection_status(self, *, Target: str) -> GetConnectionStatusResponseTypeDef:
         """
         Retrieves the Session Manager connection status for a managed node to determine
         whether it is running and ready to receive Session Manager connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_connection_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_connection_status)
         """
-
     async def get_default_patch_baseline(
         self, *, OperatingSystem: OperatingSystemType = ...
     ) -> GetDefaultPatchBaselineResultTypeDef:
         """
         Retrieves the default patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_default_patch_baseline)
         """
-
     async def get_deployable_patch_snapshot_for_instance(
         self, *, InstanceId: str, SnapshotId: str, BaselineOverride: BaselineOverrideTypeDef = ...
     ) -> GetDeployablePatchSnapshotForInstanceResultTypeDef:
         """
         Retrieves the current snapshot for the patch baseline the managed node uses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_deployable_patch_snapshot_for_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_deployable_patch_snapshot_for_instance)
         """
-
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...
@@ -1391,15 +1316,14 @@
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_document)
         """
-
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
@@ -1407,15 +1331,14 @@
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
-
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
@@ -1424,84 +1347,76 @@
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory_schema)
         """
-
     async def get_maintenance_window(self, *, WindowId: str) -> GetMaintenanceWindowResultTypeDef:
         """
         Retrieves a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window)
         """
-
     async def get_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> GetMaintenanceWindowExecutionResultTypeDef:
         """
         Retrieves details about a specific a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution)
         """
-
     async def get_maintenance_window_execution_task(
         self, *, WindowExecutionId: str, TaskId: str
     ) -> GetMaintenanceWindowExecutionTaskResultTypeDef:
         """
         Retrieves the details about a specific task run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task)
         """
-
     async def get_maintenance_window_execution_task_invocation(
         self, *, WindowExecutionId: str, TaskId: str, InvocationId: str
     ) -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:
         """
         Retrieves information about a specific task running on a specific target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task_invocation)
         """
-
     async def get_maintenance_window_task(
         self, *, WindowId: str, WindowTaskId: str
     ) -> GetMaintenanceWindowTaskResultTypeDef:
         """
         Retrieves the details of a maintenance window task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_task)
         """
-
     async def get_ops_item(
         self, *, OpsItemId: str, OpsItemArn: str = ...
     ) -> GetOpsItemResponseTypeDef:
         """
         Get information about an OpsItem by using the ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_item)
         """
-
     async def get_ops_metadata(
         self, *, OpsMetadataArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetOpsMetadataResultTypeDef:
         """
         View operational metadata related to an application in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_metadata)
         """
-
     async def get_ops_summary(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
@@ -1511,46 +1426,42 @@
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
         """
-
     async def get_parameter(
         self, *, Name: str, WithDecryption: bool = ...
     ) -> GetParameterResultTypeDef:
         """
         Get information about a single parameter by specifying the parameter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter)
         """
-
     async def get_parameter_history(
         self, *, Name: str, WithDecryption: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> GetParameterHistoryResultTypeDef:
         """
         Retrieves the history of all changes to a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter_history)
         """
-
     async def get_parameters(
         self, *, Names: Sequence[str], WithDecryption: bool = ...
     ) -> GetParametersResultTypeDef:
         """
         Get information about one or more parameters by specifying multiple parameter
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters)
         """
-
     async def get_parameters_by_path(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
@@ -1559,87 +1470,79 @@
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
-
     async def get_patch_baseline(self, *, BaselineId: str) -> GetPatchBaselineResultTypeDef:
         """
         Retrieves information about a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline)
         """
-
     async def get_patch_baseline_for_patch_group(
         self, *, PatchGroup: str, OperatingSystem: OperatingSystemType = ...
     ) -> GetPatchBaselineForPatchGroupResultTypeDef:
         """
         Retrieves the patch baseline that should be used for the specified patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline_for_patch_group)
         """
-
     async def get_resource_policies(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Returns an array of the `Policy` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_resource_policies)
         """
-
     async def get_service_setting(self, *, SettingId: str) -> GetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_service_setting)
         """
-
     async def label_parameter_version(
         self, *, Name: str, Labels: Sequence[str], ParameterVersion: int = ...
     ) -> LabelParameterVersionResultTypeDef:
         """
         A parameter label is a user-defined alias to help you manage different versions
         of a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.label_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#label_parameter_version)
         """
-
     async def list_association_versions(
         self, *, AssociationId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationVersionsResultTypeDef:
         """
         Retrieves all versions of an association for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_association_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_association_versions)
         """
-
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_associations)
         """
-
     async def list_command_invocations(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1648,15 +1551,14 @@
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
-
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1664,15 +1566,14 @@
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
-
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -1681,30 +1582,28 @@
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_items)
         """
-
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_summaries)
         """
-
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
@@ -1713,25 +1612,23 @@
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
         """
-
     async def list_document_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDocumentVersionsResultTypeDef:
         """
         List all versions for a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_versions)
         """
-
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1739,15 +1636,14 @@
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_documents)
         """
-
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
@@ -1755,30 +1651,28 @@
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
-
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_events)
         """
-
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1786,64 +1680,59 @@
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
-
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying all
         Application Manager OpsMetadata objects or blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_metadata)
         """
-
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
-
     async def list_resource_data_sync(
         self, *, SyncType: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListResourceDataSyncResultTypeDef:
         """
         Lists your resource data sync configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_data_sync)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str
     ) -> ListTagsForResourceResultTypeDef:
         """
         Returns a list of the tags assigned to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_tags_for_resource)
         """
-
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
@@ -1852,44 +1741,41 @@
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
         """
-
     async def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
+        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
         """
-
     async def put_inventory(
         self, *, InstanceId: str, Items: Sequence[InventoryItemTypeDef]
     ) -> PutInventoryResultTypeDef:
         """
         Bulk update custom inventory items on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_inventory)
         """
-
     async def put_parameter(
         self,
         *,
         Name: str,
         Value: str,
         Description: str = ...,
         Type: ParameterTypeType = ...,
@@ -1903,199 +1789,184 @@
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
-
     async def put_resource_policy(
         self, *, ResourceArn: str, Policy: str, PolicyId: str = ..., PolicyHash: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_resource_policy)
         """
-
     async def register_default_patch_baseline(
         self, *, BaselineId: str
     ) -> RegisterDefaultPatchBaselineResultTypeDef:
         """
         Defines the default patch baseline for the relevant operating system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_default_patch_baseline)
         """
-
     async def register_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> RegisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Registers a patch baseline for a patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_patch_baseline_for_patch_group)
         """
-
     async def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
-
     async def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[
-            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
-        ] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
+        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
-
     async def remove_tags_from_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str, TagKeys: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Removes tag keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.remove_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#remove_tags_from_resource)
         """
-
     async def reset_service_setting(self, *, SettingId: str) -> ResetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.reset_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#reset_service_setting)
         """
-
     async def resume_session(self, *, SessionId: str) -> ResumeSessionResponseTypeDef:
         """
         Reconnects a session to a managed node after it has been disconnected.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.resume_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#resume_session)
         """
-
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
         Payload: Mapping[str, Sequence[str]] = ...
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_automation_signal)
         """
-
     async def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigUnionTypeDef = ...,
+        NotificationConfig: NotificationConfigTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
-
     async def start_associations_once(self, *, AssociationIds: Sequence[str]) -> Dict[str, Any]:
         """
         Runs an association immediately and only one time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_associations_once)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_associations_once)
         """
-
     async def start_automation_execution(
         self,
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
-
     async def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookUnionTypeDef],
+        Runbooks: Sequence[RunbookTypeDef],
         ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -2104,15 +1975,14 @@
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
-
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...
@@ -2120,86 +1990,80 @@
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_session)
         """
-
     async def stop_automation_execution(
         self, *, AutomationExecutionId: str, Type: StopTypeType = ...
     ) -> Dict[str, Any]:
         """
         Stop an Automation that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.stop_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#stop_automation_execution)
         """
-
     async def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
         """
         Permanently ends a session and closes the data connection between the Session
         Manager client and SSM Agent on the managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.terminate_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#terminate_session)
         """
-
     async def unlabel_parameter_version(
         self, *, Name: str, ParameterVersion: int, Labels: Sequence[str]
     ) -> UnlabelParameterVersionResultTypeDef:
         """
         Remove a label or labels from a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.unlabel_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#unlabel_parameter_version)
         """
-
     async def update_association(
         self,
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
-
     async def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association_status)
         """
-
     async def update_document(
         self,
         *,
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
@@ -2210,36 +2074,33 @@
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
-
     async def update_document_default_version(
         self, *, Name: str, DocumentVersion: str
     ) -> UpdateDocumentDefaultVersionResultTypeDef:
         """
         Set the default version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_default_version)
         """
-
     async def update_document_metadata(
         self, *, Name: str, DocumentReviews: DocumentReviewsTypeDef, DocumentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates information related to approval reviews for a specific version of a
         change template in Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_metadata)
         """
-
     async def update_maintenance_window(
         self,
         *,
         WindowId: str,
         Name: str = ...,
         Description: str = ...,
         StartDate: str = ...,
@@ -2255,73 +2116,67 @@
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
-
     async def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
-
     async def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[
-            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
-        ] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
+        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
-
     async def update_managed_instance_role(
         self, *, InstanceId: str, IamRole: str
     ) -> Dict[str, Any]:
         """
         Changes the Identity and Access Management (IAM) role that is assigned to the
         on-premises server, edge device, or virtual machines (VM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_managed_instance_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_managed_instance_role)
         """
-
     async def update_ops_item(
         self,
         *,
         OpsItemId: str,
         Description: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         OperationalDataToDelete: Sequence[str] = ...,
@@ -2340,496 +2195,442 @@
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
-
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
         KeysToDelete: Sequence[str] = ...
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_metadata)
         """
-
     async def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
-        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
+        GlobalFilters: PatchFilterGroupTypeDef = ...,
+        ApprovalRules: PatchRuleGroupTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
+        Sources: Sequence[PatchSourceTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
-
     async def update_resource_data_sync(
         self, *, SyncName: str, SyncType: str, SyncSource: ResourceDataSyncSourceTypeDef
     ) -> Dict[str, Any]:
         """
         Update a resource data sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_resource_data_sync)
         """
-
     async def update_service_setting(self, *, SettingId: str, SettingValue: str) -> Dict[str, Any]:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_service_setting)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_activations"]
     ) -> DescribeActivationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_execution_targets"]
     ) -> DescribeAssociationExecutionTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_executions"]
     ) -> DescribeAssociationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_executions"]
     ) -> DescribeAutomationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_step_executions"]
     ) -> DescribeAutomationStepExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_available_patches"]
     ) -> DescribeAvailablePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_instance_associations"]
     ) -> DescribeEffectiveInstanceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_patches_for_patch_baseline"]
     ) -> DescribeEffectivePatchesForPatchBaselinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_associations_status"]
     ) -> DescribeInstanceAssociationsStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_information"]
     ) -> DescribeInstanceInformationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states"]
     ) -> DescribeInstancePatchStatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states_for_patch_group"]
     ) -> DescribeInstancePatchStatesForPatchGroupPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patches"]
     ) -> DescribeInstancePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_task_invocations"]
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_tasks"]
     ) -> DescribeMaintenanceWindowExecutionTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_executions"]
     ) -> DescribeMaintenanceWindowExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_schedule"]
     ) -> DescribeMaintenanceWindowSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_targets"]
     ) -> DescribeMaintenanceWindowTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_tasks"]
     ) -> DescribeMaintenanceWindowTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows"]
     ) -> DescribeMaintenanceWindowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows_for_target"]
     ) -> DescribeMaintenanceWindowsForTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_ops_items"]
     ) -> DescribeOpsItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_parameters"]
     ) -> DescribeParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_baselines"]
     ) -> DescribePatchBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_groups"]
     ) -> DescribePatchGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_properties"]
     ) -> DescribePatchPropertiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_sessions"]
     ) -> DescribeSessionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_inventory"]) -> GetInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_inventory_schema"]
     ) -> GetInventorySchemaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_ops_summary"]) -> GetOpsSummaryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameter_history"]
     ) -> GetParameterHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameters_by_path"]
     ) -> GetParametersByPathPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_association_versions"]
     ) -> ListAssociationVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations"]
     ) -> ListAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_command_invocations"]
     ) -> ListCommandInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_commands"]) -> ListCommandsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_items"]
     ) -> ListComplianceItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_summaries"]
     ) -> ListComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_versions"]
     ) -> ListDocumentVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_documents"]) -> ListDocumentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_events"]
     ) -> ListOpsItemEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_related_items"]
     ) -> ListOpsItemRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_metadata"]
     ) -> ListOpsMetadataPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_compliance_summaries"]
     ) -> ListResourceComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_data_sync"]
     ) -> ListResourceDataSyncPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     def get_waiter(self, waiter_name: Literal["command_executed"]) -> CommandExecutedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "SSMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,31 +91,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationUnionTypeDef,
+    AlarmConfigurationTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusUnionTypeDef,
+    AssociationStatusTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryUnionTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryUnionTypeDef,
+    CreateAssociationBatchRequestEntryTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -210,57 +210,57 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigUnionTypeDef,
+    NotificationConfigTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupUnionTypeDef,
+    PatchFilterGroupTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupUnionTypeDef,
-    PatchSourceUnionTypeDef,
+    PatchRuleGroupTypeDef,
+    PatchSourceTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookUnionTypeDef,
+    RunbookTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationUnionTypeDef,
-    TargetUnionTypeDef,
+    TargetLocationTypeDef,
+    TargetTypeDef,
     TerminateSessionResponseTypeDef,
     TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -273,23 +273,26 @@
 from .waiter import CommandExecutedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SSMClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     AssociatedInstances: Type[BotocoreClientError]
     AssociationAlreadyExists: Type[BotocoreClientError]
     AssociationDoesNotExist: Type[BotocoreClientError]
     AssociationExecutionDoesNotExist: Type[BotocoreClientError]
     AssociationLimitExceeded: Type[BotocoreClientError]
@@ -413,14 +416,15 @@
     UnsupportedFeatureRequiredException: Type[BotocoreClientError]
     UnsupportedInventoryItemContextException: Type[BotocoreClientError]
     UnsupportedInventorySchemaVersionException: Type[BotocoreClientError]
     UnsupportedOperatingSystem: Type[BotocoreClientError]
     UnsupportedParameterType: Type[BotocoreClientError]
     UnsupportedPlatformType: Type[BotocoreClientError]
 
+
 class SSMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
     """
 
     meta: ClientMeta
@@ -429,69 +433,76 @@
     def exceptions(self) -> Exceptions:
         """
         SSMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#exceptions)
         """
+
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
         Tags: Sequence[TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
+
     async def associate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationType: str, ResourceType: str, ResourceUri: str
     ) -> AssociateOpsItemRelatedItemResponseTypeDef:
         """
         Associates a related item to a Systems Manager OpsCenter OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.associate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#associate_ops_item_related_item)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#can_paginate)
         """
+
     async def cancel_command(
         self, *, CommandId: str, InstanceIds: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Attempts to cancel the command specified by the Command ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_command)
         """
+
     async def cancel_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> CancelMaintenanceWindowExecutionResultTypeDef:
         """
         Stops a maintenance window execution that is already in progress and cancels any
         tasks in the window that haven't already starting running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_maintenance_window_execution)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#close)
         """
+
     async def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
@@ -503,55 +514,58 @@
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_activation)
         """
+
     async def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association)
         """
+
     async def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association_batch)
         """
+
     async def create_document(
         self,
         *,
         Content: str,
         Name: str,
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
@@ -564,14 +578,15 @@
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
+
     async def create_maintenance_window(
         self,
         *,
         Name: str,
         Schedule: str,
         Duration: int,
         Cutoff: int,
@@ -586,14 +601,15 @@
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
+
     async def create_ops_item(
         self,
         *,
         Description: str,
         Source: str,
         Title: str,
         OpsItemType: str = ...,
@@ -612,14 +628,15 @@
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
+
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateOpsMetadataResultTypeDef:
@@ -627,37 +644,39 @@
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_metadata)
         """
+
     async def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
-        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
+        GlobalFilters: PatchFilterGroupTypeDef = ...,
+        ApprovalRules: PatchRuleGroupTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
+        Sources: Sequence[PatchSourceTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
+
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
         SyncSource: ResourceDataSyncSourceTypeDef = ...
@@ -665,41 +684,45 @@
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
         """
+
     async def delete_activation(self, *, ActivationId: str) -> Dict[str, Any]:
         """
         Deletes an activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_activation)
         """
+
     async def delete_association(
         self, *, Name: str = ..., InstanceId: str = ..., AssociationId: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociates the specified Amazon Web Services Systems Manager document (SSM
         document) from the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_association)
         """
+
     async def delete_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ..., Force: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon Web Services Systems Manager document (SSM document) and all
         managed node associations to the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_document)
         """
+
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
@@ -707,103 +730,115 @@
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
         """
+
     async def delete_maintenance_window(
         self, *, WindowId: str
     ) -> DeleteMaintenanceWindowResultTypeDef:
         """
         Deletes a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_maintenance_window)
         """
+
     async def delete_ops_metadata(self, *, OpsMetadataArn: str) -> Dict[str, Any]:
         """
         Delete OpsMetadata related to an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_ops_metadata)
         """
+
     async def delete_parameter(self, *, Name: str) -> Dict[str, Any]:
         """
         Delete a parameter from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameter)
         """
+
     async def delete_parameters(self, *, Names: Sequence[str]) -> DeleteParametersResultTypeDef:
         """
         Delete a list of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameters)
         """
+
     async def delete_patch_baseline(self, *, BaselineId: str) -> DeletePatchBaselineResultTypeDef:
         """
         Deletes a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_patch_baseline)
         """
+
     async def delete_resource_data_sync(
         self, *, SyncName: str, SyncType: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource data sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_data_sync)
         """
+
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyId: str, PolicyHash: str
     ) -> Dict[str, Any]:
         """
         Deletes a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_policy)
         """
+
     async def deregister_managed_instance(self, *, InstanceId: str) -> Dict[str, Any]:
         """
         Removes the server or virtual machine from the list of registered servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_managed_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_managed_instance)
         """
+
     async def deregister_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> DeregisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Removes a patch group from a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_patch_baseline_for_patch_group)
         """
+
     async def deregister_target_from_maintenance_window(
         self, *, WindowId: str, WindowTargetId: str, Safe: bool = ...
     ) -> DeregisterTargetFromMaintenanceWindowResultTypeDef:
         """
         Removes a target from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_target_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_target_from_maintenance_window)
         """
+
     async def deregister_task_from_maintenance_window(
         self, *, WindowId: str, WindowTaskId: str
     ) -> DeregisterTaskFromMaintenanceWindowResultTypeDef:
         """
         Removes a task from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_task_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_task_from_maintenance_window)
         """
+
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeActivationsResultTypeDef:
@@ -812,28 +847,30 @@
         was created, its expiration date, the Identity and Access Management (IAM) role
         assigned to the managed nodes in the activation, and the number of nodes
         registered by using this activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_activations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_activations)
         """
+
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
         AssociationVersion: str = ...
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
+
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -841,41 +878,44 @@
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
+
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
+
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
+
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -884,37 +924,40 @@
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
+
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
+
     async def describe_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ...
     ) -> DescribeDocumentResultTypeDef:
         """
         Describes the specified Amazon Web Services Systems Manager document (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document)
         """
+
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
         NextToken: str = ...
@@ -922,67 +965,73 @@
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document_permission)
         """
+
     async def describe_effective_instance_associations(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectiveInstanceAssociationsResultTypeDef:
         """
         All associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_instance_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_instance_associations)
         """
+
     async def describe_effective_patches_for_patch_baseline(
         self, *, BaselineId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:
         """
         Retrieves the current effective patches (the patch and the approval state) for
         the specified patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_patches_for_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_patches_for_patch_baseline)
         """
+
     async def describe_instance_associations_status(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeInstanceAssociationsStatusResultTypeDef:
         """
         The status of the associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_associations_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_associations_status)
         """
+
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeInstanceInformationResultTypeDef:
         """
-        Describes one or more of your managed nodes, including information about the
-        operating system platform, the version of SSM Agent installed on the managed
-        node, node status, and so on.
+        Provides information about one or more of your managed nodes, including the
+        operating system platform, SSM Agent version, association status, and IP
+        address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_information)
         """
+
     async def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInstancePatchStatesResultTypeDef:
         """
         Retrieves the high-level patch state of one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states)
         """
+
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -990,14 +1039,15 @@
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states_for_patch_group)
         """
+
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1005,23 +1055,25 @@
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patches)
         """
+
     async def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_inventory_deletions)
         """
+
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -1030,177 +1082,190 @@
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_task_invocations)
         """
+
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
+
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
+
     async def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
+
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
+
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
+
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
+
     async def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows_for_target)
         """
+
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
+
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
+
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
+
     async def describe_patch_group_state(
         self, *, PatchGroup: str
     ) -> DescribePatchGroupStateResultTypeDef:
         """
         Returns high-level aggregated patch compliance state information for a patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_group_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_group_state)
         """
+
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
+
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
@@ -1209,14 +1274,15 @@
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_properties)
         """
+
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[SessionFilterTypeDef] = ...
@@ -1224,91 +1290,100 @@
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_sessions)
         """
+
     async def disassociate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationId: str
     ) -> Dict[str, Any]:
         """
         Deletes the association between an OpsItem and a related item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.disassociate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#disassociate_ops_item_related_item)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#generate_presigned_url)
         """
+
     async def get_automation_execution(
         self, *, AutomationExecutionId: str
     ) -> GetAutomationExecutionResultTypeDef:
         """
         Get detailed information about a particular Automation execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_automation_execution)
         """
+
     async def get_calendar_state(
         self, *, CalendarNames: Sequence[str], AtTime: str = ...
     ) -> GetCalendarStateResponseTypeDef:
         """
         Gets the state of a Amazon Web Services Systems Manager change calendar at the
         current time or a specified time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_calendar_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_calendar_state)
         """
+
     async def get_command_invocation(
         self, *, CommandId: str, InstanceId: str, PluginName: str = ...
     ) -> GetCommandInvocationResultTypeDef:
         """
         Returns detailed information about command execution for an invocation or
         plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_command_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_command_invocation)
         """
+
     async def get_connection_status(self, *, Target: str) -> GetConnectionStatusResponseTypeDef:
         """
         Retrieves the Session Manager connection status for a managed node to determine
         whether it is running and ready to receive Session Manager connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_connection_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_connection_status)
         """
+
     async def get_default_patch_baseline(
         self, *, OperatingSystem: OperatingSystemType = ...
     ) -> GetDefaultPatchBaselineResultTypeDef:
         """
         Retrieves the default patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_default_patch_baseline)
         """
+
     async def get_deployable_patch_snapshot_for_instance(
         self, *, InstanceId: str, SnapshotId: str, BaselineOverride: BaselineOverrideTypeDef = ...
     ) -> GetDeployablePatchSnapshotForInstanceResultTypeDef:
         """
         Retrieves the current snapshot for the patch baseline the managed node uses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_deployable_patch_snapshot_for_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_deployable_patch_snapshot_for_instance)
         """
+
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...
@@ -1316,14 +1391,15 @@
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_document)
         """
+
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
@@ -1331,14 +1407,15 @@
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
+
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
@@ -1347,76 +1424,84 @@
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory_schema)
         """
+
     async def get_maintenance_window(self, *, WindowId: str) -> GetMaintenanceWindowResultTypeDef:
         """
         Retrieves a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window)
         """
+
     async def get_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> GetMaintenanceWindowExecutionResultTypeDef:
         """
         Retrieves details about a specific a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution)
         """
+
     async def get_maintenance_window_execution_task(
         self, *, WindowExecutionId: str, TaskId: str
     ) -> GetMaintenanceWindowExecutionTaskResultTypeDef:
         """
         Retrieves the details about a specific task run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task)
         """
+
     async def get_maintenance_window_execution_task_invocation(
         self, *, WindowExecutionId: str, TaskId: str, InvocationId: str
     ) -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:
         """
         Retrieves information about a specific task running on a specific target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task_invocation)
         """
+
     async def get_maintenance_window_task(
         self, *, WindowId: str, WindowTaskId: str
     ) -> GetMaintenanceWindowTaskResultTypeDef:
         """
         Retrieves the details of a maintenance window task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_task)
         """
+
     async def get_ops_item(
         self, *, OpsItemId: str, OpsItemArn: str = ...
     ) -> GetOpsItemResponseTypeDef:
         """
         Get information about an OpsItem by using the ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_item)
         """
+
     async def get_ops_metadata(
         self, *, OpsMetadataArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetOpsMetadataResultTypeDef:
         """
         View operational metadata related to an application in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_metadata)
         """
+
     async def get_ops_summary(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
@@ -1426,42 +1511,46 @@
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
         """
+
     async def get_parameter(
         self, *, Name: str, WithDecryption: bool = ...
     ) -> GetParameterResultTypeDef:
         """
         Get information about a single parameter by specifying the parameter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter)
         """
+
     async def get_parameter_history(
         self, *, Name: str, WithDecryption: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> GetParameterHistoryResultTypeDef:
         """
         Retrieves the history of all changes to a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter_history)
         """
+
     async def get_parameters(
         self, *, Names: Sequence[str], WithDecryption: bool = ...
     ) -> GetParametersResultTypeDef:
         """
         Get information about one or more parameters by specifying multiple parameter
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters)
         """
+
     async def get_parameters_by_path(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
@@ -1470,79 +1559,87 @@
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
+
     async def get_patch_baseline(self, *, BaselineId: str) -> GetPatchBaselineResultTypeDef:
         """
         Retrieves information about a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline)
         """
+
     async def get_patch_baseline_for_patch_group(
         self, *, PatchGroup: str, OperatingSystem: OperatingSystemType = ...
     ) -> GetPatchBaselineForPatchGroupResultTypeDef:
         """
         Retrieves the patch baseline that should be used for the specified patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline_for_patch_group)
         """
+
     async def get_resource_policies(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Returns an array of the `Policy` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_resource_policies)
         """
+
     async def get_service_setting(self, *, SettingId: str) -> GetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_service_setting)
         """
+
     async def label_parameter_version(
         self, *, Name: str, Labels: Sequence[str], ParameterVersion: int = ...
     ) -> LabelParameterVersionResultTypeDef:
         """
         A parameter label is a user-defined alias to help you manage different versions
         of a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.label_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#label_parameter_version)
         """
+
     async def list_association_versions(
         self, *, AssociationId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationVersionsResultTypeDef:
         """
         Retrieves all versions of an association for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_association_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_association_versions)
         """
+
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_associations)
         """
+
     async def list_command_invocations(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1551,14 +1648,15 @@
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
+
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1566,14 +1664,15 @@
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
+
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -1582,28 +1681,30 @@
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_items)
         """
+
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_summaries)
         """
+
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
@@ -1612,23 +1713,25 @@
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
         """
+
     async def list_document_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDocumentVersionsResultTypeDef:
         """
         List all versions for a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_versions)
         """
+
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1636,14 +1739,15 @@
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_documents)
         """
+
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
@@ -1651,28 +1755,30 @@
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
+
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_events)
         """
+
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1680,59 +1786,64 @@
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
+
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying all
         Application Manager OpsMetadata objects or blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_metadata)
         """
+
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
+
     async def list_resource_data_sync(
         self, *, SyncType: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListResourceDataSyncResultTypeDef:
         """
         Lists your resource data sync configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_data_sync)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str
     ) -> ListTagsForResourceResultTypeDef:
         """
         Returns a list of the tags assigned to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_tags_for_resource)
         """
+
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
@@ -1741,41 +1852,44 @@
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
         """
+
     async def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
+        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
         """
+
     async def put_inventory(
         self, *, InstanceId: str, Items: Sequence[InventoryItemTypeDef]
     ) -> PutInventoryResultTypeDef:
         """
         Bulk update custom inventory items on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_inventory)
         """
+
     async def put_parameter(
         self,
         *,
         Name: str,
         Value: str,
         Description: str = ...,
         Type: ParameterTypeType = ...,
@@ -1789,186 +1903,197 @@
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
+
     async def put_resource_policy(
         self, *, ResourceArn: str, Policy: str, PolicyId: str = ..., PolicyHash: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_resource_policy)
         """
+
     async def register_default_patch_baseline(
         self, *, BaselineId: str
     ) -> RegisterDefaultPatchBaselineResultTypeDef:
         """
         Defines the default patch baseline for the relevant operating system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_default_patch_baseline)
         """
+
     async def register_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> RegisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Registers a patch baseline for a patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_patch_baseline_for_patch_group)
         """
+
     async def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
+
     async def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[
-            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
-        ] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
+        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
+
     async def remove_tags_from_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str, TagKeys: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Removes tag keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.remove_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#remove_tags_from_resource)
         """
+
     async def reset_service_setting(self, *, SettingId: str) -> ResetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.reset_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#reset_service_setting)
         """
+
     async def resume_session(self, *, SessionId: str) -> ResumeSessionResponseTypeDef:
         """
         Reconnects a session to a managed node after it has been disconnected.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.resume_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#resume_session)
         """
+
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
         Payload: Mapping[str, Sequence[str]] = ...
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_automation_signal)
         """
+
     async def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigUnionTypeDef = ...,
+        NotificationConfig: NotificationConfigTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
+
     async def start_associations_once(self, *, AssociationIds: Sequence[str]) -> Dict[str, Any]:
         """
         Runs an association immediately and only one time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_associations_once)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_associations_once)
         """
+
     async def start_automation_execution(
         self,
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
+
     async def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookUnionTypeDef],
+        Runbooks: Sequence[RunbookTypeDef],
         ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -1977,14 +2102,15 @@
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
+
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...
@@ -1992,80 +2118,86 @@
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_session)
         """
+
     async def stop_automation_execution(
         self, *, AutomationExecutionId: str, Type: StopTypeType = ...
     ) -> Dict[str, Any]:
         """
         Stop an Automation that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.stop_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#stop_automation_execution)
         """
+
     async def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
         """
         Permanently ends a session and closes the data connection between the Session
         Manager client and SSM Agent on the managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.terminate_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#terminate_session)
         """
+
     async def unlabel_parameter_version(
         self, *, Name: str, ParameterVersion: int, Labels: Sequence[str]
     ) -> UnlabelParameterVersionResultTypeDef:
         """
         Remove a label or labels from a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.unlabel_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#unlabel_parameter_version)
         """
+
     async def update_association(
         self,
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
+
     async def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association_status)
         """
+
     async def update_document(
         self,
         *,
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
@@ -2076,33 +2208,36 @@
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
+
     async def update_document_default_version(
         self, *, Name: str, DocumentVersion: str
     ) -> UpdateDocumentDefaultVersionResultTypeDef:
         """
         Set the default version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_default_version)
         """
+
     async def update_document_metadata(
         self, *, Name: str, DocumentReviews: DocumentReviewsTypeDef, DocumentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates information related to approval reviews for a specific version of a
         change template in Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_metadata)
         """
+
     async def update_maintenance_window(
         self,
         *,
         WindowId: str,
         Name: str = ...,
         Description: str = ...,
         StartDate: str = ...,
@@ -2118,69 +2253,71 @@
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
+
     async def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
+
     async def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[
-            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
-        ] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
+        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
+
     async def update_managed_instance_role(
         self, *, InstanceId: str, IamRole: str
     ) -> Dict[str, Any]:
         """
         Changes the Identity and Access Management (IAM) role that is assigned to the
         on-premises server, edge device, or virtual machines (VM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_managed_instance_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_managed_instance_role)
         """
+
     async def update_ops_item(
         self,
         *,
         OpsItemId: str,
         Description: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         OperationalDataToDelete: Sequence[str] = ...,
@@ -2199,442 +2336,496 @@
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
+
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
         KeysToDelete: Sequence[str] = ...
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_metadata)
         """
+
     async def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
-        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
+        GlobalFilters: PatchFilterGroupTypeDef = ...,
+        ApprovalRules: PatchRuleGroupTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
+        Sources: Sequence[PatchSourceTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
+
     async def update_resource_data_sync(
         self, *, SyncName: str, SyncType: str, SyncSource: ResourceDataSyncSourceTypeDef
     ) -> Dict[str, Any]:
         """
         Update a resource data sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_resource_data_sync)
         """
+
     async def update_service_setting(self, *, SettingId: str, SettingValue: str) -> Dict[str, Any]:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_service_setting)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_activations"]
     ) -> DescribeActivationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_execution_targets"]
     ) -> DescribeAssociationExecutionTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_executions"]
     ) -> DescribeAssociationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_executions"]
     ) -> DescribeAutomationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_step_executions"]
     ) -> DescribeAutomationStepExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_available_patches"]
     ) -> DescribeAvailablePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_instance_associations"]
     ) -> DescribeEffectiveInstanceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_patches_for_patch_baseline"]
     ) -> DescribeEffectivePatchesForPatchBaselinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_associations_status"]
     ) -> DescribeInstanceAssociationsStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_information"]
     ) -> DescribeInstanceInformationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states"]
     ) -> DescribeInstancePatchStatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states_for_patch_group"]
     ) -> DescribeInstancePatchStatesForPatchGroupPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patches"]
     ) -> DescribeInstancePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_task_invocations"]
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_tasks"]
     ) -> DescribeMaintenanceWindowExecutionTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_executions"]
     ) -> DescribeMaintenanceWindowExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_schedule"]
     ) -> DescribeMaintenanceWindowSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_targets"]
     ) -> DescribeMaintenanceWindowTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_tasks"]
     ) -> DescribeMaintenanceWindowTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows"]
     ) -> DescribeMaintenanceWindowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows_for_target"]
     ) -> DescribeMaintenanceWindowsForTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_ops_items"]
     ) -> DescribeOpsItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_parameters"]
     ) -> DescribeParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_baselines"]
     ) -> DescribePatchBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_groups"]
     ) -> DescribePatchGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_properties"]
     ) -> DescribePatchPropertiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_sessions"]
     ) -> DescribeSessionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_inventory"]) -> GetInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_inventory_schema"]
     ) -> GetInventorySchemaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_ops_summary"]) -> GetOpsSummaryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameter_history"]
     ) -> GetParameterHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameters_by_path"]
     ) -> GetParametersByPathPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_association_versions"]
     ) -> ListAssociationVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations"]
     ) -> ListAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_command_invocations"]
     ) -> ListCommandInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_commands"]) -> ListCommandsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_items"]
     ) -> ListComplianceItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_summaries"]
     ) -> ListComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_versions"]
     ) -> ListDocumentVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_documents"]) -> ListDocumentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_events"]
     ) -> ListOpsItemEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_related_items"]
     ) -> ListOpsItemRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_metadata"]
     ) -> ListOpsMetadataPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_compliance_summaries"]
     ) -> ListResourceComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_data_sync"]
     ) -> ListResourceDataSyncPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     def get_waiter(self, waiter_name: Literal["command_executed"]) -> CommandExecutedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "SSMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,14 +530,15 @@
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
@@ -633,14 +634,15 @@
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
@@ -719,26 +721,28 @@
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
@@ -949,14 +953,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,15 @@
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
@@ -631,14 +632,15 @@
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
@@ -717,26 +719,28 @@
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
@@ -947,14 +951,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -574,15 +574,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -650,15 +650,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -554,15 +554,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetUnionTypeDef] = ...,
+        Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
@@ -626,15 +626,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetUnionTypeDef],
+        Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_ssm.type_defs import AccountSharingInfoTypeDef
 
     data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Mapping, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -101,50 +99,47 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusOutputTypeDef",
-    "TargetOutputTypeDef",
+    "AssociationStatusTypeDef",
+    "TargetTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
-    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
-    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigOutputTypeDef",
-    "ComplianceExecutionSummaryOutputTypeDef",
+    "NotificationConfigTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "TargetTypeDef",
+    "TimestampTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
@@ -212,29 +207,28 @@
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -248,25 +242,21 @@
     "ListDocumentVersionsRequestRequestTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
-    "MaintenanceWindowLambdaParametersOutputTypeDef",
-    "NotificationConfigTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
     "ParameterInlinePolicyTypeDef",
-    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
@@ -283,15 +273,14 @@
     "UpdateMaintenanceWindowRequestRequestTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
     "PutParameterRequestRequestTypeDef",
-    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "AssociateOpsItemRelatedItemResponseTypeDef",
     "CancelMaintenanceWindowExecutionResultTypeDef",
     "CreateActivationResultTypeDef",
     "CreateMaintenanceWindowResultTypeDef",
     "CreateOpsItemResponseTypeDef",
     "CreateOpsMetadataResultTypeDef",
@@ -327,39 +316,40 @@
     "StartAutomationExecutionResultTypeDef",
     "StartChangeRequestExecutionResultTypeDef",
     "StartSessionResponseTypeDef",
     "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionResultTypeDef",
     "UpdateMaintenanceWindowResultTypeDef",
     "UpdateOpsMetadataResultTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
     "AssociationTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
     "ListAssociationsRequestRequestTypeDef",
-    "AssociationStatusTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersOutputTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
     "ComplianceItemTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
-    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
@@ -372,14 +362,15 @@
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
@@ -391,14 +382,16 @@
     "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -450,15 +443,14 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
-    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -468,56 +460,39 @@
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
-    "NotificationConfigUnionTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
-    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
-    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
-    "TargetLocationOutputTypeDef",
-    "AlarmConfigurationUnionTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
-    "AssociationStatusUnionTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
-    "ComplianceExecutionSummaryUnionTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "SendCommandRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -527,80 +502,69 @@
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
-    "PatchRuleOutputTypeDef",
-    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
+    "ResourceDataSyncSourceWithStateTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
-    "CreateAssociationBatchRequestEntryOutputTypeDef",
-    "RunbookOutputTypeDef",
-    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "TargetLocationUnionTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "StepExecutionTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
-    "CreateAssociationBatchRequestEntryUnionTypeDef",
-    "RunbookUnionTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "PatchRuleGroupUnionTypeDef",
+    "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -659,42 +623,40 @@
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusOutputTypeDef = TypedDict(
-    "_RequiredAssociationStatusOutputTypeDef",
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusOutputTypeDef = TypedDict(
-    "_OptionalAssociationStatusOutputTypeDef",
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-
-class AssociationStatusOutputTypeDef(
-    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
 ):
     pass
 
-
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
         "Key": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -725,15 +687,14 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -794,36 +755,33 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
-
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
@@ -859,47 +817,44 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigOutputTypeDef = TypedDict(
-    "NotificationConfigOutputTypeDef",
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryOutputTypeDef",
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
     {
         "ExecutionTime": datetime,
     },
 )
-_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryOutputTypeDef",
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-
-class ComplianceExecutionSummaryOutputTypeDef(
-    _RequiredComplianceExecutionSummaryOutputTypeDef,
-    _OptionalComplianceExecutionSummaryOutputTypeDef,
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
 ):
     pass
 
-
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -909,21 +864,19 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
-
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -947,23 +900,15 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
-    {
-        "Key": str,
-        "Values": Sequence[str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDocumentRequiresTypeDef = TypedDict(
@@ -972,19 +917,17 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -1042,21 +985,19 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1065,21 +1006,19 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
@@ -1121,22 +1060,20 @@
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
-
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1168,22 +1105,20 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
-
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -1277,22 +1212,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1300,21 +1233,19 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1322,22 +1253,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
@@ -1356,22 +1285,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1379,22 +1306,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1446,21 +1371,19 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
-
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1468,22 +1391,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1495,21 +1416,19 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
-
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1615,21 +1534,19 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
-
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1666,22 +1583,20 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1805,21 +1720,19 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
-
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1836,22 +1749,20 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
-
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
@@ -1875,21 +1786,19 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
-
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -1897,19 +1806,17 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -1945,16 +1852,16 @@
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
@@ -1983,40 +1890,36 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
-
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2024,21 +1927,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2046,19 +1947,17 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
-
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
-
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -2074,43 +1973,39 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
-
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2133,59 +2028,46 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2193,22 +2075,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2294,19 +2174,17 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
-
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
-
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2316,21 +2194,19 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
-
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
-
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2338,22 +2214,20 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
-
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2361,22 +2235,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2386,22 +2258,20 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2409,22 +2279,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2473,69 +2341,42 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
-MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowAutomationParametersOutputTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
+        "Parameters": Dict[str, List[str]],
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersOutputTypeDef",
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
-    {
-        "NotificationArn": str,
-        "NotificationEvents": Sequence[NotificationEventType],
-        "NotificationType": NotificationTypeType,
-    },
-    total=False,
-)
-
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
-    {
-        "Values": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2545,22 +2386,20 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2580,22 +2419,14 @@
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterOutputTypeDef = TypedDict(
-    "PatchFilterOutputTypeDef",
-    {
-        "Key": PatchFilterKeyType,
-        "Values": List[str],
-    },
-)
-
 PatchFilterTypeDef = TypedDict(
     "PatchFilterTypeDef",
     {
         "Key": PatchFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -2612,21 +2443,19 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
@@ -2688,22 +2517,20 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
-
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -2728,43 +2555,39 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
-
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -2806,22 +2629,20 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
@@ -2880,22 +2701,20 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2911,63 +2730,38 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
-
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAlarmConfigurationOutputTypeDef",
-    {
-        "Alarms": List[AlarmTypeDef],
-    },
-)
-_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAlarmConfigurationOutputTypeDef",
-    {
-        "IgnorePollAlarmFailure": bool,
-    },
-    total=False,
-)
-
-
-class AlarmConfigurationOutputTypeDef(
-    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationTypeDef = TypedDict(
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
-
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-
 AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
     "AssociateOpsItemRelatedItemResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3380,53 +3174,134 @@
     "UpdateOpsMetadataResultTypeDef",
     {
         "OpsMetadataArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
         "DocumentVersion": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "LastExecutionDate": datetime,
         "Overview": AssociationOverviewTypeDef,
         "ScheduleExpression": str,
         "AssociationName": str,
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
 MaintenanceWindowTargetTypeDef = TypedDict(
     "MaintenanceWindowTargetTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
         "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3442,22 +3317,20 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3483,77 +3356,30 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Name": AssociationStatusNameType,
-        "Message": str,
-    },
-)
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
-    {
-        "AdditionalInfo": str,
-    },
-    total=False,
-)
-
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
-):
-    pass
-
-
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionTime": TimestampTypeDef,
-    },
-)
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionId": str,
-        "ExecutionType": str,
-    },
-    total=False,
-)
-
-
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
-):
-    pass
-
-
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3566,41 +3392,29 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
-    {
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": BlobTypeDef,
-    },
-    total=False,
-)
-
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "Comment": str,
         "DocumentName": str,
@@ -3659,29 +3473,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersOutputTypeDef",
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
     {
         "Comment": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3693,20 +3507,45 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
@@ -3768,22 +3607,19 @@
         "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3798,21 +3634,19 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -3899,21 +3733,19 @@
         "PlannedStartTime": TimestampTypeDef,
         "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -3963,21 +3795,19 @@
         "PlannedStartTime": TimestampTypeDef,
         "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -3985,21 +3815,19 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4017,21 +3845,19 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 DescribeActivationsRequestRequestTypeDef = TypedDict(
     "DescribeActivationsRequestRequestTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -4059,22 +3885,20 @@
     {
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
         {
             "AssociationId": str,
         },
     )
@@ -4086,22 +3910,20 @@
             "Filters": Sequence[AssociationExecutionFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
-
 class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
 ):
     pass
 
-
 DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4117,97 +3939,110 @@
     "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
 ):
     pass
 
-
 DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     {
         "DeletionId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -4216,22 +4051,20 @@
     {
         "PatchSet": PatchSetType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
     _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
 ):
     pass
 
-
 GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     {
         "TypeName": str,
         "Aggregator": bool,
         "SubType": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4250,66 +4083,60 @@
     {
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
     _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
     _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4368,22 +4195,20 @@
     "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
     _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4410,22 +4235,20 @@
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4435,22 +4258,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4477,22 +4298,20 @@
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4501,21 +4320,46 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4601,22 +4445,20 @@
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4625,22 +4467,20 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4676,22 +4516,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4701,22 +4539,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
@@ -4724,22 +4560,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4748,22 +4582,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
@@ -4771,22 +4603,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4795,22 +4625,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
@@ -4818,22 +4646,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4842,22 +4668,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
@@ -4865,22 +4689,20 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4889,22 +4711,20 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4999,22 +4819,20 @@
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -5025,22 +4843,20 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5087,22 +4903,20 @@
     {
         "Filters": Sequence[SessionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -5111,21 +4925,19 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5210,19 +5022,17 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
-
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
-
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5249,22 +5059,20 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
-
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5282,22 +5090,20 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -5377,15 +5183,14 @@
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5473,21 +5278,19 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
-
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5565,37 +5368,14 @@
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
-    {
-        "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ServiceRoleArn": str,
-        "TimeoutSeconds": int,
-    },
-    total=False,
-)
-
-NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
-MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5665,72 +5445,41 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
-PatchFilterGroupOutputTypeDef = TypedDict(
-    "PatchFilterGroupOutputTypeDef",
-    {
-        "PatchFilters": List[PatchFilterOutputTypeDef],
-    },
-)
-
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
-_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
-    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
-    {
-        "OrganizationSourceType": str,
-    },
-)
-_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
-    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
-    {
-        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
-    },
-    total=False,
-)
-
-
-class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
-    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-):
-    pass
-
-
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
-
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
-
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5741,21 +5490,19 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
-
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5786,15 +5533,15 @@
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5802,56 +5549,54 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[
-            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
-        ],
+        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
@@ -5860,56 +5605,77 @@
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetOutputTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "Targets": List[TargetTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
         "Priority": int,
         "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-TargetLocationOutputTypeDef = TypedDict(
-    "TargetLocationOutputTypeDef",
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
     {
-        "Accounts": List[str],
-        "Regions": List[str],
-        "TargetLocationMaxConcurrency": str,
-        "TargetLocationMaxErrors": str,
-        "ExecutionRoleName": str,
-        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5942,70 +5708,30 @@
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
-    {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
-    },
-)
-
-ComplianceExecutionSummaryUnionTypeDef = Union[
-    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
-]
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
-
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
         "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
@@ -6029,186 +5755,21 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[TargetUnionTypeDef],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetUnionTypeDef],
-    },
-)
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetUnionTypeDef],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-    },
-    total=False,
-)
-
-
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
-
-
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6283,22 +5844,20 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6380,25 +5939,14 @@
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
-    {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
-    },
-    total=False,
-)
-
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6436,37 +5984,14 @@
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPatchRuleOutputTypeDef = TypedDict(
-    "_RequiredPatchRuleOutputTypeDef",
-    {
-        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
-    },
-)
-_OptionalPatchRuleOutputTypeDef = TypedDict(
-    "_OptionalPatchRuleOutputTypeDef",
-    {
-        "ComplianceLevel": PatchComplianceLevelType,
-        "ApproveAfterDays": int,
-        "ApproveUntilDate": str,
-        "EnableNonSecurity": bool,
-    },
-    total=False,
-)
-
-
-class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
-    pass
-
-
-PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6476,32 +6001,17 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
-
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
-
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
-
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
 )
@@ -6511,20 +6021,31 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
-
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
 
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6579,131 +6100,195 @@
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusOutputTypeDef,
+        "Status": AssociationStatusTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
+_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
+_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
     {
         "InstanceId": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class CreateAssociationBatchRequestEntryOutputTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
+class CreateAssociationBatchRequestEntryTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
 
-_RequiredRunbookOutputTypeDef = TypedDict(
-    "_RequiredRunbookOutputTypeDef",
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+):
+    pass
+
+_RequiredRunbookTypeDef = TypedDict(
+    "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalRunbookOutputTypeDef = TypedDict(
-    "_OptionalRunbookOutputTypeDef",
+_OptionalRunbookTypeDef = TypedDict(
+    "_OptionalRunbookTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
     },
     total=False,
 )
 
-
-class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
+class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ClientToken": str,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
+):
+    pass
 
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
@@ -6720,128 +6305,167 @@
         "FailureDetails": FailureDetailsTypeDef,
         "StepExecutionId": str,
         "OverriddenParameters": Dict[str, List[str]],
         "IsEnd": bool,
         "NextStep": str,
         "IsCritical": bool,
         "ValidNextSteps": List[str],
-        "Targets": List[TargetOutputTypeDef],
-        "TargetLocation": TargetLocationOutputTypeDef,
+        "Targets": List[TargetTypeDef],
+        "TargetLocation": TargetLocationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
     {
-        "Name": str,
+        "AssociationId": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
     {
-        "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetTypeDef],
         "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class CreateAssociationBatchRequestEntryTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryTypeDef,
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
 ):
     pass
 
+GetMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "GetMaintenanceWindowTaskResultTypeDef",
+    {
+        "WindowId": str,
+        "WindowTaskId": str,
+        "Targets": List[TargetTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredRunbookTypeDef = TypedDict(
-    "_RequiredRunbookTypeDef",
+_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "DocumentName": str,
+        "WindowId": str,
+        "TaskArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
     },
 )
-_OptionalRunbookTypeDef = TypedDict(
-    "_OptionalRunbookTypeDef",
+_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "TargetParameterName": str,
         "Targets": Sequence[TargetTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
+class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+):
     pass
 
-
-TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
-GetMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "GetMaintenanceWindowTaskResultTypeDef",
+_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetOutputTypeDef],
+    },
+)
+_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
+        "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
+    total=False,
 )
 
+class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+):
+    pass
+
 UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
@@ -6886,121 +6510,21 @@
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
-]
-_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "TaskArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-    },
-)
-_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-):
-    pass
-
-
-PatchRuleGroupOutputTypeDef = TypedDict(
-    "PatchRuleGroupOutputTypeDef",
-    {
-        "PatchRules": List[PatchRuleOutputTypeDef],
-    },
-)
-
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -7009,31 +6533,46 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
-
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
+    {
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
+    },
+    total=False,
+)
+
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7067,18 +6606,25 @@
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+    },
+)
+
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -7095,33 +6641,62 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookOutputTypeDef],
+        "Runbooks": List[RunbookTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -7134,27 +6709,27 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookOutputTypeDef],
+        "Runbooks": List[RunbookTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
@@ -7163,172 +6738,14 @@
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestEntryUnionTypeDef = Union[
-    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
-]
-RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
-    {
-        "Parameters": Mapping[str, Sequence[str]],
-        "DocumentVersion": str,
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
-):
-    pass
-
-
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupOutputTypeDef,
-        "ApprovalRules": PatchRuleGroupOutputTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupOutputTypeDef,
-        "ApprovalRules": PatchRuleGroupOutputTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "GlobalFilters": PatchFilterGroupTypeDef,
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
@@ -7355,30 +6772,49 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceUnionTypeDef],
+        "Sources": Sequence[PatchSourceTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupTypeDef,
+        "ApprovalRules": PatchRuleGroupTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7389,27 +6825,46 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceUnionTypeDef],
+        "Sources": Sequence[PatchSourceTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupTypeDef,
+        "ApprovalRules": PatchRuleGroupTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -7438,52 +6893,14 @@
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
-    },
-)
-
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookUnionTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": TimestampTypeDef,
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": TimestampTypeDef,
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
 )
@@ -7491,13 +6908,12 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
-
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_ssm.type_defs import AccountSharingInfoTypeDef
 
     data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Mapping, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -101,49 +99,48 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusOutputTypeDef",
-    "TargetOutputTypeDef",
+    "AssociationStatusTypeDef",
+    "TargetTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
-    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
-    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigOutputTypeDef",
-    "ComplianceExecutionSummaryOutputTypeDef",
+    "NotificationConfigTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "TargetTypeDef",
+    "TimestampTypeDef",
     "DocumentRequiresTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
     "MetadataValueTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
@@ -211,29 +208,28 @@
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
@@ -247,25 +243,21 @@
     "ListDocumentVersionsRequestRequestTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
-    "MaintenanceWindowLambdaParametersOutputTypeDef",
-    "NotificationConfigTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
     "ParameterInlinePolicyTypeDef",
-    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
@@ -282,15 +274,14 @@
     "UpdateMaintenanceWindowRequestRequestTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
     "PutParameterRequestRequestTypeDef",
-    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
     "AssociateOpsItemRelatedItemResponseTypeDef",
     "CancelMaintenanceWindowExecutionResultTypeDef",
     "CreateActivationResultTypeDef",
     "CreateMaintenanceWindowResultTypeDef",
     "CreateOpsItemResponseTypeDef",
     "CreateOpsMetadataResultTypeDef",
@@ -326,39 +317,40 @@
     "StartAutomationExecutionResultTypeDef",
     "StartChangeRequestExecutionResultTypeDef",
     "StartSessionResponseTypeDef",
     "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionResultTypeDef",
     "UpdateMaintenanceWindowResultTypeDef",
     "UpdateOpsMetadataResultTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
     "AssociationTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
     "ListAssociationsRequestRequestTypeDef",
-    "AssociationStatusTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersOutputTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
     "ComplianceItemTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
-    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
@@ -371,14 +363,15 @@
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
@@ -390,14 +383,16 @@
     "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -449,15 +444,14 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
-    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -467,56 +461,39 @@
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
-    "NotificationConfigUnionTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
-    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
-    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
-    "TargetLocationOutputTypeDef",
-    "AlarmConfigurationUnionTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
-    "AssociationStatusUnionTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
-    "ComplianceExecutionSummaryUnionTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "SendCommandRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -526,80 +503,69 @@
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
-    "PatchRuleOutputTypeDef",
-    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
+    "ResourceDataSyncSourceWithStateTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
-    "CreateAssociationBatchRequestEntryOutputTypeDef",
-    "RunbookOutputTypeDef",
-    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "TargetLocationUnionTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "StepExecutionTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
-    "CreateAssociationBatchRequestEntryUnionTypeDef",
-    "RunbookUnionTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "PatchRuleGroupUnionTypeDef",
+    "GetPatchBaselineResultTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -658,40 +624,42 @@
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusOutputTypeDef = TypedDict(
-    "_RequiredAssociationStatusOutputTypeDef",
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusOutputTypeDef = TypedDict(
-    "_OptionalAssociationStatusOutputTypeDef",
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-class AssociationStatusOutputTypeDef(
-    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
 ):
     pass
 
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
+
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
         "Key": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -722,15 +690,14 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -791,34 +758,35 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
+
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
@@ -854,45 +822,46 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigOutputTypeDef = TypedDict(
-    "NotificationConfigOutputTypeDef",
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryOutputTypeDef",
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
     {
         "ExecutionTime": datetime,
     },
 )
-_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryOutputTypeDef",
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-class ComplianceExecutionSummaryOutputTypeDef(
-    _RequiredComplianceExecutionSummaryOutputTypeDef,
-    _OptionalComplianceExecutionSummaryOutputTypeDef,
+
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
 ):
     pass
 
+
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -902,19 +871,21 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
+
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -938,23 +909,15 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
-    {
-        "Key": str,
-        "Values": Sequence[str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDocumentRequiresTypeDef = TypedDict(
@@ -963,17 +926,19 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
+
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -1031,19 +996,21 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1052,19 +1019,21 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
@@ -1106,20 +1075,22 @@
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
+
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1151,20 +1122,22 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
+
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -1258,20 +1231,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1279,19 +1254,21 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1299,20 +1276,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
@@ -1331,20 +1310,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1352,20 +1333,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1417,19 +1400,21 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
+
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1437,20 +1422,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1462,19 +1449,21 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
+
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
+
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1580,19 +1569,21 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
+
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1629,20 +1620,22 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
+
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1766,19 +1759,21 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
+
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1795,20 +1790,22 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
+
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
@@ -1832,19 +1829,21 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
+
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -1852,17 +1851,19 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -1898,16 +1899,16 @@
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
@@ -1936,36 +1937,40 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
+
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -1973,19 +1978,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -1993,17 +2000,19 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
+
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
+
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
@@ -2019,39 +2028,43 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2074,55 +2087,50 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-PatchSourceOutputTypeDef = TypedDict(
-    "PatchSourceOutputTypeDef",
-    {
-        "Name": str,
-        "Products": List[str],
-        "Configuration": str,
-    },
-)
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2130,20 +2138,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2229,17 +2239,19 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
+
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
+
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2249,19 +2261,21 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
+
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
+
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2269,20 +2283,22 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
+
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2290,20 +2306,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2313,20 +2331,22 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2334,20 +2354,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2396,69 +2418,42 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
-MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowAutomationParametersOutputTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
-    },
-    total=False,
-)
-
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
+        "Parameters": Dict[str, List[str]],
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersOutputTypeDef",
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
-    {
-        "NotificationArn": str,
-        "NotificationEvents": Sequence[NotificationEventType],
-        "NotificationType": NotificationTypeType,
-    },
-    total=False,
-)
-
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
-    {
-        "Values": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2468,20 +2463,22 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2501,22 +2498,14 @@
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterOutputTypeDef = TypedDict(
-    "PatchFilterOutputTypeDef",
-    {
-        "Key": PatchFilterKeyType,
-        "Values": List[str],
-    },
-)
-
 PatchFilterTypeDef = TypedDict(
     "PatchFilterTypeDef",
     {
         "Key": PatchFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -2533,19 +2522,21 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
@@ -2607,20 +2598,22 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
+
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -2645,39 +2638,43 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
+
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -2719,20 +2716,22 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
@@ -2791,20 +2790,22 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2820,37 +2821,20 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
+
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
-_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAlarmConfigurationOutputTypeDef",
-    {
-        "Alarms": List[AlarmTypeDef],
-    },
-)
-_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAlarmConfigurationOutputTypeDef",
-    {
-        "IgnorePollAlarmFailure": bool,
-    },
-    total=False,
-)
-
-class AlarmConfigurationOutputTypeDef(
-    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
-):
-    pass
 
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
@@ -2858,19 +2842,21 @@
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
+
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
+
 AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
     "AssociateOpsItemRelatedItemResponseTypeDef",
     {
         "AssociationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3283,53 +3269,140 @@
     "UpdateOpsMetadataResultTypeDef",
     {
         "OpsMetadataArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
         "DocumentVersion": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "LastExecutionDate": datetime,
         "Overview": AssociationOverviewTypeDef,
         "ScheduleExpression": str,
         "AssociationName": str,
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+
 MaintenanceWindowTargetTypeDef = TypedDict(
     "MaintenanceWindowTargetTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
         "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3345,20 +3418,22 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3384,71 +3459,32 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Name": AssociationStatusNameType,
-        "Message": str,
-    },
-)
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
-    {
-        "AdditionalInfo": str,
-    },
-    total=False,
-)
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
-):
-    pass
-
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionTime": TimestampTypeDef,
-    },
-)
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
-    {
-        "ExecutionId": str,
-        "ExecutionType": str,
-    },
-    total=False,
-)
-
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
-):
-    pass
-
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3461,39 +3497,31 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
-    {
-        "ClientContext": str,
-        "Qualifier": str,
-        "Payload": BlobTypeDef,
-    },
-    total=False,
-)
-
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "Comment": str,
         "DocumentName": str,
@@ -3552,29 +3580,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersOutputTypeDef",
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
     {
         "Comment": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3586,20 +3614,47 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
+
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
@@ -3661,20 +3716,21 @@
         "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
+
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3689,19 +3745,21 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -3788,19 +3846,21 @@
         "PlannedStartTime": TimestampTypeDef,
         "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -3850,19 +3910,21 @@
         "PlannedStartTime": TimestampTypeDef,
         "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -3870,19 +3932,21 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3900,19 +3964,21 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 DescribeActivationsRequestRequestTypeDef = TypedDict(
     "DescribeActivationsRequestRequestTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3940,20 +4006,22 @@
     {
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
         {
             "AssociationId": str,
         },
     )
@@ -3965,20 +4033,22 @@
             "Filters": Sequence[AssociationExecutionFilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
+
 class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
     _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
 ):
     pass
 
+
 DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -3994,89 +4064,120 @@
     "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
     "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
 ):
     pass
 
+
 DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     {
         "DeletionId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -4085,20 +4186,22 @@
     {
         "PatchSet": PatchSetType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
     _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
 ):
     pass
 
+
 GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
     "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     {
         "TypeName": str,
         "Aggregator": bool,
         "SubType": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4117,60 +4220,66 @@
     {
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
     _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
     "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
     _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
     "ListAssociationsRequestListAssociationsPaginateTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4229,20 +4338,22 @@
     "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
     _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4269,20 +4380,22 @@
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4292,20 +4405,22 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4332,20 +4447,22 @@
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4354,20 +4471,49 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4452,20 +4598,22 @@
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4474,20 +4622,22 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4523,20 +4673,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4546,20 +4698,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
@@ -4567,20 +4721,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4589,20 +4745,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
@@ -4610,20 +4768,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4632,20 +4792,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
@@ -4653,20 +4815,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4675,20 +4839,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
@@ -4696,20 +4862,22 @@
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4718,20 +4886,22 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -4826,20 +4996,22 @@
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -4850,20 +5022,22 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4910,20 +5084,22 @@
     {
         "Filters": Sequence[SessionFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -4932,19 +5108,21 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5029,17 +5207,19 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
+
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
+
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5066,20 +5246,22 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
+
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5097,20 +5279,22 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -5190,15 +5374,14 @@
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5286,19 +5469,21 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
+
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5376,37 +5561,14 @@
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
-    {
-        "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ServiceRoleArn": str,
-        "TimeoutSeconds": int,
-    },
-    total=False,
-)
-
-NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
-MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
-]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5476,68 +5638,43 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
-PatchFilterGroupOutputTypeDef = TypedDict(
-    "PatchFilterGroupOutputTypeDef",
-    {
-        "PatchFilters": List[PatchFilterOutputTypeDef],
-    },
-)
-
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
-_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
-    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
-    {
-        "OrganizationSourceType": str,
-    },
-)
-_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
-    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
-    {
-        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
-    },
-    total=False,
-)
-
-class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
-    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-):
-    pass
-
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
+
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
+
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5548,19 +5685,21 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
+
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5591,15 +5730,15 @@
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5607,56 +5746,54 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigOutputTypeDef,
+        "NotificationConfig": NotificationConfigTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[
-            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
-        ],
+        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
@@ -5665,56 +5802,79 @@
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetOutputTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "Targets": List[TargetTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
         "Priority": int,
         "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-TargetLocationOutputTypeDef = TypedDict(
-    "TargetLocationOutputTypeDef",
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
     {
-        "Accounts": List[str],
-        "Regions": List[str],
-        "TargetLocationMaxConcurrency": str,
-        "TargetLocationMaxErrors": str,
-        "ExecutionRoleName": str,
-        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
+
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
+
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5747,68 +5907,30 @@
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
-    {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
-    },
-)
-
-ComplianceExecutionSummaryUnionTypeDef = Union[
-    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
-]
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
         "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
@@ -5832,176 +5954,21 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[TargetUnionTypeDef],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetUnionTypeDef],
-    },
-)
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetUnionTypeDef],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-    },
-    total=False,
-)
-
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
-
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6076,20 +6043,22 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6171,25 +6140,14 @@
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
-    {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
-    },
-    total=False,
-)
-
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6227,35 +6185,14 @@
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPatchRuleOutputTypeDef = TypedDict(
-    "_RequiredPatchRuleOutputTypeDef",
-    {
-        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
-    },
-)
-_OptionalPatchRuleOutputTypeDef = TypedDict(
-    "_OptionalPatchRuleOutputTypeDef",
-    {
-        "ComplianceLevel": PatchComplianceLevelType,
-        "ApproveAfterDays": int,
-        "ApproveUntilDate": str,
-        "EnableNonSecurity": bool,
-    },
-    total=False,
-)
-
-class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
-    pass
-
-PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6265,29 +6202,18 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
+
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
 
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
@@ -6298,19 +6224,34 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
+
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
+
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
+
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6364,128 +6305,204 @@
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusOutputTypeDef,
+        "Status": AssociationStatusTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
+_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
+_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
     {
         "InstanceId": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAssociationBatchRequestEntryTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryTypeDef,
+):
+    pass
+
+
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateAssociationBatchRequestEntryOutputTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
+
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
 ):
     pass
 
-_RequiredRunbookOutputTypeDef = TypedDict(
-    "_RequiredRunbookOutputTypeDef",
+
+_RequiredRunbookTypeDef = TypedDict(
+    "_RequiredRunbookTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalRunbookOutputTypeDef = TypedDict(
-    "_OptionalRunbookOutputTypeDef",
+_OptionalRunbookTypeDef = TypedDict(
+    "_OptionalRunbookTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
     },
     total=False,
 )
 
-class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
+
+class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
+
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ClientToken": str,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
+):
+    pass
+
+
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
         "OnFailure": str,
@@ -6501,124 +6518,173 @@
         "FailureDetails": FailureDetailsTypeDef,
         "StepExecutionId": str,
         "OverriddenParameters": Dict[str, List[str]],
         "IsEnd": bool,
         "NextStep": str,
         "IsCritical": bool,
         "ValidNextSteps": List[str],
-        "Targets": List[TargetOutputTypeDef],
-        "TargetLocation": TargetLocationOutputTypeDef,
+        "Targets": List[TargetTypeDef],
+        "TargetLocation": TargetLocationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
     {
-        "Name": str,
+        "AssociationId": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
     {
-        "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
-        "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetTypeDef],
         "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateAssociationBatchRequestEntryTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryTypeDef,
+
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
 ):
     pass
 
-_RequiredRunbookTypeDef = TypedDict(
-    "_RequiredRunbookTypeDef",
+
+GetMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "GetMaintenanceWindowTaskResultTypeDef",
     {
-        "DocumentName": str,
+        "WindowId": str,
+        "WindowTaskId": str,
+        "Targets": List[TargetTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRunbookTypeDef = TypedDict(
-    "_OptionalRunbookTypeDef",
+
+_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "TaskArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+    },
+)
+_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "TargetParameterName": str,
         "Targets": Sequence[TargetTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
+
+class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+):
     pass
 
-TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
-GetMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "GetMaintenanceWindowTaskResultTypeDef",
+
+_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetOutputTypeDef],
+    },
+)
+_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
+        "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
+    total=False,
 )
 
+
+class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
@@ -6663,117 +6729,21 @@
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
-]
-_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "TaskArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-    },
-)
-_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetUnionTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "Replace": bool,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-):
-    pass
-
-PatchRuleGroupOutputTypeDef = TypedDict(
-    "PatchRuleGroupOutputTypeDef",
-    {
-        "PatchRules": List[PatchRuleOutputTypeDef],
-    },
-)
-
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -6782,29 +6752,48 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
+
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
+    {
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
+    },
+    total=False,
+)
+
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6838,18 +6827,25 @@
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+    },
+)
+
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -6866,33 +6862,64 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookOutputTypeDef],
+        "Runbooks": List[RunbookTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
+
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -6905,27 +6932,27 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationOutputTypeDef],
+        "TargetLocations": List[TargetLocationTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookOutputTypeDef],
+        "Runbooks": List[RunbookTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
@@ -6934,166 +6961,14 @@
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestEntryUnionTypeDef = Union[
-    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
-]
-RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetUnionTypeDef],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
-):
-    pass
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
-    {
-        "Parameters": Mapping[str, Sequence[str]],
-        "DocumentVersion": str,
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
-):
-    pass
-
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupOutputTypeDef,
-        "ApprovalRules": PatchRuleGroupOutputTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupOutputTypeDef,
-        "ApprovalRules": PatchRuleGroupOutputTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "GlobalFilters": PatchFilterGroupTypeDef,
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
@@ -7120,28 +6995,51 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceUnionTypeDef],
+        "Sources": Sequence[PatchSourceTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
+
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupTypeDef,
+        "ApprovalRules": PatchRuleGroupTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7152,26 +7050,49 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceUnionTypeDef],
+        "Sources": Sequence[PatchSourceTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupTypeDef,
+        "ApprovalRules": PatchRuleGroupTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7199,50 +7120,14 @@
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
-    },
-)
-
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookUnionTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": TimestampTypeDef,
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": TimestampTypeDef,
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
 )
@@ -7250,12 +7135,13 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
+
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.py` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.pyi` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

