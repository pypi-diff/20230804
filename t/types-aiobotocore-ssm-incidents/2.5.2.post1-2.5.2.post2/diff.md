# Comparing `tmp/types-aiobotocore-ssm-incidents-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ssm-incidents-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1.tar` & `types-aiobotocore-ssm-incidents-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.085448 types-aiobotocore-ssm-incidents-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-08-02 14:53:04.081448 types-aiobotocore-ssm-incidents-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.085448 types-aiobotocore-ssm-incidents-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.081448 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35951 2023-08-02 14:50:12.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35883 2023-08-02 14:50:12.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 14:50:11.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.081448 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15093 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13552 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2113 2023-08-04 13:54:21.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2350 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2349 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27541 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27495 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10098 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10096 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8283 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8274 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33953 2023-08-04 13:54:26.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33889 2023-08-04 13:54:26.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2829 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2827 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15093 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1012 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/LICENSE` & `types-aiobotocore-ssm-incidents-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-ssm-incidents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,152 +344,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ssm_incidents.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SSMIncidents` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/literals/).
+
 ```python
-from types_aiobotocore_ssm_incidents.literals import (
-    GetResourcePoliciesPaginatorName,
-    IncidentRecordStatusType,
-    ItemTypeType,
-    ListIncidentRecordsPaginatorName,
-    ListRelatedItemsPaginatorName,
-    ListReplicationSetsPaginatorName,
-    ListResponsePlansPaginatorName,
-    ListTimelineEventsPaginatorName,
-    RegionStatusType,
-    ReplicationSetStatusType,
-    SortOrderType,
-    SsmTargetAccountType,
-    TimelineEventSortType,
-    VariableTypeType,
-    WaitForReplicationSetActiveWaiterName,
-    WaitForReplicationSetDeletedWaiterName,
-    SSMIncidentsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_ssm_incidents.literals import GetResourcePoliciesPaginatorName
 
 
 def check_value(value: GetResourcePoliciesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ssm_incidents.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSMIncidents` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/type_defs/).
+
 ```python
-from types_aiobotocore_ssm_incidents.type_defs import (
-    AddRegionActionTypeDef,
-    AttributeValueListTypeDef,
-    AutomationExecutionTypeDef,
-    ChatChannelOutputTypeDef,
-    ChatChannelTypeDef,
-    TimestampTypeDef,
-    RegionMapInputValueTypeDef,
-    ResponseMetadataTypeDef,
-    EventReferenceTypeDef,
-    DeleteIncidentRecordInputRequestTypeDef,
-    DeleteRegionActionTypeDef,
-    DeleteReplicationSetInputRequestTypeDef,
-    DeleteResourcePolicyInputRequestTypeDef,
-    DeleteResponsePlanInputRequestTypeDef,
-    DeleteTimelineEventInputRequestTypeDef,
-    DynamicSsmParameterValueTypeDef,
-    GetIncidentRecordInputRequestTypeDef,
-    GetReplicationSetInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    GetResourcePoliciesInputRequestTypeDef,
-    ResourcePolicyTypeDef,
-    GetResponsePlanInputRequestTypeDef,
-    GetTimelineEventInputRequestTypeDef,
-    IncidentRecordSourceTypeDef,
-    NotificationTargetItemTypeDef,
-    PagerDutyIncidentDetailTypeDef,
-    ListRelatedItemsInputRequestTypeDef,
-    ListReplicationSetsInputRequestTypeDef,
-    ListResponsePlansInputRequestTypeDef,
-    ResponsePlanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PagerDutyIncidentConfigurationTypeDef,
-    PutResourcePolicyInputRequestTypeDef,
-    RegionInfoTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDeletionProtectionInputRequestTypeDef,
-    ChatChannelUnionTypeDef,
-    ConditionTypeDef,
-    TriggerDetailsTypeDef,
-    CreateReplicationSetInputRequestTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
-    CreateTimelineEventOutputTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    StartIncidentOutputTypeDef,
-    CreateTimelineEventInputRequestTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
-    UpdateTimelineEventInputRequestTypeDef,
-    UpdateReplicationSetActionTypeDef,
-    SsmAutomationOutputTypeDef,
-    SsmAutomationTypeDef,
-    GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
-    GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
-    GetResourcePoliciesOutputTypeDef,
-    IncidentRecordSummaryTypeDef,
-    IncidentRecordTypeDef,
-    IncidentTemplateOutputTypeDef,
-    IncidentTemplateTypeDef,
-    UpdateIncidentRecordInputRequestTypeDef,
-    ItemValueTypeDef,
-    ListResponsePlansOutputTypeDef,
-    PagerDutyConfigurationTypeDef,
-    ReplicationSetTypeDef,
-    FilterTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
-    UpdateReplicationSetInputRequestTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ListIncidentRecordsOutputTypeDef,
-    GetIncidentRecordOutputTypeDef,
-    IncidentTemplateUnionTypeDef,
-    ItemIdentifierTypeDef,
-    IntegrationTypeDef,
-    GetReplicationSetOutputTypeDef,
-    ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
-    ListIncidentRecordsInputRequestTypeDef,
-    ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
-    ListTimelineEventsInputRequestTypeDef,
-    ActionUnionTypeDef,
-    RelatedItemTypeDef,
-    GetResponsePlanOutputTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
-    UpdateResponsePlanInputRequestTypeDef,
-    ListRelatedItemsOutputTypeDef,
-    RelatedItemsUpdateTypeDef,
-    StartIncidentInputRequestTypeDef,
-    UpdateRelatedItemsInputRequestTypeDef,
-)
+from types_aiobotocore_ssm_incidents.type_defs import AddRegionActionTypeDef
 
 
 def get_value() -> AddRegionActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/README.md` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ssm-incidents
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ssm-incidents type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-ssm-incidents"></a>
 
 # types-aiobotocore-ssm-incidents
 
 [![PyPI - types-aiobotocore-ssm-incidents](https://img.shields.io/pypi/v/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-ssm-incidents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,152 +344,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ssm_incidents.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SSMIncidents` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/literals/).
+
 ```python
-from types_aiobotocore_ssm_incidents.literals import (
-    GetResourcePoliciesPaginatorName,
-    IncidentRecordStatusType,
-    ItemTypeType,
-    ListIncidentRecordsPaginatorName,
-    ListRelatedItemsPaginatorName,
-    ListReplicationSetsPaginatorName,
-    ListResponsePlansPaginatorName,
-    ListTimelineEventsPaginatorName,
-    RegionStatusType,
-    ReplicationSetStatusType,
-    SortOrderType,
-    SsmTargetAccountType,
-    TimelineEventSortType,
-    VariableTypeType,
-    WaitForReplicationSetActiveWaiterName,
-    WaitForReplicationSetDeletedWaiterName,
-    SSMIncidentsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_ssm_incidents.literals import GetResourcePoliciesPaginatorName
 
 
 def check_value(value: GetResourcePoliciesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ssm_incidents.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSMIncidents` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/type_defs/).
+
 ```python
-from types_aiobotocore_ssm_incidents.type_defs import (
-    AddRegionActionTypeDef,
-    AttributeValueListTypeDef,
-    AutomationExecutionTypeDef,
-    ChatChannelOutputTypeDef,
-    ChatChannelTypeDef,
-    TimestampTypeDef,
-    RegionMapInputValueTypeDef,
-    ResponseMetadataTypeDef,
-    EventReferenceTypeDef,
-    DeleteIncidentRecordInputRequestTypeDef,
-    DeleteRegionActionTypeDef,
-    DeleteReplicationSetInputRequestTypeDef,
-    DeleteResourcePolicyInputRequestTypeDef,
-    DeleteResponsePlanInputRequestTypeDef,
-    DeleteTimelineEventInputRequestTypeDef,
-    DynamicSsmParameterValueTypeDef,
-    GetIncidentRecordInputRequestTypeDef,
-    GetReplicationSetInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    GetResourcePoliciesInputRequestTypeDef,
-    ResourcePolicyTypeDef,
-    GetResponsePlanInputRequestTypeDef,
-    GetTimelineEventInputRequestTypeDef,
-    IncidentRecordSourceTypeDef,
-    NotificationTargetItemTypeDef,
-    PagerDutyIncidentDetailTypeDef,
-    ListRelatedItemsInputRequestTypeDef,
-    ListReplicationSetsInputRequestTypeDef,
-    ListResponsePlansInputRequestTypeDef,
-    ResponsePlanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PagerDutyIncidentConfigurationTypeDef,
-    PutResourcePolicyInputRequestTypeDef,
-    RegionInfoTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDeletionProtectionInputRequestTypeDef,
-    ChatChannelUnionTypeDef,
-    ConditionTypeDef,
-    TriggerDetailsTypeDef,
-    CreateReplicationSetInputRequestTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
-    CreateTimelineEventOutputTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    StartIncidentOutputTypeDef,
-    CreateTimelineEventInputRequestTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
-    UpdateTimelineEventInputRequestTypeDef,
-    UpdateReplicationSetActionTypeDef,
-    SsmAutomationOutputTypeDef,
-    SsmAutomationTypeDef,
-    GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
-    GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
-    GetResourcePoliciesOutputTypeDef,
-    IncidentRecordSummaryTypeDef,
-    IncidentRecordTypeDef,
-    IncidentTemplateOutputTypeDef,
-    IncidentTemplateTypeDef,
-    UpdateIncidentRecordInputRequestTypeDef,
-    ItemValueTypeDef,
-    ListResponsePlansOutputTypeDef,
-    PagerDutyConfigurationTypeDef,
-    ReplicationSetTypeDef,
-    FilterTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
-    UpdateReplicationSetInputRequestTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ListIncidentRecordsOutputTypeDef,
-    GetIncidentRecordOutputTypeDef,
-    IncidentTemplateUnionTypeDef,
-    ItemIdentifierTypeDef,
-    IntegrationTypeDef,
-    GetReplicationSetOutputTypeDef,
-    ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
-    ListIncidentRecordsInputRequestTypeDef,
-    ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
-    ListTimelineEventsInputRequestTypeDef,
-    ActionUnionTypeDef,
-    RelatedItemTypeDef,
-    GetResponsePlanOutputTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
-    UpdateResponsePlanInputRequestTypeDef,
-    ListRelatedItemsOutputTypeDef,
-    RelatedItemsUpdateTypeDef,
-    StartIncidentInputRequestTypeDef,
-    UpdateRelatedItemsInputRequestTypeDef,
-)
+from types_aiobotocore_ssm_incidents.type_defs import AddRegionActionTypeDef
 
 
 def get_value() -> AddRegionActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/setup.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-incidents",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__init__.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__init__.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/__main__.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMIncidents 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSMIncidents 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/client.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
-    ChatChannelUnionTypeDef,
+    ActionTypeDef,
+    ChatChannelTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
-    IncidentTemplateUnionTypeDef,
+    IncidentTemplateTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
@@ -63,37 +63,33 @@
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMIncidentsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class SSMIncidentsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
     """
 
     meta: ClientMeta
@@ -102,66 +98,61 @@
     def exceptions(self) -> Exceptions:
         """
         SSMIncidentsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#close)
         """
-
     async def create_replication_set(
         self,
         *,
         regions: Mapping[str, RegionMapInputValueTypeDef],
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateReplicationSetOutputTypeDef:
         """
         A replication set replicates and encrypts your data to the provided Regions with
         the provided KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_replication_set)
         """
-
     async def create_response_plan(
         self,
         *,
-        incidentTemplate: IncidentTemplateUnionTypeDef,
+        incidentTemplate: IncidentTemplateTypeDef,
         name: str,
-        actions: Sequence[ActionUnionTypeDef] = ...,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        actions: Sequence[ActionTypeDef] = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_response_plan)
         """
-
     async def create_timeline_event(
         self,
         *,
         eventData: str,
         eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
@@ -171,166 +162,149 @@
         """
         Creates a custom timeline event on the incident details page of an incident
         record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_timeline_event)
         """
-
     async def delete_incident_record(self, *, arn: str) -> Dict[str, Any]:
         """
         Delete an incident record from Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_incident_record)
         """
-
     async def delete_replication_set(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes all Regions in your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_replication_set)
         """
-
     async def delete_resource_policy(self, *, policyId: str, resourceArn: str) -> Dict[str, Any]:
         """
         Deletes the resource policy that Resource Access Manager uses to share your
         Incident Manager resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_resource_policy)
         """
-
     async def delete_response_plan(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_response_plan)
         """
-
     async def delete_timeline_event(
         self, *, eventId: str, incidentRecordArn: str
     ) -> Dict[str, Any]:
         """
         Deletes a timeline event from an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_timeline_event)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#generate_presigned_url)
         """
-
     async def get_incident_record(self, *, arn: str) -> GetIncidentRecordOutputTypeDef:
         """
         Returns the details for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_incident_record)
         """
-
     async def get_replication_set(self, *, arn: str) -> GetReplicationSetOutputTypeDef:
         """
         Retrieve your Incident Manager replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_replication_set)
         """
-
     async def get_resource_policies(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> GetResourcePoliciesOutputTypeDef:
         """
         Retrieves the resource policies attached to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_resource_policies)
         """
-
     async def get_response_plan(self, *, arn: str) -> GetResponsePlanOutputTypeDef:
         """
         Retrieves the details of the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_response_plan)
         """
-
     async def get_timeline_event(
         self, *, eventId: str, incidentRecordArn: str
     ) -> GetTimelineEventOutputTypeDef:
         """
         Retrieves a timeline event based on its ID and incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_timeline_event)
         """
-
     async def list_incident_records(
         self, *, filters: Sequence[FilterTypeDef] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListIncidentRecordsOutputTypeDef:
         """
         Lists all incident records in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_incident_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_incident_records)
         """
-
     async def list_related_items(
         self, *, incidentRecordArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListRelatedItemsOutputTypeDef:
         """
         List all related items for an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_related_items)
         """
-
     async def list_replication_sets(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListReplicationSetsOutputTypeDef:
         """
         Lists details about the replication set configured in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_replication_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_replication_sets)
         """
-
     async def list_response_plans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListResponsePlansOutputTypeDef:
         """
         Lists all response plans in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_response_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_response_plans)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags that are attached to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_tags_for_resource)
         """
-
     async def list_timeline_events(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -339,25 +313,23 @@
     ) -> ListTimelineEventsOutputTypeDef:
         """
         Lists timeline events for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_timeline_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_timeline_events)
         """
-
     async def put_resource_policy(
         self, *, policy: str, resourceArn: str
     ) -> PutResourcePolicyOutputTypeDef:
         """
         Adds a resource policy to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#put_resource_policy)
         """
-
     async def start_incident(
         self,
         *,
         responsePlanArn: str,
         clientToken: str = ...,
         impact: int = ...,
         relatedItems: Sequence[RelatedItemTypeDef] = ...,
@@ -367,95 +339,88 @@
         """
         Used to start an incident from CloudWatch alarms, EventBridge events, or
         manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.start_incident)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#start_incident)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds a tag to a response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#untag_resource)
         """
-
     async def update_deletion_protection(
         self, *, arn: str, deletionProtected: bool, clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Update deletion protection to either allow or deny deletion of the final Region
         in a replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_deletion_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_deletion_protection)
         """
-
     async def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
         """
         Update the details of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_incident_record)
         """
-
     async def update_related_items(
         self,
         *,
         incidentRecordArn: str,
         relatedItemsUpdate: RelatedItemsUpdateTypeDef,
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Add or remove related items from the related items tab of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_related_items)
         """
-
     async def update_replication_set(
         self,
         *,
         actions: Sequence[UpdateReplicationSetActionTypeDef],
         arn: str,
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Add or delete Regions from your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_replication_set)
         """
-
     async def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[ActionUnionTypeDef] = ...,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        actions: Sequence[ActionTypeDef] = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
@@ -465,15 +430,14 @@
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_response_plan)
         """
-
     async def update_timeline_event(
         self,
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
@@ -483,91 +447,81 @@
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_timeline_event)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_incident_records"]
     ) -> ListIncidentRecordsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_related_items"]
     ) -> ListRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_replication_sets"]
     ) -> ListReplicationSetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_response_plans"]
     ) -> ListResponsePlansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_timeline_events"]
     ) -> ListTimelineEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["wait_for_replication_set_active"]
     ) -> WaitForReplicationSetActiveWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["wait_for_replication_set_deleted"]
     ) -> WaitForReplicationSetDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "SSMIncidentsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/client.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
-    ActionUnionTypeDef,
-    ChatChannelUnionTypeDef,
+    ActionTypeDef,
+    ChatChannelTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
-    IncidentTemplateUnionTypeDef,
+    IncidentTemplateTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
@@ -63,33 +63,37 @@
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SSMIncidentsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class SSMIncidentsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
     """
 
     meta: ClientMeta
@@ -98,61 +102,66 @@
     def exceptions(self) -> Exceptions:
         """
         SSMIncidentsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#close)
         """
+
     async def create_replication_set(
         self,
         *,
         regions: Mapping[str, RegionMapInputValueTypeDef],
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateReplicationSetOutputTypeDef:
         """
         A replication set replicates and encrypts your data to the provided Regions with
         the provided KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_replication_set)
         """
+
     async def create_response_plan(
         self,
         *,
-        incidentTemplate: IncidentTemplateUnionTypeDef,
+        incidentTemplate: IncidentTemplateTypeDef,
         name: str,
-        actions: Sequence[ActionUnionTypeDef] = ...,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        actions: Sequence[ActionTypeDef] = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_response_plan)
         """
+
     async def create_timeline_event(
         self,
         *,
         eventData: str,
         eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
@@ -162,149 +171,166 @@
         """
         Creates a custom timeline event on the incident details page of an incident
         record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#create_timeline_event)
         """
+
     async def delete_incident_record(self, *, arn: str) -> Dict[str, Any]:
         """
         Delete an incident record from Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_incident_record)
         """
+
     async def delete_replication_set(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes all Regions in your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_replication_set)
         """
+
     async def delete_resource_policy(self, *, policyId: str, resourceArn: str) -> Dict[str, Any]:
         """
         Deletes the resource policy that Resource Access Manager uses to share your
         Incident Manager resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_resource_policy)
         """
+
     async def delete_response_plan(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_response_plan)
         """
+
     async def delete_timeline_event(
         self, *, eventId: str, incidentRecordArn: str
     ) -> Dict[str, Any]:
         """
         Deletes a timeline event from an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.delete_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#delete_timeline_event)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#generate_presigned_url)
         """
+
     async def get_incident_record(self, *, arn: str) -> GetIncidentRecordOutputTypeDef:
         """
         Returns the details for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_incident_record)
         """
+
     async def get_replication_set(self, *, arn: str) -> GetReplicationSetOutputTypeDef:
         """
         Retrieve your Incident Manager replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_replication_set)
         """
+
     async def get_resource_policies(
         self, *, resourceArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> GetResourcePoliciesOutputTypeDef:
         """
         Retrieves the resource policies attached to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_resource_policies)
         """
+
     async def get_response_plan(self, *, arn: str) -> GetResponsePlanOutputTypeDef:
         """
         Retrieves the details of the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_response_plan)
         """
+
     async def get_timeline_event(
         self, *, eventId: str, incidentRecordArn: str
     ) -> GetTimelineEventOutputTypeDef:
         """
         Retrieves a timeline event based on its ID and incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_timeline_event)
         """
+
     async def list_incident_records(
         self, *, filters: Sequence[FilterTypeDef] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListIncidentRecordsOutputTypeDef:
         """
         Lists all incident records in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_incident_records)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_incident_records)
         """
+
     async def list_related_items(
         self, *, incidentRecordArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListRelatedItemsOutputTypeDef:
         """
         List all related items for an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_related_items)
         """
+
     async def list_replication_sets(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListReplicationSetsOutputTypeDef:
         """
         Lists details about the replication set configured in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_replication_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_replication_sets)
         """
+
     async def list_response_plans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListResponsePlansOutputTypeDef:
         """
         Lists all response plans in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_response_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_response_plans)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags that are attached to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_tags_for_resource)
         """
+
     async def list_timeline_events(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -313,23 +339,25 @@
     ) -> ListTimelineEventsOutputTypeDef:
         """
         Lists timeline events for the specified incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.list_timeline_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#list_timeline_events)
         """
+
     async def put_resource_policy(
         self, *, policy: str, resourceArn: str
     ) -> PutResourcePolicyOutputTypeDef:
         """
         Adds a resource policy to the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#put_resource_policy)
         """
+
     async def start_incident(
         self,
         *,
         responsePlanArn: str,
         clientToken: str = ...,
         impact: int = ...,
         relatedItems: Sequence[RelatedItemTypeDef] = ...,
@@ -339,88 +367,95 @@
         """
         Used to start an incident from CloudWatch alarms, EventBridge events, or
         manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.start_incident)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#start_incident)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds a tag to a response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#untag_resource)
         """
+
     async def update_deletion_protection(
         self, *, arn: str, deletionProtected: bool, clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Update deletion protection to either allow or deny deletion of the final Region
         in a replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_deletion_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_deletion_protection)
         """
+
     async def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
         """
         Update the details of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_incident_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_incident_record)
         """
+
     async def update_related_items(
         self,
         *,
         incidentRecordArn: str,
         relatedItemsUpdate: RelatedItemsUpdateTypeDef,
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Add or remove related items from the related items tab of an incident record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_related_items)
         """
+
     async def update_replication_set(
         self,
         *,
         actions: Sequence[UpdateReplicationSetActionTypeDef],
         arn: str,
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Add or delete Regions from your replication set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_replication_set)
         """
+
     async def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[ActionUnionTypeDef] = ...,
-        chatChannel: ChatChannelUnionTypeDef = ...,
+        actions: Sequence[ActionTypeDef] = ...,
+        chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
@@ -430,14 +465,15 @@
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_response_plan)
         """
+
     async def update_timeline_event(
         self,
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
@@ -447,81 +483,91 @@
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#update_timeline_event)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_incident_records"]
     ) -> ListIncidentRecordsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_related_items"]
     ) -> ListRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_replication_sets"]
     ) -> ListReplicationSetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_response_plans"]
     ) -> ListResponsePlansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_timeline_events"]
     ) -> ListTimelineEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_paginator)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["wait_for_replication_set_active"]
     ) -> WaitForReplicationSetActiveWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["wait_for_replication_set_deleted"]
     ) -> WaitForReplicationSetDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "SSMIncidentsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/client/)
         """
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/literals.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetResourcePoliciesPaginatorName",
     "IncidentRecordStatusType",
     "ItemTypeType",
     "ListIncidentRecordsPaginatorName",
     "ListRelatedItemsPaginatorName",
     "ListReplicationSetsPaginatorName",
@@ -40,15 +39,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 IncidentRecordStatusType = Literal["OPEN", "RESOLVED"]
 ItemTypeType = Literal[
     "ANALYSIS",
     "ATTACHMENT",
     "AUTOMATION",
     "INCIDENT",
@@ -83,14 +81,15 @@
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
@@ -186,14 +185,15 @@
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
@@ -272,26 +272,28 @@
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/literals.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.py`

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
     "GetResourcePoliciesPaginatorName",
     "IncidentRecordStatusType",
     "ItemTypeType",
     "ListIncidentRecordsPaginatorName",
     "ListRelatedItemsPaginatorName",
     "ListReplicationSetsPaginatorName",
@@ -39,14 +40,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 IncidentRecordStatusType = Literal["OPEN", "RESOLVED"]
 ItemTypeType = Literal[
     "ANALYSIS",
     "ATTACHMENT",
     "AUTOMATION",
     "INCIDENT",
@@ -81,14 +83,15 @@
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
@@ -184,14 +187,15 @@
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
@@ -270,26 +274,28 @@
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/paginator.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/paginator.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/type_defs.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
-    "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "TimestampTypeDef",
     "RegionMapInputValueTypeDef",
     "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
@@ -70,15 +69,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
-    "ChatChannelUnionTypeDef",
     "ConditionTypeDef",
     "TriggerDetailsTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
     "CreateReplicationSetOutputTypeDef",
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
@@ -86,52 +84,47 @@
     "PutResourcePolicyOutputTypeDef",
     "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
     "EventSummaryTypeDef",
     "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
-    "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
-    "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "IncidentTemplateUnionTypeDef",
     "ItemIdentifierTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
-    "ActionUnionTypeDef",
     "RelatedItemTypeDef",
-    "GetResponsePlanOutputTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
+    "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -167,23 +160,14 @@
     "AutomationExecutionTypeDef",
     {
         "ssmExecutionArn": str,
     },
     total=False,
 )
 
-ChatChannelOutputTypeDef = TypedDict(
-    "ChatChannelOutputTypeDef",
-    {
-        "chatbotSns": List[str],
-        "empty": Dict[str, Any],
-    },
-    total=False,
-)
-
 ChatChannelTypeDef = TypedDict(
     "ChatChannelTypeDef",
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
@@ -542,15 +526,14 @@
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
 
-ChatChannelUnionTypeDef = Union[ChatChannelTypeDef, ChatChannelOutputTypeDef]
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": TimestampTypeDef,
         "before": TimestampTypeDef,
         "equals": AttributeValueListTypeDef,
     },
@@ -762,39 +745,14 @@
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
 )
 
-_RequiredSsmAutomationOutputTypeDef = TypedDict(
-    "_RequiredSsmAutomationOutputTypeDef",
-    {
-        "documentName": str,
-        "roleArn": str,
-    },
-)
-_OptionalSsmAutomationOutputTypeDef = TypedDict(
-    "_OptionalSsmAutomationOutputTypeDef",
-    {
-        "documentVersion": str,
-        "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
-        "parameters": Dict[str, List[str]],
-        "targetAccount": SsmTargetAccountType,
-    },
-    total=False,
-)
-
-
-class SsmAutomationOutputTypeDef(
-    _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
-):
-    pass
-
-
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -967,52 +925,27 @@
         "title": str,
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
-        "chatChannel": ChatChannelOutputTypeDef,
+        "chatChannel": ChatChannelTypeDef,
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
 
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
 
-_RequiredIncidentTemplateOutputTypeDef = TypedDict(
-    "_RequiredIncidentTemplateOutputTypeDef",
-    {
-        "impact": int,
-        "title": str,
-    },
-)
-_OptionalIncidentTemplateOutputTypeDef = TypedDict(
-    "_OptionalIncidentTemplateOutputTypeDef",
-    {
-        "dedupeString": str,
-        "incidentTags": Dict[str, str],
-        "notificationTargets": List[NotificationTargetItemTypeDef],
-        "summary": str,
-    },
-    total=False,
-)
-
-
-class IncidentTemplateOutputTypeDef(
-    _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
-):
-    pass
-
-
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -1158,22 +1091,14 @@
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "ssmAutomation": SsmAutomationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
@@ -1191,15 +1116,14 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IncidentTemplateUnionTypeDef = Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef]
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
@@ -1285,15 +1209,14 @@
 
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
 
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1306,40 +1229,25 @@
 )
 
 
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
 
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionUnionTypeDef],
+        "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
@@ -1349,24 +1257,39 @@
 
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
 
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionUnionTypeDef],
+        "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/type_defs.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
-    "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "TimestampTypeDef",
     "RegionMapInputValueTypeDef",
     "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
@@ -69,15 +68,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
-    "ChatChannelUnionTypeDef",
     "ConditionTypeDef",
     "TriggerDetailsTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
     "CreateReplicationSetOutputTypeDef",
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
@@ -85,52 +83,47 @@
     "PutResourcePolicyOutputTypeDef",
     "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
     "EventSummaryTypeDef",
     "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
-    "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
-    "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
-    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "IncidentTemplateUnionTypeDef",
     "ItemIdentifierTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
-    "ActionUnionTypeDef",
     "RelatedItemTypeDef",
-    "GetResponsePlanOutputTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
+    "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -164,23 +157,14 @@
     "AutomationExecutionTypeDef",
     {
         "ssmExecutionArn": str,
     },
     total=False,
 )
 
-ChatChannelOutputTypeDef = TypedDict(
-    "ChatChannelOutputTypeDef",
-    {
-        "chatbotSns": List[str],
-        "empty": Dict[str, Any],
-    },
-    total=False,
-)
-
 ChatChannelTypeDef = TypedDict(
     "ChatChannelTypeDef",
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
@@ -525,15 +509,14 @@
 
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
-ChatChannelUnionTypeDef = Union[ChatChannelTypeDef, ChatChannelOutputTypeDef]
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": TimestampTypeDef,
         "before": TimestampTypeDef,
         "equals": AttributeValueListTypeDef,
     },
@@ -733,37 +716,14 @@
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
 )
 
-_RequiredSsmAutomationOutputTypeDef = TypedDict(
-    "_RequiredSsmAutomationOutputTypeDef",
-    {
-        "documentName": str,
-        "roleArn": str,
-    },
-)
-_OptionalSsmAutomationOutputTypeDef = TypedDict(
-    "_OptionalSsmAutomationOutputTypeDef",
-    {
-        "documentVersion": str,
-        "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
-        "parameters": Dict[str, List[str]],
-        "targetAccount": SsmTargetAccountType,
-    },
-    total=False,
-)
-
-class SsmAutomationOutputTypeDef(
-    _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
-):
-    pass
-
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -924,48 +884,25 @@
         "title": str,
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
-        "chatChannel": ChatChannelOutputTypeDef,
+        "chatChannel": ChatChannelTypeDef,
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
-_RequiredIncidentTemplateOutputTypeDef = TypedDict(
-    "_RequiredIncidentTemplateOutputTypeDef",
-    {
-        "impact": int,
-        "title": str,
-    },
-)
-_OptionalIncidentTemplateOutputTypeDef = TypedDict(
-    "_OptionalIncidentTemplateOutputTypeDef",
-    {
-        "dedupeString": str,
-        "incidentTags": Dict[str, str],
-        "notificationTargets": List[NotificationTargetItemTypeDef],
-        "summary": str,
-    },
-    total=False,
-)
-
-class IncidentTemplateOutputTypeDef(
-    _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
-):
-    pass
-
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -1103,22 +1040,14 @@
 
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-ActionOutputTypeDef = TypedDict(
-    "ActionOutputTypeDef",
-    {
-        "ssmAutomation": SsmAutomationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
@@ -1136,15 +1065,14 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IncidentTemplateUnionTypeDef = Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef]
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
@@ -1226,15 +1154,14 @@
 )
 
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
-ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1245,40 +1172,25 @@
     },
     total=False,
 )
 
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionUnionTypeDef],
+        "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
@@ -1286,24 +1198,39 @@
 )
 
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[ActionUnionTypeDef],
+        "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/waiter.py` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents/waiter.pyi` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post1/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

