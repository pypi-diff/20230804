# Comparing `tmp/types-aiobotocore-connect-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-connect-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
```

## Comparing `types-aiobotocore-connect-2.5.2.post1.tar` & `types-aiobotocore-connect-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.233613 types-aiobotocore-connect-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47006 2023-08-02 14:52:07.225613 types-aiobotocore-connect-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45488 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.233613 types-aiobotocore-connect-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.225613 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   156992 2023-08-02 14:35:45.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   156744 2023-08-02 14:35:44.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-08-02 14:35:45.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-08-02 14:35:45.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-02 14:35:45.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-02 14:35:45.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   226764 2023-08-02 14:35:52.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   226415 2023-08-02 14:35:49.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:42.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.225613 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47006 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:07.000000 types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.963744 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156901 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   156653 2023-08-04 11:43:02.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-08-04 11:43:04.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-08-04 11:43:04.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-04 11:43:03.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   217314 2023-08-04 11:43:11.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216983 2023-08-04 11:43:07.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:01.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.967744 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:41.000000 types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-2.5.2.post1/LICENSE` & `types-aiobotocore-connect-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/setup.py` & `types-aiobotocore-connect-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__init__.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__init__.pyi` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/__main__.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/client.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationFormItemUnionTypeDef,
+    EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
@@ -205,15 +205,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
-    MetricV2UnionTypeDef,
+    MetricV2TypeDef,
     MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
@@ -225,15 +225,15 @@
     ReferenceTypeDef,
     ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RuleActionUnionTypeDef,
+    RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
     SearchPromptsResponseTypeDef,
     SearchQueuesResponseTypeDef,
     SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsResponseTypeDef,
@@ -245,18 +245,18 @@
     SecurityProfilesSearchFilterTypeDef,
     StartChatContactResponseTypeDef,
     StartContactEvaluationResponseTypeDef,
     StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactResponseTypeDef,
     SubmitContactEvaluationResponseTypeDef,
-    TaskTemplateConstraintsUnionTypeDef,
-    TaskTemplateDefaultsUnionTypeDef,
-    TaskTemplateFieldUnionTypeDef,
-    TelephonyConfigUnionTypeDef,
+    TaskTemplateConstraintsTypeDef,
+    TaskTemplateDefaultsTypeDef,
+    TaskTemplateFieldTypeDef,
+    TelephonyConfigTypeDef,
     TimestampTypeDef,
     TransferContactResponseTypeDef,
     UpdateContactEvaluationResponseTypeDef,
     UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdatePromptResponseTypeDef,
@@ -532,15 +532,15 @@
         """
 
     async def create_evaluation_form(
         self,
         *,
         InstanceId: str,
         Title: str,
-        Items: Sequence[EvaluationFormItemUnionTypeDef],
+        Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
@@ -688,15 +688,15 @@
     async def create_rule(
         self,
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
-        Actions: Sequence[RuleActionUnionTypeDef],
+        Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
@@ -722,19 +722,19 @@
         """
 
     async def create_task_template(
         self,
         *,
         InstanceId: str,
         Name: str,
-        Fields: Sequence[TaskTemplateFieldUnionTypeDef],
+        Fields: Sequence[TaskTemplateFieldTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
-        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
+        Constraints: TaskTemplateConstraintsTypeDef = ...,
+        Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
@@ -1400,15 +1400,15 @@
     async def get_metric_data_v2(
         self,
         *,
         ResourceArn: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
-        Metrics: Sequence[MetricV2UnionTypeDef],
+        Metrics: Sequence[MetricV2TypeDef],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
@@ -2451,15 +2451,15 @@
     async def update_evaluation_form(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
-        Items: Sequence[EvaluationFormItemUnionTypeDef],
+        Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
@@ -2676,15 +2676,15 @@
     async def update_rule(
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
-        Actions: Sequence[RuleActionUnionTypeDef],
+        Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_rule)
@@ -2711,29 +2711,29 @@
         self,
         *,
         TaskTemplateId: str,
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
-        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
+        Constraints: TaskTemplateConstraintsTypeDef = ...,
+        Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldUnionTypeDef] = ...
+        Fields: Sequence[TaskTemplateFieldTypeDef] = ...
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_task_template)
         """
 
     async def update_traffic_distribution(
-        self, *, Id: str, TelephonyConfig: TelephonyConfigUnionTypeDef = ...
+        self, *, Id: str, TelephonyConfig: TelephonyConfigTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_traffic_distribution)
         """
```

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/client.pyi` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     DescribeTrafficDistributionGroupResponseTypeDef,
     DescribeUserHierarchyGroupResponseTypeDef,
     DescribeUserHierarchyStructureResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVocabularyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationAnswerInputTypeDef,
-    EvaluationFormItemUnionTypeDef,
+    EvaluationFormItemTypeDef,
     EvaluationFormScoringStrategyTypeDef,
     EvaluationNoteTypeDef,
     FiltersTypeDef,
     FilterV2TypeDef,
     GetContactAttributesResponseTypeDef,
     GetCurrentMetricDataResponseTypeDef,
     GetCurrentUserDataResponseTypeDef,
@@ -205,15 +205,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskTemplatesResponseTypeDef,
     ListTrafficDistributionGroupsResponseTypeDef,
     ListUseCasesResponseTypeDef,
     ListUserHierarchyGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     MediaConcurrencyTypeDef,
-    MetricV2UnionTypeDef,
+    MetricV2TypeDef,
     MonitorContactResponseTypeDef,
     OutboundCallerConfigTypeDef,
     ParticipantDetailsToAddTypeDef,
     ParticipantDetailsTypeDef,
     PersistentChatTypeDef,
     PromptSearchCriteriaTypeDef,
     PromptSearchFilterTypeDef,
@@ -225,15 +225,15 @@
     ReferenceTypeDef,
     ReplicateInstanceResponseTypeDef,
     ResourceTagsSearchCriteriaTypeDef,
     RoutingProfileQueueConfigTypeDef,
     RoutingProfileQueueReferenceTypeDef,
     RoutingProfileSearchCriteriaTypeDef,
     RoutingProfileSearchFilterTypeDef,
-    RuleActionUnionTypeDef,
+    RuleActionTypeDef,
     RuleTriggerEventSourceTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SearchHoursOfOperationsResponseTypeDef,
     SearchPromptsResponseTypeDef,
     SearchQueuesResponseTypeDef,
     SearchQuickConnectsResponseTypeDef,
     SearchResourceTagsResponseTypeDef,
@@ -245,18 +245,18 @@
     SecurityProfilesSearchFilterTypeDef,
     StartChatContactResponseTypeDef,
     StartContactEvaluationResponseTypeDef,
     StartContactStreamingResponseTypeDef,
     StartOutboundVoiceContactResponseTypeDef,
     StartTaskContactResponseTypeDef,
     SubmitContactEvaluationResponseTypeDef,
-    TaskTemplateConstraintsUnionTypeDef,
-    TaskTemplateDefaultsUnionTypeDef,
-    TaskTemplateFieldUnionTypeDef,
-    TelephonyConfigUnionTypeDef,
+    TaskTemplateConstraintsTypeDef,
+    TaskTemplateDefaultsTypeDef,
+    TaskTemplateFieldTypeDef,
+    TelephonyConfigTypeDef,
     TimestampTypeDef,
     TransferContactResponseTypeDef,
     UpdateContactEvaluationResponseTypeDef,
     UpdateEvaluationFormResponseTypeDef,
     UpdateParticipantRoleConfigChannelInfoTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdatePromptResponseTypeDef,
@@ -510,15 +510,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_contact_flow_module)
         """
     async def create_evaluation_form(
         self,
         *,
         InstanceId: str,
         Title: str,
-        Items: Sequence[EvaluationFormItemUnionTypeDef],
+        Items: Sequence["EvaluationFormItemTypeDef"],
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...
     ) -> CreateEvaluationFormResponseTypeDef:
         """
         Creates an evaluation form in the specified Amazon Connect instance.
 
@@ -657,15 +657,15 @@
     async def create_rule(
         self,
         *,
         InstanceId: str,
         Name: str,
         TriggerEventSource: RuleTriggerEventSourceTypeDef,
         Function: str,
-        Actions: Sequence[RuleActionUnionTypeDef],
+        Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType,
         ClientToken: str = ...
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)
@@ -689,19 +689,19 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#create_security_profile)
         """
     async def create_task_template(
         self,
         *,
         InstanceId: str,
         Name: str,
-        Fields: Sequence[TaskTemplateFieldUnionTypeDef],
+        Fields: Sequence[TaskTemplateFieldTypeDef],
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
-        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
+        Constraints: TaskTemplateConstraintsTypeDef = ...,
+        Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
         ClientToken: str = ...
     ) -> CreateTaskTemplateResponseTypeDef:
         """
         Creates a new task template in the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)
@@ -1305,15 +1305,15 @@
     async def get_metric_data_v2(
         self,
         *,
         ResourceArn: str,
         StartTime: TimestampTypeDef,
         EndTime: TimestampTypeDef,
         Filters: Sequence[FilterV2TypeDef],
-        Metrics: Sequence[MetricV2UnionTypeDef],
+        Metrics: Sequence[MetricV2TypeDef],
         Groupings: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetMetricDataV2ResponseTypeDef:
         """
         Gets metric data from the specified Amazon Connect instance.
 
@@ -2278,15 +2278,15 @@
     async def update_evaluation_form(
         self,
         *,
         InstanceId: str,
         EvaluationFormId: str,
         EvaluationFormVersion: int,
         Title: str,
-        Items: Sequence[EvaluationFormItemUnionTypeDef],
+        Items: Sequence["EvaluationFormItemTypeDef"],
         CreateNewVersion: bool = ...,
         Description: str = ...,
         ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,
         ClientToken: str = ...
     ) -> UpdateEvaluationFormResponseTypeDef:
         """
         Updates details about a specific evaluation form version in the specified Amazon
@@ -2485,15 +2485,15 @@
     async def update_rule(
         self,
         *,
         RuleId: str,
         InstanceId: str,
         Name: str,
         Function: str,
-        Actions: Sequence[RuleActionUnionTypeDef],
+        Actions: Sequence[RuleActionTypeDef],
         PublishStatus: RulePublishStatusType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_rule)
@@ -2518,28 +2518,28 @@
         self,
         *,
         TaskTemplateId: str,
         InstanceId: str,
         Name: str = ...,
         Description: str = ...,
         ContactFlowId: str = ...,
-        Constraints: TaskTemplateConstraintsUnionTypeDef = ...,
-        Defaults: TaskTemplateDefaultsUnionTypeDef = ...,
+        Constraints: TaskTemplateConstraintsTypeDef = ...,
+        Defaults: TaskTemplateDefaultsTypeDef = ...,
         Status: TaskTemplateStatusType = ...,
-        Fields: Sequence[TaskTemplateFieldUnionTypeDef] = ...
+        Fields: Sequence[TaskTemplateFieldTypeDef] = ...
     ) -> UpdateTaskTemplateResponseTypeDef:
         """
         Updates details about a specific task template in the specified Amazon Connect
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_task_template)
         """
     async def update_traffic_distribution(
-        self, *, Id: str, TelephonyConfig: TelephonyConfigUnionTypeDef = ...
+        self, *, Id: str, TelephonyConfig: TelephonyConfigTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the traffic distribution for a given traffic distribution group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#update_traffic_distribution)
         """
```

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/literals.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/literals.pyi` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/paginator.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/paginator.pyi` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/type_defs.py` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionSummaryTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "QueueReferenceTypeDef",
     "AgentInfoTypeDef",
     "AgentStatusReferenceTypeDef",
@@ -120,15 +119,14 @@
     "ContactFlowTypeDef",
     "QueueInfoTypeDef",
     "WisdomInfoTypeDef",
     "TagConditionTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "EvaluationFormItemUnionTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantTokenCredentialsTypeDef",
     "CreatePromptRequestRequestTypeDef",
     "OutboundCallerConfigTypeDef",
@@ -202,15 +200,14 @@
     "DismissUserContactRequestRequestTypeDef",
     "DistributionTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
-    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSummaryTypeDef",
     "EvaluationFormVersionSummaryTypeDef",
     "EvaluationScoreTypeDef",
     "EvaluationNoteTypeDef",
@@ -283,19 +280,17 @@
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
     "TrafficDistributionGroupSummaryTypeDef",
     "ListUseCasesRequestRequestTypeDef",
     "UseCaseTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
-    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
     "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerValueTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
     "PutUserStatusRequestRequestTypeDef",
@@ -434,15 +429,14 @@
     "SearchPromptsResponseTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
     "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeVocabularyResponseTypeDef",
     "DimensionsTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "RoutingProfileQueueConfigTypeDef",
-    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "KinesisVideoStreamConfigTypeDef",
     "S3ConfigTypeDef",
     "EvaluationAnswerInputTypeDef",
     "EvaluationAnswerOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
@@ -506,15 +500,14 @@
     "InstanceTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsResponseTypeDef",
     "InvisibleFieldInfoTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "RequiredFieldInfoTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
-    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "ListPhoneNumbersV2ResponseTypeDef",
     "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsResponseTypeDef",
     "ListQuickConnectsResponseTypeDef",
     "ListQueuesResponseTypeDef",
@@ -522,24 +515,21 @@
     "ListRoutingProfilesResponseTypeDef",
     "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
-    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
-    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "StartChatContactRequestRequestTypeDef",
     "QuickConnectConfigTypeDef",
     "ReferenceSummaryTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "SearchResourceTagsResponseTypeDef",
     "SearchSecurityProfilesResponseTypeDef",
     "SearchVocabulariesResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
@@ -563,49 +553,42 @@
     "RoutingProfileTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "CurrentMetricResultTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "GetTrafficDistributionResponseTypeDef",
-    "TelephonyConfigUnionTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "InstanceStorageConfigTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
-    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationTypeDef",
     "ListContactEvaluationsResponseTypeDef",
     "UserDataTypeDef",
     "HierarchyGroupTypeDef",
     "DescribeUserHierarchyStructureResponseTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "DescribeInstanceResponseTypeDef",
-    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
-    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
-    "TaskTemplateFieldUnionTypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
     "MetricDataV2TypeDef",
-    "MetricV2UnionTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "ListContactReferencesResponseTypeDef",
-    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     "SearchUsersResponseTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     "SearchPromptsRequestRequestTypeDef",
@@ -623,46 +606,38 @@
     "DescribeRoutingProfileResponseTypeDef",
     "SearchRoutingProfilesResponseTypeDef",
     "GetCurrentMetricDataResponseTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     "DescribeInstanceStorageConfigResponseTypeDef",
     "ListInstanceStorageConfigsResponseTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
-    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     "DescribeContactEvaluationResponseTypeDef",
     "GetCurrentUserDataResponseTypeDef",
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "SearchHoursOfOperationsResponseTypeDef",
-    "TaskTemplateConstraintsUnionTypeDef",
-    "GetTaskTemplateResponseTypeDef",
-    "UpdateTaskTemplateResponseTypeDef",
-    "TaskTemplateDefaultsUnionTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
+    "GetTaskTemplateResponseTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
+    "UpdateTaskTemplateResponseTypeDef",
     "MetricResultV2TypeDef",
-    "GetMetricDataV2RequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "SearchQuickConnectsResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
-    "RuleActionUnionTypeDef",
-    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    "UpdateRuleRequestRequestTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
     "GetMetricDataResponseTypeDef",
     "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "UpdateRuleRequestRequestTypeDef",
-    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
-    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
         "ActionType": ActionTypeType,
@@ -787,22 +762,20 @@
     "_OptionalAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "VocabularyId": str,
     },
     total=False,
 )
 
-
 class AssociateDefaultVocabularyRequestRequestTypeDef(
     _RequiredAssociateDefaultVocabularyRequestRequestTypeDef,
     _OptionalAssociateDefaultVocabularyRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
     "AssociateLambdaFunctionRequestRequestTypeDef",
     {
         "InstanceId": str,
         "FunctionArn": str,
     },
 )
@@ -890,21 +863,19 @@
         "PhoneNumberDescription": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
     total=False,
@@ -1011,21 +982,19 @@
         "Description": str,
         "DisplayOrder": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateContactFlowModuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Content": str,
     },
@@ -1036,22 +1005,20 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateContactFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "Content": str,
@@ -1062,24 +1029,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
-
-EvaluationFormItemUnionTypeDef = Union[
-    "EvaluationFormItemTypeDef", "EvaluationFormItemOutputTypeDef"
-]
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
@@ -1098,21 +1060,19 @@
         "ClientToken": str,
         "InstanceAlias": str,
         "DirectoryId": str,
     },
     total=False,
 )
 
-
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateIntegrationAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationAssociationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
     },
@@ -1124,22 +1084,20 @@
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 ParticipantDetailsToAddTypeDef = TypedDict(
     "ParticipantDetailsToAddTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
         "DisplayName": str,
     },
     total=False,
@@ -1167,21 +1125,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
-
 OutboundCallerConfigTypeDef = TypedDict(
     "OutboundCallerConfigTypeDef",
     {
         "OutboundCallerIdName": str,
         "OutboundCallerIdNumberId": str,
         "OutboundFlowId": str,
     },
@@ -1198,21 +1154,19 @@
     "_OptionalRuleTriggerEventSourceTypeDef",
     {
         "IntegrationAssociationId": str,
     },
     total=False,
 )
 
-
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
-
 _RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileName": str,
         "InstanceId": str,
     },
 )
@@ -1224,22 +1178,20 @@
         "Tags": Mapping[str, str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrafficDistributionGroupRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
     },
 )
@@ -1249,22 +1201,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateUseCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUseCaseRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationAssociationId": str,
         "UseCaseType": UseCaseTypeType,
     },
@@ -1273,21 +1223,19 @@
     "_OptionalCreateUseCaseRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserHierarchyGroupRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
     },
 )
@@ -1296,22 +1244,20 @@
     {
         "ParentGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "Email": str,
         "SecondaryEmail": str,
@@ -1332,19 +1278,17 @@
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
     },
     total=False,
 )
 
-
 class UserPhoneConfigTypeDef(_RequiredUserPhoneConfigTypeDef, _OptionalUserPhoneConfigTypeDef):
     pass
 
-
 _RequiredCreateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyName": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "Content": str,
@@ -1355,21 +1299,19 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
@@ -1465,22 +1407,20 @@
     "_OptionalDeleteEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
-
 class DeleteEvaluationFormRequestRequestTypeDef(
     _RequiredDeleteEvaluationFormRequestRequestTypeDef,
     _OptionalDeleteEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DeleteHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1631,22 +1571,20 @@
     "_OptionalDescribeEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
-
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1826,19 +1764,17 @@
         "FailureReason": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class VocabularyTypeDef(_RequiredVocabularyTypeDef, _OptionalVocabularyTypeDef):
     pass
 
-
 RoutingProfileReferenceTypeDef = TypedDict(
     "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
     total=False,
@@ -1974,46 +1910,20 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
-
 class EvaluationFormNumericQuestionOptionTypeDef(
     _RequiredEvaluationFormNumericQuestionOptionTypeDef,
     _OptionalEvaluationFormNumericQuestionOptionTypeDef,
 ):
     pass
 
-
-_RequiredEvaluationFormSectionOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSectionOutputTypeDef",
-    {
-        "Title": str,
-        "RefId": str,
-        "Items": List[Dict[str, Any]],
-    },
-)
-_OptionalEvaluationFormSectionOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSectionOutputTypeDef",
-    {
-        "Instructions": str,
-        "Weight": float,
-    },
-    total=False,
-)
-
-
-class EvaluationFormSectionOutputTypeDef(
-    _RequiredEvaluationFormSectionOutputTypeDef, _OptionalEvaluationFormSectionOutputTypeDef
-):
-    pass
-
-
 _RequiredEvaluationFormSectionTypeDef = TypedDict(
     "_RequiredEvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence[Dict[str, Any]],
     },
@@ -2023,21 +1933,19 @@
     {
         "Instructions": str,
         "Weight": float,
     },
     total=False,
 )
 
-
 class EvaluationFormSectionTypeDef(
     _RequiredEvaluationFormSectionTypeDef, _OptionalEvaluationFormSectionTypeDef
 ):
     pass
 
-
 SingleSelectQuestionRuleCategoryAutomationTypeDef = TypedDict(
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     {
         "Category": str,
         "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
         "OptionRefId": str,
     },
@@ -2055,22 +1963,20 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionOptionTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionOptionTypeDef,
 ):
     pass
 
-
 _RequiredEvaluationFormSummaryTypeDef = TypedDict(
     "_RequiredEvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
@@ -2086,21 +1992,19 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "ActiveVersion": int,
     },
     total=False,
 )
 
-
 class EvaluationFormSummaryTypeDef(
     _RequiredEvaluationFormSummaryTypeDef, _OptionalEvaluationFormSummaryTypeDef
 ):
     pass
 
-
 EvaluationFormVersionSummaryTypeDef = TypedDict(
     "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
@@ -2201,21 +2105,19 @@
     "_OptionalGetTaskTemplateRequestRequestTypeDef",
     {
         "SnapshotVersion": str,
     },
     total=False,
 )
 
-
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
-
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -2375,21 +2277,19 @@
         "NextToken": str,
         "MaxResults": int,
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
     },
     total=False,
 )
 
-
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListApprovedOriginsRequestRequestTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestRequestTypeDef = TypedDict(
@@ -2397,22 +2297,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -2421,21 +2319,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListContactEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -2443,22 +2339,20 @@
     "_OptionalListContactEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowModulesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestRequestTypeDef = TypedDict(
@@ -2467,22 +2361,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ContactFlowModuleState": ContactFlowModuleStateType,
     },
     total=False,
 )
 
-
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestRequestTypeDef = TypedDict(
@@ -2491,21 +2383,19 @@
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListContactReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -2514,22 +2404,20 @@
     "_OptionalListContactReferencesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
@@ -2538,22 +2426,20 @@
         "LanguageCode": VocabularyLanguageCodeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -2562,22 +2448,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestRequestTypeDef = TypedDict(
@@ -2585,22 +2469,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestRequestTypeDef = TypedDict(
@@ -2608,22 +2490,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestRequestTypeDef = TypedDict(
@@ -2631,22 +2511,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceStorageConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -2655,22 +2533,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2688,22 +2564,20 @@
         "IntegrationType": IntegrationTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLambdaFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestRequestTypeDef = TypedDict(
@@ -2711,22 +2585,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLexBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListLexBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestRequestTypeDef = TypedDict(
@@ -2734,21 +2606,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListPhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -2758,21 +2628,19 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
-
 PhoneNumberSummaryTypeDef = TypedDict(
     "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
@@ -2818,21 +2686,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
-
 PromptSummaryTypeDef = TypedDict(
     "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -2851,22 +2717,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-
 QuickConnectSummaryTypeDef = TypedDict(
     "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
@@ -2886,21 +2750,19 @@
         "QueueTypes": Sequence[QueueTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
-
 QueueSummaryTypeDef = TypedDict(
     "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
@@ -2920,21 +2782,19 @@
         "NextToken": str,
         "MaxResults": int,
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
     },
     total=False,
 )
 
-
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -2943,22 +2803,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
-
 RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
     "RoutingProfileQueueConfigSummaryTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
@@ -2978,22 +2836,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 RoutingProfileSummaryTypeDef = TypedDict(
     "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -3013,21 +2869,19 @@
         "EventSourceName": EventSourceNameType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListSecurityKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestRequestTypeDef = TypedDict(
@@ -3035,21 +2889,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
-
 SecurityKeyTypeDef = TypedDict(
     "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
@@ -3068,22 +2920,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -3091,22 +2941,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 SecurityProfileSummaryTypeDef = TypedDict(
     "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -3133,21 +2981,19 @@
         "MaxResults": int,
         "Status": TaskTemplateStatusType,
         "Name": str,
     },
     total=False,
 )
 
-
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
-
 TaskTemplateMetadataTypeDef = TypedDict(
     "TaskTemplateMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
@@ -3192,21 +3038,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
-
 UseCaseTypeDef = TypedDict(
     "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
@@ -3224,22 +3068,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -3247,40 +3089,29 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 UserSummaryTypeDef = TypedDict(
     "UserSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
     },
     total=False,
 )
 
-MetricFilterV2OutputTypeDef = TypedDict(
-    "MetricFilterV2OutputTypeDef",
-    {
-        "MetricFilterKey": str,
-        "MetricFilterValues": List[str],
-    },
-    total=False,
-)
-
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
@@ -3308,30 +3139,19 @@
     {
         "AllowedMonitorCapabilities": Sequence[MonitorCapabilityType],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
-
-NotificationRecipientTypeOutputTypeDef = TypedDict(
-    "NotificationRecipientTypeOutputTypeDef",
-    {
-        "UserTags": Dict[str, str],
-        "UserIds": List[str],
-    },
-    total=False,
-)
-
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
     total=False,
@@ -3439,22 +3259,20 @@
     "_OptionalReleasePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ReleasePhoneNumberRequestRequestTypeDef(
     _RequiredReleasePhoneNumberRequestRequestTypeDef,
     _OptionalReleasePhoneNumberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredReplicateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ReplicaRegion": str,
         "ReplicaAlias": str,
     },
@@ -3463,21 +3281,19 @@
     "_OptionalReplicateInstanceRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
-
 TagSearchConditionTypeDef = TypedDict(
     "TagSearchConditionTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
@@ -3508,22 +3324,20 @@
         "PhoneNumberPrefix": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchAvailablePhoneNumbersRequestRequestTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestRequestTypeDef,
 ):
     pass
 
-
 TagSetTypeDef = TypedDict(
     "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -3556,22 +3370,20 @@
         "State": VocabularyStateType,
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
     total=False,
 )
 
-
 class SearchVocabulariesRequestRequestTypeDef(
     _RequiredSearchVocabulariesRequestRequestTypeDef,
     _OptionalSearchVocabulariesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredVocabularySummaryTypeDef = TypedDict(
     "_RequiredVocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
@@ -3583,21 +3395,19 @@
     "_OptionalVocabularySummaryTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
-
 class VocabularySummaryTypeDef(
     _RequiredVocabularySummaryTypeDef, _OptionalVocabularySummaryTypeDef
 ):
     pass
 
-
 _RequiredStartContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "EvaluationFormId": str,
     },
@@ -3606,22 +3416,20 @@
     "_OptionalStartContactEvaluationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
@@ -3683,21 +3491,19 @@
         "QueueId": str,
         "UserId": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -3717,21 +3523,19 @@
         "State": AgentStatusStateType,
         "DisplayOrder": int,
         "ResetOrderNumber": bool,
     },
     total=False,
 )
 
-
 class UpdateAgentStatusRequestRequestTypeDef(
     _RequiredUpdateAgentStatusRequestRequestTypeDef, _OptionalUpdateAgentStatusRequestRequestTypeDef
 ):
     pass
 
-
 UpdateContactAttributesRequestRequestTypeDef = TypedDict(
     "UpdateContactAttributesRequestRequestTypeDef",
     {
         "InitialContactId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -3759,22 +3563,20 @@
         "Name": str,
         "Description": str,
         "ContactFlowState": ContactFlowStateType,
     },
     total=False,
 )
 
-
 class UpdateContactFlowMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateContactFlowModuleContentRequestRequestTypeDef = TypedDict(
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
         "Content": str,
     },
@@ -3793,22 +3595,20 @@
         "Name": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
     },
     total=False,
 )
 
-
 class UpdateContactFlowModuleMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowModuleMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowModuleMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContactFlowNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactFlowNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
@@ -3817,22 +3617,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateContactFlowNameRequestRequestTypeDef(
     _RequiredUpdateContactFlowNameRequestRequestTypeDef,
     _OptionalUpdateContactFlowNameRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateInstanceAttributeRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
@@ -3849,21 +3647,19 @@
     "_OptionalUpdatePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
@@ -3873,21 +3669,19 @@
         "Name": str,
         "Description": str,
         "S3Uri": str,
     },
     total=False,
 )
 
-
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
-
 UpdateQueueHoursOfOperationRequestRequestTypeDef = TypedDict(
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "HoursOfOperationId": str,
     },
@@ -3904,22 +3698,20 @@
     "_OptionalUpdateQueueMaxContactsRequestRequestTypeDef",
     {
         "MaxContacts": int,
     },
     total=False,
 )
 
-
 class UpdateQueueMaxContactsRequestRequestTypeDef(
     _RequiredUpdateQueueMaxContactsRequestRequestTypeDef,
     _OptionalUpdateQueueMaxContactsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateQueueNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -3928,21 +3720,19 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateQueueNameRequestRequestTypeDef(
     _RequiredUpdateQueueNameRequestRequestTypeDef, _OptionalUpdateQueueNameRequestRequestTypeDef
 ):
     pass
 
-
 UpdateQueueStatusRequestRequestTypeDef = TypedDict(
     "UpdateQueueStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "Status": QueueStatusType,
     },
@@ -3960,22 +3750,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateQuickConnectNameRequestRequestTypeDef(
     _RequiredUpdateQuickConnectNameRequestRequestTypeDef,
     _OptionalUpdateQuickConnectNameRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "DefaultOutboundQueueId": str,
     },
@@ -3993,22 +3781,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateRoutingProfileNameRequestRequestTypeDef(
     _RequiredUpdateRoutingProfileNameRequestRequestTypeDef,
     _OptionalUpdateRoutingProfileNameRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -4019,22 +3805,20 @@
         "Permissions": Sequence[str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateUserHierarchyGroupNameRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     {
         "Name": str,
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
@@ -4051,22 +3835,20 @@
     "_OptionalUpdateUserHierarchyRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
     },
     total=False,
 )
 
-
 class UpdateUserHierarchyRequestRequestTypeDef(
     _RequiredUpdateUserHierarchyRequestRequestTypeDef,
     _OptionalUpdateUserHierarchyRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateUserRoutingProfileRequestRequestTypeDef = TypedDict(
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     {
         "RoutingProfileId": str,
         "UserId": str,
         "InstanceId": str,
     },
@@ -4564,22 +4346,20 @@
         "AnswerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "CampaignId": str,
         "TrafficType": TrafficTypeType,
     },
     total=False,
 )
 
-
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateLexBotRequestRequestTypeDef = TypedDict(
     "AssociateLexBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": LexBotTypeDef,
     },
 )
@@ -4604,21 +4384,19 @@
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
 )
 
-
 class AssociateBotRequestRequestTypeDef(
     _RequiredAssociateBotRequestRequestTypeDef, _OptionalAssociateBotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDisassociateBotRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateBotRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDisassociateBotRequestRequestTypeDef = TypedDict(
@@ -4626,21 +4404,19 @@
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
 )
 
-
 class DisassociateBotRequestRequestTypeDef(
     _RequiredDisassociateBotRequestRequestTypeDef, _OptionalDisassociateBotRequestRequestTypeDef
 ):
     pass
 
-
 LexBotConfigTypeDef = TypedDict(
     "LexBotConfigTypeDef",
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
@@ -4778,71 +4554,67 @@
 )
 
 _RequiredCreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Title": str,
-        "Items": Sequence[EvaluationFormItemUnionTypeDef],
+        "Items": Sequence["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalCreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEvaluationFormRequestRequestTypeDef",
     {
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredEvaluationFormContentTypeDef = TypedDict(
     "_RequiredEvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Items": List["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalEvaluationFormContentTypeDef = TypedDict(
     "_OptionalEvaluationFormContentTypeDef",
     {
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationFormContentTypeDef(
     _RequiredEvaluationFormContentTypeDef, _OptionalEvaluationFormContentTypeDef
 ):
     pass
 
-
 _RequiredEvaluationFormTypeDef = TypedDict(
     "_RequiredEvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
         "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Items": List["EvaluationFormItemTypeDef"],
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 _OptionalEvaluationFormTypeDef = TypedDict(
@@ -4851,48 +4623,44 @@
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class EvaluationFormTypeDef(_RequiredEvaluationFormTypeDef, _OptionalEvaluationFormTypeDef):
     pass
 
-
 _RequiredUpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Title": str,
-        "Items": Sequence[EvaluationFormItemUnionTypeDef],
+        "Items": Sequence["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalUpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEvaluationFormRequestRequestTypeDef",
     {
         "CreateNewVersion": bool,
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateParticipantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParticipantRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ParticipantDetails": ParticipantDetailsToAddTypeDef,
     },
@@ -4901,21 +4669,19 @@
     "_OptionalCreateParticipantRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
-
 CreateParticipantResponseTypeDef = TypedDict(
     "CreateParticipantResponseTypeDef",
     {
         "ParticipantCredentials": ParticipantTokenCredentialsTypeDef,
         "ParticipantId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4937,21 +4703,19 @@
         "MaxContacts": int,
         "QuickConnectIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-
 QueueTypeDef = TypedDict(
     "QueueTypeDef",
     {
         "Name": str,
         "QueueArn": str,
         "QueueId": str,
         "Description": str,
@@ -5000,21 +4764,19 @@
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 UpdateUserPhoneConfigRequestRequestTypeDef = TypedDict(
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     {
         "PhoneConfig": UserPhoneConfigTypeDef,
         "UserId": str,
         "InstanceId": str,
     },
@@ -5059,19 +4821,17 @@
     "_OptionalMediaConcurrencyTypeDef",
     {
         "CrossChannelBehavior": CrossChannelBehaviorTypeDef,
     },
     total=False,
 )
 
-
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
-
 CurrentMetricDataTypeDef = TypedDict(
     "CurrentMetricDataTypeDef",
     {
         "Metric": CurrentMetricTypeDef,
         "Value": float,
     },
     total=False,
@@ -5152,25 +4912,18 @@
     {
         "QueueReference": RoutingProfileQueueReferenceTypeDef,
         "Priority": int,
         "Delay": int,
     },
 )
 
-TelephonyConfigOutputTypeDef = TypedDict(
-    "TelephonyConfigOutputTypeDef",
-    {
-        "Distributions": List[DistributionTypeDef],
-    },
-)
-
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": Sequence[DistributionTypeDef],
+        "Distributions": List[DistributionTypeDef],
     },
 )
 
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
@@ -5190,19 +4943,17 @@
     "_OptionalS3ConfigTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
-
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": EvaluationAnswerDataTypeDef,
     },
     total=False,
 )
@@ -5262,21 +5013,19 @@
     {
         "ContactAgentId": str,
         "Score": EvaluationScoreTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationMetadataTypeDef(
     _RequiredEvaluationMetadataTypeDef, _OptionalEvaluationMetadataTypeDef
 ):
     pass
 
-
 _RequiredEvaluationSummaryTypeDef = TypedDict(
     "_RequiredEvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
@@ -5290,21 +5039,19 @@
     "_OptionalEvaluationSummaryTypeDef",
     {
         "Score": EvaluationScoreTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationSummaryTypeDef(
     _RequiredEvaluationSummaryTypeDef, _OptionalEvaluationSummaryTypeDef
 ):
     pass
 
-
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetCurrentMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Filters": FiltersTypeDef,
         "CurrentMetrics": Sequence[CurrentMetricTypeDef],
     },
@@ -5316,22 +5063,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SortCriteria": Sequence[CurrentMetricSortCriteriaTypeDef],
     },
     total=False,
 )
 
-
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef = TypedDict(
     "_RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef = TypedDict(
@@ -5339,44 +5084,40 @@
     {
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAgentStatusRequestListAgentStatusesPaginateTypeDef(
     _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef(
     _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListBotsRequestListBotsPaginateTypeDef = TypedDict(
     "_RequiredListBotsRequestListBotsPaginateTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -5384,21 +5125,19 @@
     "_OptionalListBotsRequestListBotsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListBotsRequestListBotsPaginateTypeDef(
     _RequiredListBotsRequestListBotsPaginateTypeDef, _OptionalListBotsRequestListBotsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -5406,22 +5145,20 @@
     "_OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef(
     _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     _OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
@@ -5429,22 +5166,20 @@
     {
         "ContactFlowModuleState": ContactFlowModuleStateType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef(
     _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
@@ -5452,22 +5187,20 @@
     {
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListContactFlowsRequestListContactFlowsPaginateTypeDef(
     _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef,
     _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -5476,22 +5209,20 @@
     "_OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListContactReferencesRequestListContactReferencesPaginateTypeDef(
     _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef,
     _OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
@@ -5499,22 +5230,20 @@
     {
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef(
     _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -5522,88 +5251,80 @@
     "_OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef(
     _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     _OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef(
     _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef(
     _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef(
     _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -5611,22 +5332,20 @@
     "_OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef(
     _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     _OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
 ):
     pass
 
-
 ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
     "ListInstancesRequestListInstancesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -5642,66 +5361,60 @@
     {
         "IntegrationType": IntegrationTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef(
     _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     _OptionalListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef(
     _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListLexBotsRequestListLexBotsPaginateTypeDef = TypedDict(
     "_RequiredListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestListLexBotsPaginateTypeDef = TypedDict(
     "_OptionalListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLexBotsRequestListLexBotsPaginateTypeDef(
     _RequiredListLexBotsRequestListLexBotsPaginateTypeDef,
     _OptionalListLexBotsRequestListLexBotsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
@@ -5710,22 +5423,20 @@
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef(
     _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
 ):
     pass
 
-
 ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef = TypedDict(
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
@@ -5744,22 +5455,20 @@
     "_OptionalListPromptsRequestListPromptsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPromptsRequestListPromptsPaginateTypeDef(
     _RequiredListPromptsRequestListPromptsPaginateTypeDef,
     _OptionalListPromptsRequestListPromptsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -5767,22 +5476,20 @@
     "_OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef(
     _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     _OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
@@ -5790,22 +5497,20 @@
     {
         "QueueTypes": Sequence[QueueTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListQueuesRequestListQueuesPaginateTypeDef(
     _RequiredListQueuesRequestListQueuesPaginateTypeDef,
     _OptionalListQueuesRequestListQueuesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
@@ -5813,22 +5518,20 @@
     {
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListQuickConnectsRequestListQuickConnectsPaginateTypeDef(
     _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -5836,44 +5539,40 @@
     "_OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef(
     _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     _OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef(
     _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
@@ -5882,44 +5581,40 @@
         "PublishStatus": RulePublishStatusType,
         "EventSourceName": EventSourceNameType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSecurityKeysRequestListSecurityKeysPaginateTypeDef(
     _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -5927,44 +5622,40 @@
     "_OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef(
     _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     _OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
     "_OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef(
     _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
     "_RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -5973,22 +5664,20 @@
         "Status": TaskTemplateStatusType,
         "Name": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef(
     _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
 ):
     pass
 
-
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     {
         "InstanceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6005,66 +5694,60 @@
     "_OptionalListUseCasesRequestListUseCasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUseCasesRequestListUseCasesPaginateTypeDef(
     _RequiredListUseCasesRequestListUseCasesPaginateTypeDef,
     _OptionalListUseCasesRequestListUseCasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef(
     _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -6074,22 +5757,20 @@
     {
         "PhoneNumberPrefix": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
@@ -6099,22 +5780,20 @@
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
-
 UpdateContactScheduleRequestRequestTypeDef = TypedDict(
     "UpdateContactScheduleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ScheduledTime": TimestampTypeDef,
     },
@@ -6343,37 +6022,14 @@
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredTaskTemplateFieldOutputTypeDef = TypedDict(
-    "_RequiredTaskTemplateFieldOutputTypeDef",
-    {
-        "Id": TaskTemplateFieldIdentifierTypeDef,
-    },
-)
-_OptionalTaskTemplateFieldOutputTypeDef = TypedDict(
-    "_OptionalTaskTemplateFieldOutputTypeDef",
-    {
-        "Description": str,
-        "Type": TaskTemplateFieldTypeType,
-        "SingleSelectOptions": List[str],
-    },
-    total=False,
-)
-
-
-class TaskTemplateFieldOutputTypeDef(
-    _RequiredTaskTemplateFieldOutputTypeDef, _OptionalTaskTemplateFieldOutputTypeDef
-):
-    pass
-
-
 _RequiredTaskTemplateFieldTypeDef = TypedDict(
     "_RequiredTaskTemplateFieldTypeDef",
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
     },
 )
 _OptionalTaskTemplateFieldTypeDef = TypedDict(
@@ -6382,21 +6038,19 @@
         "Description": str,
         "Type": TaskTemplateFieldTypeType,
         "SingleSelectOptions": Sequence[str],
     },
     total=False,
 )
 
-
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
-
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumberSummaryList": List[PhoneNumberSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6515,59 +6169,24 @@
     {
         "UserSummaryList": List[UserSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricV2OutputTypeDef = TypedDict(
-    "MetricV2OutputTypeDef",
-    {
-        "Name": str,
-        "Threshold": List[ThresholdV2TypeDef],
-        "MetricFilters": List[MetricFilterV2OutputTypeDef],
-    },
-    total=False,
-)
-
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
         "Threshold": Sequence[ThresholdV2TypeDef],
         "MetricFilters": Sequence[MetricFilterV2TypeDef],
     },
     total=False,
 )
 
-_RequiredSendNotificationActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredSendNotificationActionDefinitionOutputTypeDef",
-    {
-        "DeliveryMethod": Literal["EMAIL"],
-        "Content": str,
-        "ContentType": Literal["PLAIN_TEXT"],
-        "Recipient": NotificationRecipientTypeOutputTypeDef,
-    },
-)
-_OptionalSendNotificationActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalSendNotificationActionDefinitionOutputTypeDef",
-    {
-        "Subject": str,
-    },
-    total=False,
-)
-
-
-class SendNotificationActionDefinitionOutputTypeDef(
-    _RequiredSendNotificationActionDefinitionOutputTypeDef,
-    _OptionalSendNotificationActionDefinitionOutputTypeDef,
-):
-    pass
-
-
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -6577,22 +6196,20 @@
     "_OptionalSendNotificationActionDefinitionTypeDef",
     {
         "Subject": str,
     },
     total=False,
 )
 
-
 class SendNotificationActionDefinitionTypeDef(
     _RequiredSendNotificationActionDefinitionTypeDef,
     _OptionalSendNotificationActionDefinitionTypeDef,
 ):
     pass
 
-
 ParticipantTimerConfigurationTypeDef = TypedDict(
     "ParticipantTimerConfigurationTypeDef",
     {
         "ParticipantRole": TimerEligibleParticipantRolesType,
         "TimerType": ParticipantTimerTypeType,
         "TimerValue": ParticipantTimerValueTypeDef,
     },
@@ -6616,21 +6233,19 @@
         "SupportedMessagingContentTypes": Sequence[str],
         "PersistentChat": PersistentChatTypeDef,
         "RelatedContactId": str,
     },
     total=False,
 )
 
-
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 _OptionalQuickConnectConfigTypeDef = TypedDict(
@@ -6639,21 +6254,19 @@
         "UserConfig": UserQuickConnectConfigTypeDef,
         "QueueConfig": QueueQuickConnectConfigTypeDef,
         "PhoneConfig": PhoneNumberQuickConnectConfigTypeDef,
     },
     total=False,
 )
 
-
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
-
 ReferenceSummaryTypeDef = TypedDict(
     "ReferenceSummaryTypeDef",
     {
         "Url": UrlReferenceTypeDef,
         "Attachment": AttachmentReferenceTypeDef,
         "String": StringReferenceTypeDef,
         "Number": NumberReferenceTypeDef,
@@ -6683,44 +6296,19 @@
         "TaskTemplateId": str,
         "QuickConnectId": str,
         "RelatedContactId": str,
     },
     total=False,
 )
 
-
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredTaskActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTaskActionDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "ContactFlowId": str,
-    },
-)
-_OptionalTaskActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTaskActionDefinitionOutputTypeDef",
-    {
-        "Description": str,
-        "References": Dict[str, ReferenceTypeDef],
-    },
-    total=False,
-)
-
-
-class TaskActionDefinitionOutputTypeDef(
-    _RequiredTaskActionDefinitionOutputTypeDef, _OptionalTaskActionDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
     },
 )
@@ -6729,21 +6317,19 @@
     {
         "Description": str,
         "References": Mapping[str, ReferenceTypeDef],
     },
     total=False,
 )
 
-
 class TaskActionDefinitionTypeDef(
     _RequiredTaskActionDefinitionTypeDef, _OptionalTaskActionDefinitionTypeDef
 ):
     pass
 
-
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -6753,21 +6339,19 @@
         "Name": str,
         "Description": str,
         "References": Mapping[str, ReferenceTypeDef],
     },
     total=False,
 )
 
-
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
-
 ResourceTagsSearchCriteriaTypeDef = TypedDict(
     "ResourceTagsSearchCriteriaTypeDef",
     {
         "TagSearchCondition": TagSearchConditionTypeDef,
     },
     total=False,
 )
@@ -6865,22 +6449,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeContactResponseTypeDef = TypedDict(
     "DescribeContactResponseTypeDef",
     {
         "Contact": ContactTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7034,64 +6616,59 @@
     {
         "QueueConfigs": Sequence[RoutingProfileQueueConfigTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "QueueConfigs": Sequence[RoutingProfileQueueConfigTypeDef],
     },
 )
 
 GetTrafficDistributionResponseTypeDef = TypedDict(
     "GetTrafficDistributionResponseTypeDef",
     {
-        "TelephonyConfig": TelephonyConfigOutputTypeDef,
+        "TelephonyConfig": TelephonyConfigTypeDef,
         "Id": str,
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TelephonyConfigUnionTypeDef = Union[TelephonyConfigTypeDef, TelephonyConfigOutputTypeDef]
 _RequiredUpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "TelephonyConfig": TelephonyConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTrafficDistributionRequestRequestTypeDef(
     _RequiredUpdateTrafficDistributionRequestRequestTypeDef,
     _OptionalUpdateTrafficDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
 )
 _OptionalInstanceStorageConfigTypeDef = TypedDict(
@@ -7102,21 +6679,19 @@
         "KinesisVideoStreamConfig": KinesisVideoStreamConfigTypeDef,
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
         "KinesisFirehoseConfig": KinesisFirehoseConfigTypeDef,
     },
     total=False,
 )
 
-
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
-
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -7125,22 +6700,20 @@
     {
         "Answers": Mapping[str, EvaluationAnswerInputTypeDef],
         "Notes": Mapping[str, EvaluationNoteTypeDef],
     },
     total=False,
 )
 
-
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -7149,46 +6722,20 @@
     {
         "Answers": Mapping[str, EvaluationAnswerInputTypeDef],
         "Notes": Mapping[str, EvaluationNoteTypeDef],
     },
     total=False,
 )
 
-
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef",
-    {
-        "MinValue": int,
-        "MaxValue": int,
-    },
-)
-_OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef",
-    {
-        "Options": List[EvaluationFormNumericQuestionOptionTypeDef],
-        "Automation": EvaluationFormNumericQuestionAutomationTypeDef,
-    },
-    total=False,
-)
-
-
-class EvaluationFormNumericQuestionPropertiesOutputTypeDef(
-    _RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef,
-    _OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredEvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
 )
@@ -7197,66 +6744,40 @@
     {
         "Options": Sequence[EvaluationFormNumericQuestionOptionTypeDef],
         "Automation": EvaluationFormNumericQuestionAutomationTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
-
-_RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
-    {
-        "Options": List[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
-    },
-)
-_OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
-    {
-        "DefaultOptionRefId": str,
-    },
-    total=False,
-)
-
-
-class EvaluationFormSingleSelectQuestionAutomationOutputTypeDef(
-    _RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-    _OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-):
-    pass
-
-
 _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "DefaultOptionRefId": str,
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionAutomationTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef,
 ):
     pass
 
-
 _RequiredEvaluationTypeDef = TypedDict(
     "_RequiredEvaluationTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "Metadata": EvaluationMetadataTypeDef,
         "Answers": Dict[str, EvaluationAnswerOutputTypeDef],
@@ -7271,19 +6792,17 @@
     {
         "Scores": Dict[str, EvaluationScoreTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
     pass
 
-
 ListContactEvaluationsResponseTypeDef = TypedDict(
     "ListContactEvaluationsResponseTypeDef",
     {
         "EvaluationSummaryList": List[EvaluationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7349,22 +6868,20 @@
     {
         "Groupings": Sequence[GroupingType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetMetricDataRequestGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataRequestGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataRequestGetMetricDataPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "Filters": FiltersTypeDef,
@@ -7377,21 +6894,19 @@
         "Groupings": Sequence[GroupingType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
-
 HistoricalMetricDataTypeDef = TypedDict(
     "HistoricalMetricDataTypeDef",
     {
         "Metric": HistoricalMetricTypeDef,
         "Value": float,
     },
     total=False,
@@ -7411,22 +6926,20 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-
 HoursOfOperationTypeDef = TypedDict(
     "HoursOfOperationTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "Name": str,
         "Description": str,
@@ -7451,77 +6964,80 @@
         "Description": str,
         "TimeZone": str,
         "Config": Sequence[HoursOfOperationConfigTypeDef],
     },
     total=False,
 )
 
-
 class UpdateHoursOfOperationRequestRequestTypeDef(
     _RequiredUpdateHoursOfOperationRequestRequestTypeDef,
     _OptionalUpdateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInstanceResponseTypeDef = TypedDict(
     "DescribeInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTemplateConstraintsOutputTypeDef = TypedDict(
-    "TaskTemplateConstraintsOutputTypeDef",
-    {
-        "RequiredFields": List[RequiredFieldInfoTypeDef],
-        "ReadOnlyFields": List[ReadOnlyFieldInfoTypeDef],
-        "InvisibleFields": List[InvisibleFieldInfoTypeDef],
-    },
-    total=False,
-)
-
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": Sequence[RequiredFieldInfoTypeDef],
         "ReadOnlyFields": Sequence[ReadOnlyFieldInfoTypeDef],
         "InvisibleFields": Sequence[InvisibleFieldInfoTypeDef],
     },
     total=False,
 )
 
-TaskTemplateDefaultsOutputTypeDef = TypedDict(
-    "TaskTemplateDefaultsOutputTypeDef",
+TaskTemplateDefaultsTypeDef = TypedDict(
+    "TaskTemplateDefaultsTypeDef",
     {
-        "DefaultFieldValues": List[TaskTemplateDefaultFieldValueTypeDef],
+        "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
     },
     total=False,
 )
 
-TaskTemplateDefaultsTypeDef = TypedDict(
-    "TaskTemplateDefaultsTypeDef",
+_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
-        "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
+        "ResourceArn": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2TypeDef],
+    },
+)
+_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataV2RequestRequestTypeDef",
+    {
+        "Groupings": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-TaskTemplateFieldUnionTypeDef = Union[TaskTemplateFieldTypeDef, TaskTemplateFieldOutputTypeDef]
+class GetMetricDataV2RequestRequestTypeDef(
+    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
+):
+    pass
+
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
-        "Metric": MetricV2OutputTypeDef,
+        "Metric": MetricV2TypeDef,
         "Value": float,
     },
     total=False,
 )
 
-MetricV2UnionTypeDef = Union[MetricV2TypeDef, MetricV2OutputTypeDef]
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
 
@@ -7538,22 +7054,20 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
-
 QuickConnectTypeDef = TypedDict(
     "QuickConnectTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "Name": str,
         "Description": str,
@@ -7577,36 +7091,14 @@
     {
         "ReferenceSummaryList": List[ReferenceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRuleActionOutputTypeDef = TypedDict(
-    "_RequiredRuleActionOutputTypeDef",
-    {
-        "ActionType": ActionTypeType,
-    },
-)
-_OptionalRuleActionOutputTypeDef = TypedDict(
-    "_OptionalRuleActionOutputTypeDef",
-    {
-        "TaskAction": TaskActionDefinitionOutputTypeDef,
-        "EventBridgeAction": EventBridgeActionDefinitionTypeDef,
-        "AssignContactCategoryAction": Dict[str, Any],
-        "SendNotificationAction": SendNotificationActionDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RuleActionOutputTypeDef(_RequiredRuleActionOutputTypeDef, _OptionalRuleActionOutputTypeDef):
-    pass
-
-
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalRuleActionTypeDef = TypedDict(
@@ -7616,19 +7108,17 @@
         "EventBridgeAction": EventBridgeActionDefinitionTypeDef,
         "AssignContactCategoryAction": Mapping[str, Any],
         "SendNotificationAction": SendNotificationActionDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
-
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -7638,22 +7128,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SearchCriteria": ResourceTagsSearchCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class SearchResourceTagsRequestRequestTypeDef(
     _RequiredSearchResourceTagsRequestRequestTypeDef,
     _OptionalSearchResourceTagsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
@@ -7662,22 +7150,20 @@
         "ResourceTypes": Sequence[str],
         "SearchCriteria": ResourceTagsSearchCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
-
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "Users": List[UserSearchSummaryTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -7697,22 +7183,20 @@
         "MaxResults": int,
         "SearchFilter": HoursOfOperationSearchFilterTypeDef,
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchHoursOfOperationsRequestRequestTypeDef(
     _RequiredSearchHoursOfOperationsRequestRequestTypeDef,
     _OptionalSearchHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
@@ -7721,22 +7205,20 @@
         "SearchFilter": HoursOfOperationSearchFilterTypeDef,
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -7746,21 +7228,19 @@
         "MaxResults": int,
         "SearchFilter": PromptSearchFilterTypeDef,
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchPromptsRequestRequestTypeDef(
     _RequiredSearchPromptsRequestRequestTypeDef, _OptionalSearchPromptsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
@@ -7769,22 +7249,20 @@
         "SearchFilter": PromptSearchFilterTypeDef,
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -7794,21 +7272,19 @@
         "MaxResults": int,
         "SearchFilter": QueueSearchFilterTypeDef,
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchQueuesRequestRequestTypeDef(
     _RequiredSearchQueuesRequestRequestTypeDef, _OptionalSearchQueuesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
@@ -7817,22 +7293,20 @@
         "SearchFilter": QueueSearchFilterTypeDef,
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -7842,22 +7316,20 @@
         "MaxResults": int,
         "SearchFilter": QuickConnectSearchFilterTypeDef,
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchQuickConnectsRequestRequestTypeDef(
     _RequiredSearchQuickConnectsRequestRequestTypeDef,
     _OptionalSearchQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
@@ -7866,22 +7338,20 @@
         "SearchFilter": QuickConnectSearchFilterTypeDef,
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
@@ -7891,22 +7361,20 @@
         "MaxResults": int,
         "SearchFilter": RoutingProfileSearchFilterTypeDef,
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
     },
     total=False,
 )
 
-
 class SearchRoutingProfilesRequestRequestTypeDef(
     _RequiredSearchRoutingProfilesRequestRequestTypeDef,
     _OptionalSearchRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
@@ -7915,22 +7383,20 @@
         "SearchFilter": RoutingProfileSearchFilterTypeDef,
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -7940,22 +7406,20 @@
         "MaxResults": int,
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": SecurityProfilesSearchFilterTypeDef,
     },
     total=False,
 )
 
-
 class SearchSecurityProfilesRequestRequestTypeDef(
     _RequiredSearchSecurityProfilesRequestRequestTypeDef,
     _OptionalSearchSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
@@ -7964,22 +7428,20 @@
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": SecurityProfilesSearchFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
-
 SearchUsersRequestRequestTypeDef = TypedDict(
     "SearchUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
         "NextToken": str,
         "MaxResults": int,
         "SearchFilter": UserSearchFilterTypeDef,
@@ -8060,37 +7522,14 @@
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": InstanceStorageConfigTypeDef,
     },
 )
 
-_RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
-    {
-        "Options": List[EvaluationFormSingleSelectQuestionOptionTypeDef],
-    },
-)
-_OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
-    {
-        "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
-        "Automation": EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef(
-    _RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
-    _OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
-):
-    pass
-
-
 _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
@@ -8098,22 +7537,20 @@
     {
         "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
         "Automation": EvaluationFormSingleSelectQuestionAutomationTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
-
 DescribeContactEvaluationResponseTypeDef = TypedDict(
     "DescribeContactEvaluationResponseTypeDef",
     {
         "Evaluation": EvaluationTypeDef,
         "EvaluationForm": EvaluationFormContentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8160,65 +7597,20 @@
         "HoursOfOperations": List[HoursOfOperationTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTemplateConstraintsUnionTypeDef = Union[
-    TaskTemplateConstraintsTypeDef, TaskTemplateConstraintsOutputTypeDef
-]
-GetTaskTemplateResponseTypeDef = TypedDict(
-    "GetTaskTemplateResponseTypeDef",
-    {
-        "InstanceId": str,
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsOutputTypeDef,
-        "Defaults": TaskTemplateDefaultsOutputTypeDef,
-        "Fields": List[TaskTemplateFieldOutputTypeDef],
-        "Status": TaskTemplateStatusType,
-        "LastModifiedTime": datetime,
-        "CreatedTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTaskTemplateResponseTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseTypeDef",
-    {
-        "InstanceId": str,
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsOutputTypeDef,
-        "Defaults": TaskTemplateDefaultsOutputTypeDef,
-        "Fields": List[TaskTemplateFieldOutputTypeDef],
-        "Status": TaskTemplateStatusType,
-        "LastModifiedTime": datetime,
-        "CreatedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TaskTemplateDefaultsUnionTypeDef = Union[
-    TaskTemplateDefaultsTypeDef, TaskTemplateDefaultsOutputTypeDef
-]
 _RequiredCreateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskTemplateRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
-        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Fields": Sequence[TaskTemplateFieldTypeDef],
     },
 )
 _OptionalCreateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTaskTemplateRequestRequestTypeDef",
     {
         "Description": str,
         "ContactFlowId": str,
@@ -8226,21 +7618,39 @@
         "Defaults": TaskTemplateDefaultsTypeDef,
         "Status": TaskTemplateStatusType,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
+GetTaskTemplateResponseTypeDef = TypedDict(
+    "GetTaskTemplateResponseTypeDef",
+    {
+        "InstanceId": str,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "Constraints": TaskTemplateConstraintsTypeDef,
+        "Defaults": TaskTemplateDefaultsTypeDef,
+        "Fields": List[TaskTemplateFieldTypeDef],
+        "Status": TaskTemplateStatusType,
+        "LastModifiedTime": datetime,
+        "CreatedTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskTemplateRequestRequestTypeDef",
     {
         "TaskTemplateId": str,
         "InstanceId": str,
     },
@@ -8250,63 +7660,53 @@
     {
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
         "Constraints": TaskTemplateConstraintsTypeDef,
         "Defaults": TaskTemplateDefaultsTypeDef,
         "Status": TaskTemplateStatusType,
-        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Fields": Sequence[TaskTemplateFieldTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
+UpdateTaskTemplateResponseTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseTypeDef",
+    {
+        "InstanceId": str,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "Constraints": TaskTemplateConstraintsTypeDef,
+        "Defaults": TaskTemplateDefaultsTypeDef,
+        "Fields": List[TaskTemplateFieldTypeDef],
+        "Status": TaskTemplateStatusType,
+        "LastModifiedTime": datetime,
+        "CreatedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 MetricResultV2TypeDef = TypedDict(
     "MetricResultV2TypeDef",
     {
         "Dimensions": Dict[str, str],
         "Collections": List[MetricDataV2TypeDef],
     },
     total=False,
 )
 
-_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataV2RequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Filters": Sequence[FilterV2TypeDef],
-        "Metrics": Sequence[MetricV2UnionTypeDef],
-    },
-)
-_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataV2RequestRequestTypeDef",
-    {
-        "Groupings": Sequence[str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetMetricDataV2RequestRequestTypeDef(
-    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
-):
-    pass
-
-
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": ChatParticipantRoleConfigTypeDef,
     },
     total=False,
 )
@@ -8325,50 +7725,74 @@
         "QuickConnects": List[QuickConnectTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
+        "Function": str,
+        "Actions": Sequence[RuleActionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": RuleTriggerEventSourceTypeDef,
         "Function": str,
-        "Actions": List[RuleActionOutputTypeDef],
+        "Actions": List[RuleActionTypeDef],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-
-RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
-EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
-    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+UpdateRuleRequestRequestTypeDef = TypedDict(
+    "UpdateRuleRequestRequestTypeDef",
     {
-        "Numeric": EvaluationFormNumericQuestionPropertiesOutputTypeDef,
-        "SingleSelect": EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
+        "RuleId": str,
+        "InstanceId": str,
+        "Name": str,
+        "Function": str,
+        "Actions": Sequence[RuleActionTypeDef],
+        "PublishStatus": RulePublishStatusType,
     },
-    total=False,
 )
 
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": EvaluationFormNumericQuestionPropertiesTypeDef,
         "SingleSelect": EvaluationFormSingleSelectQuestionPropertiesTypeDef,
@@ -8407,78 +7831,14 @@
     "DescribeRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
-        "Function": str,
-        "Actions": Sequence[RuleActionUnionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-
-UpdateRuleRequestRequestTypeDef = TypedDict(
-    "UpdateRuleRequestRequestTypeDef",
-    {
-        "RuleId": str,
-        "InstanceId": str,
-        "Name": str,
-        "Function": str,
-        "Actions": Sequence[RuleActionUnionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
-
-_RequiredEvaluationFormQuestionOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormQuestionOutputTypeDef",
-    {
-        "Title": str,
-        "RefId": str,
-        "QuestionType": EvaluationFormQuestionTypeType,
-    },
-)
-_OptionalEvaluationFormQuestionOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormQuestionOutputTypeDef",
-    {
-        "Instructions": str,
-        "NotApplicableEnabled": bool,
-        "QuestionTypeProperties": EvaluationFormQuestionTypePropertiesOutputTypeDef,
-        "Weight": float,
-    },
-    total=False,
-)
-
-
-class EvaluationFormQuestionOutputTypeDef(
-    _RequiredEvaluationFormQuestionOutputTypeDef, _OptionalEvaluationFormQuestionOutputTypeDef
-):
-    pass
-
-
 _RequiredEvaluationFormQuestionTypeDef = TypedDict(
     "_RequiredEvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
     },
@@ -8490,30 +7850,19 @@
         "NotApplicableEnabled": bool,
         "QuestionTypeProperties": EvaluationFormQuestionTypePropertiesTypeDef,
         "Weight": float,
     },
     total=False,
 )
 
-
 class EvaluationFormQuestionTypeDef(
     _RequiredEvaluationFormQuestionTypeDef, _OptionalEvaluationFormQuestionTypeDef
 ):
     pass
 
-
-EvaluationFormItemOutputTypeDef = TypedDict(
-    "EvaluationFormItemOutputTypeDef",
-    {
-        "Section": Dict[str, Any],
-        "Question": EvaluationFormQuestionOutputTypeDef,
-    },
-    total=False,
-)
-
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": EvaluationFormQuestionTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect/type_defs.pyi` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionSummaryTypeDef",
     "ActivateEvaluationFormRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "QueueReferenceTypeDef",
     "AgentInfoTypeDef",
     "AgentStatusReferenceTypeDef",
@@ -119,15 +120,14 @@
     "ContactFlowTypeDef",
     "QueueInfoTypeDef",
     "WisdomInfoTypeDef",
     "TagConditionTypeDef",
     "CreateAgentStatusRequestRequestTypeDef",
     "CreateContactFlowModuleRequestRequestTypeDef",
     "CreateContactFlowRequestRequestTypeDef",
-    "EvaluationFormItemUnionTypeDef",
     "EvaluationFormScoringStrategyTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "CreateIntegrationAssociationRequestRequestTypeDef",
     "ParticipantDetailsToAddTypeDef",
     "ParticipantTokenCredentialsTypeDef",
     "CreatePromptRequestRequestTypeDef",
     "OutboundCallerConfigTypeDef",
@@ -201,15 +201,14 @@
     "DismissUserContactRequestRequestTypeDef",
     "DistributionTypeDef",
     "EmailReferenceTypeDef",
     "EncryptionConfigTypeDef",
     "EvaluationAnswerDataTypeDef",
     "NumericQuestionPropertyValueAutomationTypeDef",
     "EvaluationFormNumericQuestionOptionTypeDef",
-    "EvaluationFormSectionOutputTypeDef",
     "EvaluationFormSectionTypeDef",
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionOptionTypeDef",
     "EvaluationFormSummaryTypeDef",
     "EvaluationFormVersionSummaryTypeDef",
     "EvaluationScoreTypeDef",
     "EvaluationNoteTypeDef",
@@ -282,19 +281,17 @@
     "ListTrafficDistributionGroupsRequestRequestTypeDef",
     "TrafficDistributionGroupSummaryTypeDef",
     "ListUseCasesRequestRequestTypeDef",
     "UseCaseTypeDef",
     "ListUserHierarchyGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserSummaryTypeDef",
-    "MetricFilterV2OutputTypeDef",
     "MetricFilterV2TypeDef",
     "ThresholdV2TypeDef",
     "MonitorContactRequestRequestTypeDef",
-    "NotificationRecipientTypeOutputTypeDef",
     "NotificationRecipientTypeTypeDef",
     "NumberReferenceTypeDef",
     "ParticipantDetailsTypeDef",
     "ParticipantTimerValueTypeDef",
     "PersistentChatTypeDef",
     "PhoneNumberQuickConnectConfigTypeDef",
     "PutUserStatusRequestRequestTypeDef",
@@ -433,15 +430,14 @@
     "SearchPromptsResponseTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
     "DescribeTrafficDistributionGroupResponseTypeDef",
     "DescribeVocabularyResponseTypeDef",
     "DimensionsTypeDef",
     "DisassociateRoutingProfileQueuesRequestRequestTypeDef",
     "RoutingProfileQueueConfigTypeDef",
-    "TelephonyConfigOutputTypeDef",
     "TelephonyConfigTypeDef",
     "KinesisVideoStreamConfigTypeDef",
     "S3ConfigTypeDef",
     "EvaluationAnswerInputTypeDef",
     "EvaluationAnswerOutputTypeDef",
     "EvaluationFormNumericQuestionAutomationTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationOptionTypeDef",
@@ -505,15 +501,14 @@
     "InstanceTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIntegrationAssociationsResponseTypeDef",
     "InvisibleFieldInfoTypeDef",
     "ReadOnlyFieldInfoTypeDef",
     "RequiredFieldInfoTypeDef",
     "TaskTemplateDefaultFieldValueTypeDef",
-    "TaskTemplateFieldOutputTypeDef",
     "TaskTemplateFieldTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "ListPhoneNumbersV2ResponseTypeDef",
     "ListPromptsResponseTypeDef",
     "ListQueueQuickConnectsResponseTypeDef",
     "ListQuickConnectsResponseTypeDef",
     "ListQueuesResponseTypeDef",
@@ -521,24 +516,21 @@
     "ListRoutingProfilesResponseTypeDef",
     "ListSecurityKeysResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListTaskTemplatesResponseTypeDef",
     "ListTrafficDistributionGroupsResponseTypeDef",
     "ListUseCasesResponseTypeDef",
     "ListUsersResponseTypeDef",
-    "MetricV2OutputTypeDef",
     "MetricV2TypeDef",
-    "SendNotificationActionDefinitionOutputTypeDef",
     "SendNotificationActionDefinitionTypeDef",
     "ParticipantTimerConfigurationTypeDef",
     "StartChatContactRequestRequestTypeDef",
     "QuickConnectConfigTypeDef",
     "ReferenceSummaryTypeDef",
     "StartTaskContactRequestRequestTypeDef",
-    "TaskActionDefinitionOutputTypeDef",
     "TaskActionDefinitionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ResourceTagsSearchCriteriaTypeDef",
     "SearchResourceTagsResponseTypeDef",
     "SearchSecurityProfilesResponseTypeDef",
     "SearchVocabulariesResponseTypeDef",
     "StartContactRecordingRequestRequestTypeDef",
@@ -562,49 +554,42 @@
     "RoutingProfileTypeDef",
     "UpdateRoutingProfileConcurrencyRequestRequestTypeDef",
     "CurrentMetricResultTypeDef",
     "AssociateRoutingProfileQueuesRequestRequestTypeDef",
     "CreateRoutingProfileRequestRequestTypeDef",
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     "GetTrafficDistributionResponseTypeDef",
-    "TelephonyConfigUnionTypeDef",
     "UpdateTrafficDistributionRequestRequestTypeDef",
     "InstanceStorageConfigTypeDef",
     "SubmitContactEvaluationRequestRequestTypeDef",
     "UpdateContactEvaluationRequestRequestTypeDef",
-    "EvaluationFormNumericQuestionPropertiesOutputTypeDef",
     "EvaluationFormNumericQuestionPropertiesTypeDef",
-    "EvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
     "EvaluationFormSingleSelectQuestionAutomationTypeDef",
     "EvaluationTypeDef",
     "ListContactEvaluationsResponseTypeDef",
     "UserDataTypeDef",
     "HierarchyGroupTypeDef",
     "DescribeUserHierarchyStructureResponseTypeDef",
     "UpdateUserHierarchyStructureRequestRequestTypeDef",
     "GetMetricDataRequestGetMetricDataPaginateTypeDef",
     "GetMetricDataRequestRequestTypeDef",
     "HistoricalMetricDataTypeDef",
     "CreateHoursOfOperationRequestRequestTypeDef",
     "HoursOfOperationTypeDef",
     "UpdateHoursOfOperationRequestRequestTypeDef",
     "DescribeInstanceResponseTypeDef",
-    "TaskTemplateConstraintsOutputTypeDef",
     "TaskTemplateConstraintsTypeDef",
-    "TaskTemplateDefaultsOutputTypeDef",
     "TaskTemplateDefaultsTypeDef",
-    "TaskTemplateFieldUnionTypeDef",
+    "GetMetricDataV2RequestRequestTypeDef",
     "MetricDataV2TypeDef",
-    "MetricV2UnionTypeDef",
     "ChatParticipantRoleConfigTypeDef",
     "CreateQuickConnectRequestRequestTypeDef",
     "QuickConnectTypeDef",
     "UpdateQuickConnectConfigRequestRequestTypeDef",
     "ListContactReferencesResponseTypeDef",
-    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "SearchResourceTagsRequestRequestTypeDef",
     "SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     "SearchUsersResponseTypeDef",
     "SearchHoursOfOperationsRequestRequestTypeDef",
     "SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     "SearchPromptsRequestRequestTypeDef",
@@ -622,46 +607,38 @@
     "DescribeRoutingProfileResponseTypeDef",
     "SearchRoutingProfilesResponseTypeDef",
     "GetCurrentMetricDataResponseTypeDef",
     "AssociateInstanceStorageConfigRequestRequestTypeDef",
     "DescribeInstanceStorageConfigResponseTypeDef",
     "ListInstanceStorageConfigsResponseTypeDef",
     "UpdateInstanceStorageConfigRequestRequestTypeDef",
-    "EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
     "EvaluationFormSingleSelectQuestionPropertiesTypeDef",
     "DescribeContactEvaluationResponseTypeDef",
     "GetCurrentUserDataResponseTypeDef",
     "DescribeUserHierarchyGroupResponseTypeDef",
     "HistoricalMetricResultTypeDef",
     "DescribeHoursOfOperationResponseTypeDef",
     "SearchHoursOfOperationsResponseTypeDef",
-    "TaskTemplateConstraintsUnionTypeDef",
-    "GetTaskTemplateResponseTypeDef",
-    "UpdateTaskTemplateResponseTypeDef",
-    "TaskTemplateDefaultsUnionTypeDef",
     "CreateTaskTemplateRequestRequestTypeDef",
+    "GetTaskTemplateResponseTypeDef",
     "UpdateTaskTemplateRequestRequestTypeDef",
+    "UpdateTaskTemplateResponseTypeDef",
     "MetricResultV2TypeDef",
-    "GetMetricDataV2RequestRequestTypeDef",
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     "DescribeQuickConnectResponseTypeDef",
     "SearchQuickConnectsResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "RuleTypeDef",
-    "RuleActionUnionTypeDef",
-    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+    "UpdateRuleRequestRequestTypeDef",
     "EvaluationFormQuestionTypePropertiesTypeDef",
     "GetMetricDataResponseTypeDef",
     "GetMetricDataV2ResponseTypeDef",
     "UpdateParticipantRoleConfigRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "UpdateRuleRequestRequestTypeDef",
-    "EvaluationFormQuestionOutputTypeDef",
     "EvaluationFormQuestionTypeDef",
-    "EvaluationFormItemOutputTypeDef",
     "EvaluationFormItemTypeDef",
 )
 
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
         "ActionType": ActionTypeType,
@@ -786,20 +763,22 @@
     "_OptionalAssociateDefaultVocabularyRequestRequestTypeDef",
     {
         "VocabularyId": str,
     },
     total=False,
 )
 
+
 class AssociateDefaultVocabularyRequestRequestTypeDef(
     _RequiredAssociateDefaultVocabularyRequestRequestTypeDef,
     _OptionalAssociateDefaultVocabularyRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateLambdaFunctionRequestRequestTypeDef = TypedDict(
     "AssociateLambdaFunctionRequestRequestTypeDef",
     {
         "InstanceId": str,
         "FunctionArn": str,
     },
 )
@@ -887,19 +866,21 @@
         "PhoneNumberDescription": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ClaimPhoneNumberRequestRequestTypeDef(
     _RequiredClaimPhoneNumberRequestRequestTypeDef, _OptionalClaimPhoneNumberRequestRequestTypeDef
 ):
     pass
 
+
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
     total=False,
@@ -1006,19 +987,21 @@
         "Description": str,
         "DisplayOrder": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAgentStatusRequestRequestTypeDef(
     _RequiredCreateAgentStatusRequestRequestTypeDef, _OptionalCreateAgentStatusRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateContactFlowModuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactFlowModuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Content": str,
     },
@@ -1029,20 +1012,22 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateContactFlowModuleRequestRequestTypeDef(
     _RequiredCreateContactFlowModuleRequestRequestTypeDef,
     _OptionalCreateContactFlowModuleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateContactFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactFlowRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "Content": str,
@@ -1053,22 +1038,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateContactFlowRequestRequestTypeDef(
     _RequiredCreateContactFlowRequestRequestTypeDef, _OptionalCreateContactFlowRequestRequestTypeDef
 ):
     pass
 
-EvaluationFormItemUnionTypeDef = Union[
-    "EvaluationFormItemTypeDef", "EvaluationFormItemOutputTypeDef"
-]
+
 EvaluationFormScoringStrategyTypeDef = TypedDict(
     "EvaluationFormScoringStrategyTypeDef",
     {
         "Mode": EvaluationFormScoringModeType,
         "Status": EvaluationFormScoringStatusType,
     },
 )
@@ -1087,19 +1071,21 @@
         "ClientToken": str,
         "InstanceAlias": str,
         "DirectoryId": str,
     },
     total=False,
 )
 
+
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateIntegrationAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationAssociationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
     },
@@ -1111,20 +1097,22 @@
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIntegrationAssociationRequestRequestTypeDef(
     _RequiredCreateIntegrationAssociationRequestRequestTypeDef,
     _OptionalCreateIntegrationAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 ParticipantDetailsToAddTypeDef = TypedDict(
     "ParticipantDetailsToAddTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
         "DisplayName": str,
     },
     total=False,
@@ -1152,19 +1140,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePromptRequestRequestTypeDef(
     _RequiredCreatePromptRequestRequestTypeDef, _OptionalCreatePromptRequestRequestTypeDef
 ):
     pass
 
+
 OutboundCallerConfigTypeDef = TypedDict(
     "OutboundCallerConfigTypeDef",
     {
         "OutboundCallerIdName": str,
         "OutboundCallerIdNumberId": str,
         "OutboundFlowId": str,
     },
@@ -1181,19 +1171,21 @@
     "_OptionalRuleTriggerEventSourceTypeDef",
     {
         "IntegrationAssociationId": str,
     },
     total=False,
 )
 
+
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
+
 _RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileName": str,
         "InstanceId": str,
     },
 )
@@ -1205,20 +1197,22 @@
         "Tags": Mapping[str, str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrafficDistributionGroupRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
     },
 )
@@ -1228,20 +1222,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateTrafficDistributionGroupRequestRequestTypeDef(
     _RequiredCreateTrafficDistributionGroupRequestRequestTypeDef,
     _OptionalCreateTrafficDistributionGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateUseCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUseCaseRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IntegrationAssociationId": str,
         "UseCaseType": UseCaseTypeType,
     },
@@ -1250,19 +1246,21 @@
     "_OptionalCreateUseCaseRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUseCaseRequestRequestTypeDef(
     _RequiredCreateUseCaseRequestRequestTypeDef, _OptionalCreateUseCaseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserHierarchyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserHierarchyGroupRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
     },
 )
@@ -1271,20 +1269,22 @@
     {
         "ParentGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUserHierarchyGroupRequestRequestTypeDef(
     _RequiredCreateUserHierarchyGroupRequestRequestTypeDef,
     _OptionalCreateUserHierarchyGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "Email": str,
         "SecondaryEmail": str,
@@ -1305,17 +1305,19 @@
         "AutoAccept": bool,
         "AfterContactWorkTimeLimit": int,
         "DeskPhoneNumber": str,
     },
     total=False,
 )
 
+
 class UserPhoneConfigTypeDef(_RequiredUserPhoneConfigTypeDef, _OptionalUserPhoneConfigTypeDef):
     pass
 
+
 _RequiredCreateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyRequestRequestTypeDef",
     {
         "InstanceId": str,
         "VocabularyName": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "Content": str,
@@ -1326,19 +1328,21 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
+
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
@@ -1434,20 +1438,22 @@
     "_OptionalDeleteEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
+
 class DeleteEvaluationFormRequestRequestTypeDef(
     _RequiredDeleteEvaluationFormRequestRequestTypeDef,
     _OptionalDeleteEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DeleteHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1598,20 +1604,22 @@
     "_OptionalDescribeEvaluationFormRequestRequestTypeDef",
     {
         "EvaluationFormVersion": int,
     },
     total=False,
 )
 
+
 class DescribeEvaluationFormRequestRequestTypeDef(
     _RequiredDescribeEvaluationFormRequestRequestTypeDef,
     _OptionalDescribeEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeHoursOfOperationRequestRequestTypeDef = TypedDict(
     "DescribeHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "HoursOfOperationId": str,
     },
 )
@@ -1791,17 +1799,19 @@
         "FailureReason": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class VocabularyTypeDef(_RequiredVocabularyTypeDef, _OptionalVocabularyTypeDef):
     pass
 
+
 RoutingProfileReferenceTypeDef = TypedDict(
     "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
     total=False,
@@ -1937,41 +1947,21 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
+
 class EvaluationFormNumericQuestionOptionTypeDef(
     _RequiredEvaluationFormNumericQuestionOptionTypeDef,
     _OptionalEvaluationFormNumericQuestionOptionTypeDef,
 ):
     pass
 
-_RequiredEvaluationFormSectionOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSectionOutputTypeDef",
-    {
-        "Title": str,
-        "RefId": str,
-        "Items": List[Dict[str, Any]],
-    },
-)
-_OptionalEvaluationFormSectionOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSectionOutputTypeDef",
-    {
-        "Instructions": str,
-        "Weight": float,
-    },
-    total=False,
-)
-
-class EvaluationFormSectionOutputTypeDef(
-    _RequiredEvaluationFormSectionOutputTypeDef, _OptionalEvaluationFormSectionOutputTypeDef
-):
-    pass
 
 _RequiredEvaluationFormSectionTypeDef = TypedDict(
     "_RequiredEvaluationFormSectionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "Items": Sequence[Dict[str, Any]],
@@ -1982,19 +1972,21 @@
     {
         "Instructions": str,
         "Weight": float,
     },
     total=False,
 )
 
+
 class EvaluationFormSectionTypeDef(
     _RequiredEvaluationFormSectionTypeDef, _OptionalEvaluationFormSectionTypeDef
 ):
     pass
 
+
 SingleSelectQuestionRuleCategoryAutomationTypeDef = TypedDict(
     "SingleSelectQuestionRuleCategoryAutomationTypeDef",
     {
         "Category": str,
         "Condition": SingleSelectQuestionRuleCategoryAutomationConditionType,
         "OptionRefId": str,
     },
@@ -2012,20 +2004,22 @@
     {
         "Score": int,
         "AutomaticFail": bool,
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionOptionTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionOptionTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionOptionTypeDef,
 ):
     pass
 
+
 _RequiredEvaluationFormSummaryTypeDef = TypedDict(
     "_RequiredEvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
@@ -2041,19 +2035,21 @@
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
         "ActiveVersion": int,
     },
     total=False,
 )
 
+
 class EvaluationFormSummaryTypeDef(
     _RequiredEvaluationFormSummaryTypeDef, _OptionalEvaluationFormSummaryTypeDef
 ):
     pass
 
+
 EvaluationFormVersionSummaryTypeDef = TypedDict(
     "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
@@ -2154,19 +2150,21 @@
     "_OptionalGetTaskTemplateRequestRequestTypeDef",
     {
         "SnapshotVersion": str,
     },
     total=False,
 )
 
+
 class GetTaskTemplateRequestRequestTypeDef(
     _RequiredGetTaskTemplateRequestRequestTypeDef, _OptionalGetTaskTemplateRequestRequestTypeDef
 ):
     pass
 
+
 GetTrafficDistributionRequestRequestTypeDef = TypedDict(
     "GetTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -2326,19 +2324,21 @@
         "NextToken": str,
         "MaxResults": int,
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
     },
     total=False,
 )
 
+
 class ListAgentStatusRequestRequestTypeDef(
     _RequiredListAgentStatusRequestRequestTypeDef, _OptionalListAgentStatusRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListApprovedOriginsRequestRequestTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestRequestTypeDef = TypedDict(
@@ -2346,20 +2346,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListApprovedOriginsRequestRequestTypeDef(
     _RequiredListApprovedOriginsRequestRequestTypeDef,
     _OptionalListApprovedOriginsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -2368,19 +2370,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListBotsRequestRequestTypeDef(
     _RequiredListBotsRequestRequestTypeDef, _OptionalListBotsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListContactEvaluationsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -2388,20 +2392,22 @@
     "_OptionalListContactEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactEvaluationsRequestRequestTypeDef(
     _RequiredListContactEvaluationsRequestRequestTypeDef,
     _OptionalListContactEvaluationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowModulesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestRequestTypeDef = TypedDict(
@@ -2410,20 +2416,22 @@
         "NextToken": str,
         "MaxResults": int,
         "ContactFlowModuleState": ContactFlowModuleStateType,
     },
     total=False,
 )
 
+
 class ListContactFlowModulesRequestRequestTypeDef(
     _RequiredListContactFlowModulesRequestRequestTypeDef,
     _OptionalListContactFlowModulesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestRequestTypeDef = TypedDict(
@@ -2432,19 +2440,21 @@
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListContactFlowsRequestRequestTypeDef(
     _RequiredListContactFlowsRequestRequestTypeDef, _OptionalListContactFlowsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListContactReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -2453,20 +2463,22 @@
     "_OptionalListContactReferencesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactReferencesRequestRequestTypeDef(
     _RequiredListContactReferencesRequestRequestTypeDef,
     _OptionalListContactReferencesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestRequestTypeDef = TypedDict(
@@ -2475,20 +2487,22 @@
         "LanguageCode": VocabularyLanguageCodeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDefaultVocabulariesRequestRequestTypeDef(
     _RequiredListDefaultVocabulariesRequestRequestTypeDef,
     _OptionalListDefaultVocabulariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -2497,20 +2511,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEvaluationFormVersionsRequestRequestTypeDef(
     _RequiredListEvaluationFormVersionsRequestRequestTypeDef,
     _OptionalListEvaluationFormVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormsRequestRequestTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestRequestTypeDef = TypedDict(
@@ -2518,20 +2534,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEvaluationFormsRequestRequestTypeDef(
     _RequiredListEvaluationFormsRequestRequestTypeDef,
     _OptionalListEvaluationFormsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListHoursOfOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestRequestTypeDef = TypedDict(
@@ -2539,20 +2557,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListHoursOfOperationsRequestRequestTypeDef(
     _RequiredListHoursOfOperationsRequestRequestTypeDef,
     _OptionalListHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestRequestTypeDef = TypedDict(
@@ -2560,20 +2580,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstanceAttributesRequestRequestTypeDef(
     _RequiredListInstanceAttributesRequestRequestTypeDef,
     _OptionalListInstanceAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceStorageConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -2582,20 +2604,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInstanceStorageConfigsRequestRequestTypeDef(
     _RequiredListInstanceStorageConfigsRequestRequestTypeDef,
     _OptionalListInstanceStorageConfigsRequestRequestTypeDef,
 ):
     pass
 
+
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2613,20 +2637,22 @@
         "IntegrationType": IntegrationTypeType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLambdaFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestRequestTypeDef = TypedDict(
@@ -2634,20 +2660,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLambdaFunctionsRequestRequestTypeDef(
     _RequiredListLambdaFunctionsRequestRequestTypeDef,
     _OptionalListLambdaFunctionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLexBotsRequestRequestTypeDef = TypedDict(
     "_RequiredListLexBotsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestRequestTypeDef = TypedDict(
@@ -2655,19 +2683,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLexBotsRequestRequestTypeDef(
     _RequiredListLexBotsRequestRequestTypeDef, _OptionalListLexBotsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListPhoneNumbersRequestRequestTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestRequestTypeDef = TypedDict(
@@ -2677,19 +2707,21 @@
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPhoneNumbersRequestRequestTypeDef(
     _RequiredListPhoneNumbersRequestRequestTypeDef, _OptionalListPhoneNumbersRequestRequestTypeDef
 ):
     pass
 
+
 PhoneNumberSummaryTypeDef = TypedDict(
     "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
@@ -2735,19 +2767,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPromptsRequestRequestTypeDef(
     _RequiredListPromptsRequestRequestTypeDef, _OptionalListPromptsRequestRequestTypeDef
 ):
     pass
 
+
 PromptSummaryTypeDef = TypedDict(
     "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -2766,20 +2800,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListQueueQuickConnectsRequestRequestTypeDef(
     _RequiredListQueueQuickConnectsRequestRequestTypeDef,
     _OptionalListQueueQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
+
 QuickConnectSummaryTypeDef = TypedDict(
     "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
@@ -2799,19 +2835,21 @@
         "QueueTypes": Sequence[QueueTypeType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListQueuesRequestRequestTypeDef(
     _RequiredListQueuesRequestRequestTypeDef, _OptionalListQueuesRequestRequestTypeDef
 ):
     pass
 
+
 QueueSummaryTypeDef = TypedDict(
     "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
@@ -2831,19 +2869,21 @@
         "NextToken": str,
         "MaxResults": int,
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
     },
     total=False,
 )
 
+
 class ListQuickConnectsRequestRequestTypeDef(
     _RequiredListQuickConnectsRequestRequestTypeDef, _OptionalListQuickConnectsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -2852,20 +2892,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListRoutingProfileQueuesRequestRequestTypeDef(
     _RequiredListRoutingProfileQueuesRequestRequestTypeDef,
     _OptionalListRoutingProfileQueuesRequestRequestTypeDef,
 ):
     pass
 
+
 RoutingProfileQueueConfigSummaryTypeDef = TypedDict(
     "RoutingProfileQueueConfigSummaryTypeDef",
     {
         "QueueId": str,
         "QueueArn": str,
         "QueueName": str,
         "Priority": int,
@@ -2885,20 +2927,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListRoutingProfilesRequestRequestTypeDef(
     _RequiredListRoutingProfilesRequestRequestTypeDef,
     _OptionalListRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 RoutingProfileSummaryTypeDef = TypedDict(
     "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -2918,19 +2962,21 @@
         "EventSourceName": EventSourceNameType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListSecurityKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestRequestTypeDef = TypedDict(
@@ -2938,19 +2984,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityKeysRequestRequestTypeDef(
     _RequiredListSecurityKeysRequestRequestTypeDef, _OptionalListSecurityKeysRequestRequestTypeDef
 ):
     pass
 
+
 SecurityKeyTypeDef = TypedDict(
     "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
@@ -2969,20 +3017,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityProfilePermissionsRequestRequestTypeDef(
     _RequiredListSecurityProfilePermissionsRequestRequestTypeDef,
     _OptionalListSecurityProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -2990,20 +3040,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListSecurityProfilesRequestRequestTypeDef(
     _RequiredListSecurityProfilesRequestRequestTypeDef,
     _OptionalListSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 SecurityProfileSummaryTypeDef = TypedDict(
     "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
@@ -3030,19 +3082,21 @@
         "MaxResults": int,
         "Status": TaskTemplateStatusType,
         "Name": str,
     },
     total=False,
 )
 
+
 class ListTaskTemplatesRequestRequestTypeDef(
     _RequiredListTaskTemplatesRequestRequestTypeDef, _OptionalListTaskTemplatesRequestRequestTypeDef
 ):
     pass
 
+
 TaskTemplateMetadataTypeDef = TypedDict(
     "TaskTemplateMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
@@ -3087,19 +3141,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUseCasesRequestRequestTypeDef(
     _RequiredListUseCasesRequestRequestTypeDef, _OptionalListUseCasesRequestRequestTypeDef
 ):
     pass
 
+
 UseCaseTypeDef = TypedDict(
     "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
@@ -3117,20 +3173,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUserHierarchyGroupsRequestRequestTypeDef(
     _RequiredListUserHierarchyGroupsRequestRequestTypeDef,
     _OptionalListUserHierarchyGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -3138,38 +3196,31 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 UserSummaryTypeDef = TypedDict(
     "UserSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
     },
     total=False,
 )
 
-MetricFilterV2OutputTypeDef = TypedDict(
-    "MetricFilterV2OutputTypeDef",
-    {
-        "MetricFilterKey": str,
-        "MetricFilterValues": List[str],
-    },
-    total=False,
-)
-
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
     },
     total=False,
@@ -3197,27 +3248,20 @@
     {
         "AllowedMonitorCapabilities": Sequence[MonitorCapabilityType],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class MonitorContactRequestRequestTypeDef(
     _RequiredMonitorContactRequestRequestTypeDef, _OptionalMonitorContactRequestRequestTypeDef
 ):
     pass
 
-NotificationRecipientTypeOutputTypeDef = TypedDict(
-    "NotificationRecipientTypeOutputTypeDef",
-    {
-        "UserTags": Dict[str, str],
-        "UserIds": List[str],
-    },
-    total=False,
-)
 
 NotificationRecipientTypeTypeDef = TypedDict(
     "NotificationRecipientTypeTypeDef",
     {
         "UserTags": Mapping[str, str],
         "UserIds": Sequence[str],
     },
@@ -3326,20 +3370,22 @@
     "_OptionalReleasePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ReleasePhoneNumberRequestRequestTypeDef(
     _RequiredReleasePhoneNumberRequestRequestTypeDef,
     _OptionalReleasePhoneNumberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredReplicateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ReplicaRegion": str,
         "ReplicaAlias": str,
     },
@@ -3348,19 +3394,21 @@
     "_OptionalReplicateInstanceRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ReplicateInstanceRequestRequestTypeDef(
     _RequiredReplicateInstanceRequestRequestTypeDef, _OptionalReplicateInstanceRequestRequestTypeDef
 ):
     pass
 
+
 TagSearchConditionTypeDef = TypedDict(
     "TagSearchConditionTypeDef",
     {
         "tagKey": str,
         "tagValue": str,
         "tagKeyComparisonType": StringComparisonTypeType,
         "tagValueComparisonType": StringComparisonTypeType,
@@ -3391,20 +3439,22 @@
         "PhoneNumberPrefix": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchAvailablePhoneNumbersRequestRequestTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestRequestTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestRequestTypeDef,
 ):
     pass
 
+
 TagSetTypeDef = TypedDict(
     "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -3437,20 +3487,22 @@
         "State": VocabularyStateType,
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
     },
     total=False,
 )
 
+
 class SearchVocabulariesRequestRequestTypeDef(
     _RequiredSearchVocabulariesRequestRequestTypeDef,
     _OptionalSearchVocabulariesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredVocabularySummaryTypeDef = TypedDict(
     "_RequiredVocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
@@ -3462,19 +3514,21 @@
     "_OptionalVocabularySummaryTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
+
 class VocabularySummaryTypeDef(
     _RequiredVocabularySummaryTypeDef, _OptionalVocabularySummaryTypeDef
 ):
     pass
 
+
 _RequiredStartContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "EvaluationFormId": str,
     },
@@ -3483,20 +3537,22 @@
     "_OptionalStartContactEvaluationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartContactEvaluationRequestRequestTypeDef(
     _RequiredStartContactEvaluationRequestRequestTypeDef,
     _OptionalStartContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
+
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
@@ -3558,19 +3614,21 @@
         "QueueId": str,
         "UserId": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class TransferContactRequestRequestTypeDef(
     _RequiredTransferContactRequestRequestTypeDef, _OptionalTransferContactRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -3590,19 +3648,21 @@
         "State": AgentStatusStateType,
         "DisplayOrder": int,
         "ResetOrderNumber": bool,
     },
     total=False,
 )
 
+
 class UpdateAgentStatusRequestRequestTypeDef(
     _RequiredUpdateAgentStatusRequestRequestTypeDef, _OptionalUpdateAgentStatusRequestRequestTypeDef
 ):
     pass
 
+
 UpdateContactAttributesRequestRequestTypeDef = TypedDict(
     "UpdateContactAttributesRequestRequestTypeDef",
     {
         "InitialContactId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -3630,20 +3690,22 @@
         "Name": str,
         "Description": str,
         "ContactFlowState": ContactFlowStateType,
     },
     total=False,
 )
 
+
 class UpdateContactFlowMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateContactFlowModuleContentRequestRequestTypeDef = TypedDict(
     "UpdateContactFlowModuleContentRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowModuleId": str,
         "Content": str,
     },
@@ -3662,20 +3724,22 @@
         "Name": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
     },
     total=False,
 )
 
+
 class UpdateContactFlowModuleMetadataRequestRequestTypeDef(
     _RequiredUpdateContactFlowModuleMetadataRequestRequestTypeDef,
     _OptionalUpdateContactFlowModuleMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContactFlowNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactFlowNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactFlowId": str,
     },
 )
@@ -3684,20 +3748,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateContactFlowNameRequestRequestTypeDef(
     _RequiredUpdateContactFlowNameRequestRequestTypeDef,
     _OptionalUpdateContactFlowNameRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateInstanceAttributeRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAttributeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
@@ -3714,19 +3780,21 @@
     "_OptionalUpdatePhoneNumberRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePromptRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
@@ -3736,19 +3804,21 @@
         "Name": str,
         "Description": str,
         "S3Uri": str,
     },
     total=False,
 )
 
+
 class UpdatePromptRequestRequestTypeDef(
     _RequiredUpdatePromptRequestRequestTypeDef, _OptionalUpdatePromptRequestRequestTypeDef
 ):
     pass
 
+
 UpdateQueueHoursOfOperationRequestRequestTypeDef = TypedDict(
     "UpdateQueueHoursOfOperationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "HoursOfOperationId": str,
     },
@@ -3765,20 +3835,22 @@
     "_OptionalUpdateQueueMaxContactsRequestRequestTypeDef",
     {
         "MaxContacts": int,
     },
     total=False,
 )
 
+
 class UpdateQueueMaxContactsRequestRequestTypeDef(
     _RequiredUpdateQueueMaxContactsRequestRequestTypeDef,
     _OptionalUpdateQueueMaxContactsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateQueueNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueNameRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -3787,19 +3859,21 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateQueueNameRequestRequestTypeDef(
     _RequiredUpdateQueueNameRequestRequestTypeDef, _OptionalUpdateQueueNameRequestRequestTypeDef
 ):
     pass
 
+
 UpdateQueueStatusRequestRequestTypeDef = TypedDict(
     "UpdateQueueStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
         "Status": QueueStatusType,
     },
@@ -3817,20 +3891,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateQuickConnectNameRequestRequestTypeDef(
     _RequiredUpdateQuickConnectNameRequestRequestTypeDef,
     _OptionalUpdateQuickConnectNameRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "DefaultOutboundQueueId": str,
     },
@@ -3848,20 +3924,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateRoutingProfileNameRequestRequestTypeDef(
     _RequiredUpdateRoutingProfileNameRequestRequestTypeDef,
     _OptionalUpdateRoutingProfileNameRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -3872,20 +3950,22 @@
         "Permissions": Sequence[str],
         "AllowedAccessControlTags": Mapping[str, str],
         "TagRestrictedResources": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateUserHierarchyGroupNameRequestRequestTypeDef = TypedDict(
     "UpdateUserHierarchyGroupNameRequestRequestTypeDef",
     {
         "Name": str,
         "HierarchyGroupId": str,
         "InstanceId": str,
     },
@@ -3902,20 +3982,22 @@
     "_OptionalUpdateUserHierarchyRequestRequestTypeDef",
     {
         "HierarchyGroupId": str,
     },
     total=False,
 )
 
+
 class UpdateUserHierarchyRequestRequestTypeDef(
     _RequiredUpdateUserHierarchyRequestRequestTypeDef,
     _OptionalUpdateUserHierarchyRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateUserRoutingProfileRequestRequestTypeDef = TypedDict(
     "UpdateUserRoutingProfileRequestRequestTypeDef",
     {
         "RoutingProfileId": str,
         "UserId": str,
         "InstanceId": str,
     },
@@ -4413,20 +4495,22 @@
         "AnswerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "CampaignId": str,
         "TrafficType": TrafficTypeType,
     },
     total=False,
 )
 
+
 class StartOutboundVoiceContactRequestRequestTypeDef(
     _RequiredStartOutboundVoiceContactRequestRequestTypeDef,
     _OptionalStartOutboundVoiceContactRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateLexBotRequestRequestTypeDef = TypedDict(
     "AssociateLexBotRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LexBot": LexBotTypeDef,
     },
 )
@@ -4451,19 +4535,21 @@
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
 )
 
+
 class AssociateBotRequestRequestTypeDef(
     _RequiredAssociateBotRequestRequestTypeDef, _OptionalAssociateBotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDisassociateBotRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateBotRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDisassociateBotRequestRequestTypeDef = TypedDict(
@@ -4471,19 +4557,21 @@
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
 )
 
+
 class DisassociateBotRequestRequestTypeDef(
     _RequiredDisassociateBotRequestRequestTypeDef, _OptionalDisassociateBotRequestRequestTypeDef
 ):
     pass
 
+
 LexBotConfigTypeDef = TypedDict(
     "LexBotConfigTypeDef",
     {
         "LexBot": LexBotTypeDef,
         "LexV2Bot": LexV2BotTypeDef,
     },
     total=False,
@@ -4621,67 +4709,71 @@
 )
 
 _RequiredCreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Title": str,
-        "Items": Sequence[EvaluationFormItemUnionTypeDef],
+        "Items": Sequence["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalCreateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEvaluationFormRequestRequestTypeDef",
     {
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateEvaluationFormRequestRequestTypeDef(
     _RequiredCreateEvaluationFormRequestRequestTypeDef,
     _OptionalCreateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredEvaluationFormContentTypeDef = TypedDict(
     "_RequiredEvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Items": List["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalEvaluationFormContentTypeDef = TypedDict(
     "_OptionalEvaluationFormContentTypeDef",
     {
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationFormContentTypeDef(
     _RequiredEvaluationFormContentTypeDef, _OptionalEvaluationFormContentTypeDef
 ):
     pass
 
+
 _RequiredEvaluationFormTypeDef = TypedDict(
     "_RequiredEvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
         "Status": EvaluationFormVersionStatusType,
-        "Items": List["EvaluationFormItemOutputTypeDef"],
+        "Items": List["EvaluationFormItemTypeDef"],
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 _OptionalEvaluationFormTypeDef = TypedDict(
@@ -4690,44 +4782,48 @@
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class EvaluationFormTypeDef(_RequiredEvaluationFormTypeDef, _OptionalEvaluationFormTypeDef):
     pass
 
+
 _RequiredUpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Title": str,
-        "Items": Sequence[EvaluationFormItemUnionTypeDef],
+        "Items": Sequence["EvaluationFormItemTypeDef"],
     },
 )
 _OptionalUpdateEvaluationFormRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEvaluationFormRequestRequestTypeDef",
     {
         "CreateNewVersion": bool,
         "Description": str,
         "ScoringStrategy": EvaluationFormScoringStrategyTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdateEvaluationFormRequestRequestTypeDef(
     _RequiredUpdateEvaluationFormRequestRequestTypeDef,
     _OptionalUpdateEvaluationFormRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateParticipantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParticipantRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ParticipantDetails": ParticipantDetailsToAddTypeDef,
     },
@@ -4736,19 +4832,21 @@
     "_OptionalCreateParticipantRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateParticipantRequestRequestTypeDef(
     _RequiredCreateParticipantRequestRequestTypeDef, _OptionalCreateParticipantRequestRequestTypeDef
 ):
     pass
 
+
 CreateParticipantResponseTypeDef = TypedDict(
     "CreateParticipantResponseTypeDef",
     {
         "ParticipantCredentials": ParticipantTokenCredentialsTypeDef,
         "ParticipantId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4770,19 +4868,21 @@
         "MaxContacts": int,
         "QuickConnectIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
+
 QueueTypeDef = TypedDict(
     "QueueTypeDef",
     {
         "Name": str,
         "QueueArn": str,
         "QueueId": str,
         "Description": str,
@@ -4831,19 +4931,21 @@
         "DirectoryUserId": str,
         "HierarchyGroupId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 UpdateUserPhoneConfigRequestRequestTypeDef = TypedDict(
     "UpdateUserPhoneConfigRequestRequestTypeDef",
     {
         "PhoneConfig": UserPhoneConfigTypeDef,
         "UserId": str,
         "InstanceId": str,
     },
@@ -4888,17 +4990,19 @@
     "_OptionalMediaConcurrencyTypeDef",
     {
         "CrossChannelBehavior": CrossChannelBehaviorTypeDef,
     },
     total=False,
 )
 
+
 class MediaConcurrencyTypeDef(_RequiredMediaConcurrencyTypeDef, _OptionalMediaConcurrencyTypeDef):
     pass
 
+
 CurrentMetricDataTypeDef = TypedDict(
     "CurrentMetricDataTypeDef",
     {
         "Metric": CurrentMetricTypeDef,
         "Value": float,
     },
     total=False,
@@ -4979,25 +5083,18 @@
     {
         "QueueReference": RoutingProfileQueueReferenceTypeDef,
         "Priority": int,
         "Delay": int,
     },
 )
 
-TelephonyConfigOutputTypeDef = TypedDict(
-    "TelephonyConfigOutputTypeDef",
-    {
-        "Distributions": List[DistributionTypeDef],
-    },
-)
-
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
-        "Distributions": Sequence[DistributionTypeDef],
+        "Distributions": List[DistributionTypeDef],
     },
 )
 
 KinesisVideoStreamConfigTypeDef = TypedDict(
     "KinesisVideoStreamConfigTypeDef",
     {
         "Prefix": str,
@@ -5017,17 +5114,19 @@
     "_OptionalS3ConfigTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3ConfigTypeDef(_RequiredS3ConfigTypeDef, _OptionalS3ConfigTypeDef):
     pass
 
+
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": EvaluationAnswerDataTypeDef,
     },
     total=False,
 )
@@ -5087,19 +5186,21 @@
     {
         "ContactAgentId": str,
         "Score": EvaluationScoreTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationMetadataTypeDef(
     _RequiredEvaluationMetadataTypeDef, _OptionalEvaluationMetadataTypeDef
 ):
     pass
 
+
 _RequiredEvaluationSummaryTypeDef = TypedDict(
     "_RequiredEvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
@@ -5113,19 +5214,21 @@
     "_OptionalEvaluationSummaryTypeDef",
     {
         "Score": EvaluationScoreTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationSummaryTypeDef(
     _RequiredEvaluationSummaryTypeDef, _OptionalEvaluationSummaryTypeDef
 ):
     pass
 
+
 _RequiredGetCurrentMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetCurrentMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Filters": FiltersTypeDef,
         "CurrentMetrics": Sequence[CurrentMetricTypeDef],
     },
@@ -5137,20 +5240,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SortCriteria": Sequence[CurrentMetricSortCriteriaTypeDef],
     },
     total=False,
 )
 
+
 class GetCurrentMetricDataRequestRequestTypeDef(
     _RequiredGetCurrentMetricDataRequestRequestTypeDef,
     _OptionalGetCurrentMetricDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef = TypedDict(
     "_RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef = TypedDict(
@@ -5158,40 +5263,44 @@
     {
         "AgentStatusTypes": Sequence[AgentStatusTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAgentStatusRequestListAgentStatusesPaginateTypeDef(
     _RequiredListAgentStatusRequestListAgentStatusesPaginateTypeDef,
     _OptionalListAgentStatusRequestListAgentStatusesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef = TypedDict(
     "_OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef(
     _RequiredListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
     _OptionalListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListBotsRequestListBotsPaginateTypeDef = TypedDict(
     "_RequiredListBotsRequestListBotsPaginateTypeDef",
     {
         "InstanceId": str,
         "LexVersion": LexVersionType,
     },
 )
@@ -5199,19 +5308,21 @@
     "_OptionalListBotsRequestListBotsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListBotsRequestListBotsPaginateTypeDef(
     _RequiredListBotsRequestListBotsPaginateTypeDef, _OptionalListBotsRequestListBotsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef = TypedDict(
     "_RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -5219,20 +5330,22 @@
     "_OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef(
     _RequiredListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
     _OptionalListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef = TypedDict(
@@ -5240,20 +5353,22 @@
     {
         "ContactFlowModuleState": ContactFlowModuleStateType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef(
     _RequiredListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
     _OptionalListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
     "_RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef = TypedDict(
@@ -5261,20 +5376,22 @@
     {
         "ContactFlowTypes": Sequence[ContactFlowTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListContactFlowsRequestListContactFlowsPaginateTypeDef(
     _RequiredListContactFlowsRequestListContactFlowsPaginateTypeDef,
     _OptionalListContactFlowsRequestListContactFlowsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef = TypedDict(
     "_RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ReferenceTypes": Sequence[ReferenceTypeType],
     },
@@ -5283,20 +5400,22 @@
     "_OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListContactReferencesRequestListContactReferencesPaginateTypeDef(
     _RequiredListContactReferencesRequestListContactReferencesPaginateTypeDef,
     _OptionalListContactReferencesRequestListContactReferencesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef = TypedDict(
@@ -5304,20 +5423,22 @@
     {
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef(
     _RequiredListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
     _OptionalListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
     },
 )
@@ -5325,80 +5446,88 @@
     "_OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef(
     _RequiredListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
     _OptionalListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef = TypedDict(
     "_OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef(
     _RequiredListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
     _OptionalListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef = TypedDict(
     "_OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef(
     _RequiredListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
     _OptionalListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef = TypedDict(
     "_OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef(
     _RequiredListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
     _OptionalListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef = TypedDict(
     "_RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "InstanceId": str,
         "ResourceType": InstanceStorageResourceTypeType,
     },
 )
@@ -5406,20 +5535,22 @@
     "_OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef(
     _RequiredListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
     _OptionalListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef,
 ):
     pass
 
+
 ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
     "ListInstancesRequestListInstancesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -5435,60 +5566,66 @@
     {
         "IntegrationType": IntegrationTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef(
     _RequiredListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
     _OptionalListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef = TypedDict(
     "_OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef(
     _RequiredListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
     _OptionalListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListLexBotsRequestListLexBotsPaginateTypeDef = TypedDict(
     "_RequiredListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListLexBotsRequestListLexBotsPaginateTypeDef = TypedDict(
     "_OptionalListLexBotsRequestListLexBotsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLexBotsRequestListLexBotsPaginateTypeDef(
     _RequiredListLexBotsRequestListLexBotsPaginateTypeDef,
     _OptionalListLexBotsRequestListLexBotsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef = TypedDict(
@@ -5497,20 +5634,22 @@
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef(
     _RequiredListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
     _OptionalListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef,
 ):
     pass
 
+
 ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef = TypedDict(
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
         "PhoneNumberTypes": Sequence[PhoneNumberTypeType],
         "PhoneNumberPrefix": str,
@@ -5529,20 +5668,22 @@
     "_OptionalListPromptsRequestListPromptsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPromptsRequestListPromptsPaginateTypeDef(
     _RequiredListPromptsRequestListPromptsPaginateTypeDef,
     _OptionalListPromptsRequestListPromptsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
         "QueueId": str,
     },
 )
@@ -5550,20 +5691,22 @@
     "_OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef(
     _RequiredListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
     _OptionalListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
     "_RequiredListQueuesRequestListQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
@@ -5571,20 +5714,22 @@
     {
         "QueueTypes": Sequence[QueueTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListQueuesRequestListQueuesPaginateTypeDef(
     _RequiredListQueuesRequestListQueuesPaginateTypeDef,
     _OptionalListQueuesRequestListQueuesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef = TypedDict(
@@ -5592,20 +5737,22 @@
     {
         "QuickConnectTypes": Sequence[QuickConnectTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListQuickConnectsRequestListQuickConnectsPaginateTypeDef(
     _RequiredListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
     _OptionalListQuickConnectsRequestListQuickConnectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
     },
 )
@@ -5613,40 +5760,44 @@
     "_OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef(
     _RequiredListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
     _OptionalListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef = TypedDict(
     "_OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef(
     _RequiredListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
     _OptionalListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
@@ -5655,40 +5806,44 @@
         "PublishStatus": RulePublishStatusType,
         "EventSourceName": EventSourceNameType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef = TypedDict(
     "_OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSecurityKeysRequestListSecurityKeysPaginateTypeDef(
     _RequiredListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
     _OptionalListSecurityKeysRequestListSecurityKeysPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "SecurityProfileId": str,
         "InstanceId": str,
     },
 )
@@ -5696,40 +5851,44 @@
     "_OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef(
     _RequiredListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
     _OptionalListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
     "_OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef(
     _RequiredListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     _OptionalListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
     "_RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef = TypedDict(
@@ -5738,20 +5897,22 @@
         "Status": TaskTemplateStatusType,
         "Name": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef(
     _RequiredListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
     _OptionalListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef,
 ):
     pass
 
+
 ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef = TypedDict(
     "ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef",
     {
         "InstanceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -5768,60 +5929,66 @@
     "_OptionalListUseCasesRequestListUseCasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUseCasesRequestListUseCasesPaginateTypeDef(
     _RequiredListUseCasesRequestListUseCasesPaginateTypeDef,
     _OptionalListUseCasesRequestListUseCasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef = TypedDict(
     "_OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef(
     _RequiredListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
     _OptionalListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef = TypedDict(
     "_RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
@@ -5831,20 +5998,22 @@
     {
         "PhoneNumberPrefix": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(
     _RequiredSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
     _OptionalSearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
     "_RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef = TypedDict(
@@ -5854,20 +6023,22 @@
         "NameStartsWith": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(
     _RequiredSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
     _OptionalSearchVocabulariesRequestSearchVocabulariesPaginateTypeDef,
 ):
     pass
 
+
 UpdateContactScheduleRequestRequestTypeDef = TypedDict(
     "UpdateContactScheduleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
         "ScheduledTime": TimestampTypeDef,
     },
@@ -6096,35 +6267,14 @@
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredTaskTemplateFieldOutputTypeDef = TypedDict(
-    "_RequiredTaskTemplateFieldOutputTypeDef",
-    {
-        "Id": TaskTemplateFieldIdentifierTypeDef,
-    },
-)
-_OptionalTaskTemplateFieldOutputTypeDef = TypedDict(
-    "_OptionalTaskTemplateFieldOutputTypeDef",
-    {
-        "Description": str,
-        "Type": TaskTemplateFieldTypeType,
-        "SingleSelectOptions": List[str],
-    },
-    total=False,
-)
-
-class TaskTemplateFieldOutputTypeDef(
-    _RequiredTaskTemplateFieldOutputTypeDef, _OptionalTaskTemplateFieldOutputTypeDef
-):
-    pass
-
 _RequiredTaskTemplateFieldTypeDef = TypedDict(
     "_RequiredTaskTemplateFieldTypeDef",
     {
         "Id": TaskTemplateFieldIdentifierTypeDef,
     },
 )
 _OptionalTaskTemplateFieldTypeDef = TypedDict(
@@ -6133,19 +6283,21 @@
         "Description": str,
         "Type": TaskTemplateFieldTypeType,
         "SingleSelectOptions": Sequence[str],
     },
     total=False,
 )
 
+
 class TaskTemplateFieldTypeDef(
     _RequiredTaskTemplateFieldTypeDef, _OptionalTaskTemplateFieldTypeDef
 ):
     pass
 
+
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumberSummaryList": List[PhoneNumberSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6264,57 +6416,24 @@
     {
         "UserSummaryList": List[UserSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricV2OutputTypeDef = TypedDict(
-    "MetricV2OutputTypeDef",
-    {
-        "Name": str,
-        "Threshold": List[ThresholdV2TypeDef],
-        "MetricFilters": List[MetricFilterV2OutputTypeDef],
-    },
-    total=False,
-)
-
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
         "Threshold": Sequence[ThresholdV2TypeDef],
         "MetricFilters": Sequence[MetricFilterV2TypeDef],
     },
     total=False,
 )
 
-_RequiredSendNotificationActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredSendNotificationActionDefinitionOutputTypeDef",
-    {
-        "DeliveryMethod": Literal["EMAIL"],
-        "Content": str,
-        "ContentType": Literal["PLAIN_TEXT"],
-        "Recipient": NotificationRecipientTypeOutputTypeDef,
-    },
-)
-_OptionalSendNotificationActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalSendNotificationActionDefinitionOutputTypeDef",
-    {
-        "Subject": str,
-    },
-    total=False,
-)
-
-class SendNotificationActionDefinitionOutputTypeDef(
-    _RequiredSendNotificationActionDefinitionOutputTypeDef,
-    _OptionalSendNotificationActionDefinitionOutputTypeDef,
-):
-    pass
-
 _RequiredSendNotificationActionDefinitionTypeDef = TypedDict(
     "_RequiredSendNotificationActionDefinitionTypeDef",
     {
         "DeliveryMethod": Literal["EMAIL"],
         "Content": str,
         "ContentType": Literal["PLAIN_TEXT"],
         "Recipient": NotificationRecipientTypeTypeDef,
@@ -6324,20 +6443,22 @@
     "_OptionalSendNotificationActionDefinitionTypeDef",
     {
         "Subject": str,
     },
     total=False,
 )
 
+
 class SendNotificationActionDefinitionTypeDef(
     _RequiredSendNotificationActionDefinitionTypeDef,
     _OptionalSendNotificationActionDefinitionTypeDef,
 ):
     pass
 
+
 ParticipantTimerConfigurationTypeDef = TypedDict(
     "ParticipantTimerConfigurationTypeDef",
     {
         "ParticipantRole": TimerEligibleParticipantRolesType,
         "TimerType": ParticipantTimerTypeType,
         "TimerValue": ParticipantTimerValueTypeDef,
     },
@@ -6361,19 +6482,21 @@
         "SupportedMessagingContentTypes": Sequence[str],
         "PersistentChat": PersistentChatTypeDef,
         "RelatedContactId": str,
     },
     total=False,
 )
 
+
 class StartChatContactRequestRequestTypeDef(
     _RequiredStartChatContactRequestRequestTypeDef, _OptionalStartChatContactRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
     },
 )
 _OptionalQuickConnectConfigTypeDef = TypedDict(
@@ -6382,19 +6505,21 @@
         "UserConfig": UserQuickConnectConfigTypeDef,
         "QueueConfig": QueueQuickConnectConfigTypeDef,
         "PhoneConfig": PhoneNumberQuickConnectConfigTypeDef,
     },
     total=False,
 )
 
+
 class QuickConnectConfigTypeDef(
     _RequiredQuickConnectConfigTypeDef, _OptionalQuickConnectConfigTypeDef
 ):
     pass
 
+
 ReferenceSummaryTypeDef = TypedDict(
     "ReferenceSummaryTypeDef",
     {
         "Url": UrlReferenceTypeDef,
         "Attachment": AttachmentReferenceTypeDef,
         "String": StringReferenceTypeDef,
         "Number": NumberReferenceTypeDef,
@@ -6424,39 +6549,20 @@
         "TaskTemplateId": str,
         "QuickConnectId": str,
         "RelatedContactId": str,
     },
     total=False,
 )
 
+
 class StartTaskContactRequestRequestTypeDef(
     _RequiredStartTaskContactRequestRequestTypeDef, _OptionalStartTaskContactRequestRequestTypeDef
 ):
     pass
 
-_RequiredTaskActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTaskActionDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "ContactFlowId": str,
-    },
-)
-_OptionalTaskActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTaskActionDefinitionOutputTypeDef",
-    {
-        "Description": str,
-        "References": Dict[str, ReferenceTypeDef],
-    },
-    total=False,
-)
-
-class TaskActionDefinitionOutputTypeDef(
-    _RequiredTaskActionDefinitionOutputTypeDef, _OptionalTaskActionDefinitionOutputTypeDef
-):
-    pass
 
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
     },
@@ -6466,19 +6572,21 @@
     {
         "Description": str,
         "References": Mapping[str, ReferenceTypeDef],
     },
     total=False,
 )
 
+
 class TaskActionDefinitionTypeDef(
     _RequiredTaskActionDefinitionTypeDef, _OptionalTaskActionDefinitionTypeDef
 ):
     pass
 
+
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
     },
 )
@@ -6488,19 +6596,21 @@
         "Name": str,
         "Description": str,
         "References": Mapping[str, ReferenceTypeDef],
     },
     total=False,
 )
 
+
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
+
 ResourceTagsSearchCriteriaTypeDef = TypedDict(
     "ResourceTagsSearchCriteriaTypeDef",
     {
         "TagSearchCondition": TagSearchConditionTypeDef,
     },
     total=False,
 )
@@ -6598,20 +6708,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetCurrentUserDataRequestRequestTypeDef(
     _RequiredGetCurrentUserDataRequestRequestTypeDef,
     _OptionalGetCurrentUserDataRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeContactResponseTypeDef = TypedDict(
     "DescribeContactResponseTypeDef",
     {
         "Contact": ContactTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6765,60 +6877,63 @@
     {
         "QueueConfigs": Sequence[RoutingProfileQueueConfigTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRoutingProfileRequestRequestTypeDef(
     _RequiredCreateRoutingProfileRequestRequestTypeDef,
     _OptionalCreateRoutingProfileRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRoutingProfileQueuesRequestRequestTypeDef = TypedDict(
     "UpdateRoutingProfileQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RoutingProfileId": str,
         "QueueConfigs": Sequence[RoutingProfileQueueConfigTypeDef],
     },
 )
 
 GetTrafficDistributionResponseTypeDef = TypedDict(
     "GetTrafficDistributionResponseTypeDef",
     {
-        "TelephonyConfig": TelephonyConfigOutputTypeDef,
+        "TelephonyConfig": TelephonyConfigTypeDef,
         "Id": str,
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TelephonyConfigUnionTypeDef = Union[TelephonyConfigTypeDef, TelephonyConfigOutputTypeDef]
 _RequiredUpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateTrafficDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrafficDistributionRequestRequestTypeDef",
     {
         "TelephonyConfig": TelephonyConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTrafficDistributionRequestRequestTypeDef(
     _RequiredUpdateTrafficDistributionRequestRequestTypeDef,
     _OptionalUpdateTrafficDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
 )
 _OptionalInstanceStorageConfigTypeDef = TypedDict(
@@ -6829,19 +6944,21 @@
         "KinesisVideoStreamConfig": KinesisVideoStreamConfigTypeDef,
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
         "KinesisFirehoseConfig": KinesisFirehoseConfigTypeDef,
     },
     total=False,
 )
 
+
 class InstanceStorageConfigTypeDef(
     _RequiredInstanceStorageConfigTypeDef, _OptionalInstanceStorageConfigTypeDef
 ):
     pass
 
+
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -6850,20 +6967,22 @@
     {
         "Answers": Mapping[str, EvaluationAnswerInputTypeDef],
         "Notes": Mapping[str, EvaluationNoteTypeDef],
     },
     total=False,
 )
 
+
 class SubmitContactEvaluationRequestRequestTypeDef(
     _RequiredSubmitContactEvaluationRequestRequestTypeDef,
     _OptionalSubmitContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
     },
 )
@@ -6872,41 +6991,21 @@
     {
         "Answers": Mapping[str, EvaluationAnswerInputTypeDef],
         "Notes": Mapping[str, EvaluationNoteTypeDef],
     },
     total=False,
 )
 
+
 class UpdateContactEvaluationRequestRequestTypeDef(
     _RequiredUpdateContactEvaluationRequestRequestTypeDef,
     _OptionalUpdateContactEvaluationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef",
-    {
-        "MinValue": int,
-        "MaxValue": int,
-    },
-)
-_OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef",
-    {
-        "Options": List[EvaluationFormNumericQuestionOptionTypeDef],
-        "Automation": EvaluationFormNumericQuestionAutomationTypeDef,
-    },
-    total=False,
-)
-
-class EvaluationFormNumericQuestionPropertiesOutputTypeDef(
-    _RequiredEvaluationFormNumericQuestionPropertiesOutputTypeDef,
-    _OptionalEvaluationFormNumericQuestionPropertiesOutputTypeDef,
-):
-    pass
 
 _RequiredEvaluationFormNumericQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormNumericQuestionPropertiesTypeDef",
     {
         "MinValue": int,
         "MaxValue": int,
     },
@@ -6916,39 +7015,21 @@
     {
         "Options": Sequence[EvaluationFormNumericQuestionOptionTypeDef],
         "Automation": EvaluationFormNumericQuestionAutomationTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationFormNumericQuestionPropertiesTypeDef(
     _RequiredEvaluationFormNumericQuestionPropertiesTypeDef,
     _OptionalEvaluationFormNumericQuestionPropertiesTypeDef,
 ):
     pass
 
-_RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
-    {
-        "Options": List[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
-    },
-)
-_OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef",
-    {
-        "DefaultOptionRefId": str,
-    },
-    total=False,
-)
-
-class EvaluationFormSingleSelectQuestionAutomationOutputTypeDef(
-    _RequiredEvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-    _OptionalEvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-):
-    pass
 
 _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],
     },
 )
@@ -6956,20 +7037,22 @@
     "_OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef",
     {
         "DefaultOptionRefId": str,
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionAutomationTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionAutomationTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionAutomationTypeDef,
 ):
     pass
 
+
 _RequiredEvaluationTypeDef = TypedDict(
     "_RequiredEvaluationTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "Metadata": EvaluationMetadataTypeDef,
         "Answers": Dict[str, EvaluationAnswerOutputTypeDef],
@@ -6984,17 +7067,19 @@
     {
         "Scores": Dict[str, EvaluationScoreTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
     pass
 
+
 ListContactEvaluationsResponseTypeDef = TypedDict(
     "ListContactEvaluationsResponseTypeDef",
     {
         "EvaluationSummaryList": List[EvaluationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7060,20 +7145,22 @@
     {
         "Groupings": Sequence[GroupingType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetMetricDataRequestGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataRequestGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataRequestGetMetricDataPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetMetricDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetMetricDataRequestRequestTypeDef",
     {
         "InstanceId": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "Filters": FiltersTypeDef,
@@ -7086,19 +7173,21 @@
         "Groupings": Sequence[GroupingType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetMetricDataRequestRequestTypeDef(
     _RequiredGetMetricDataRequestRequestTypeDef, _OptionalGetMetricDataRequestRequestTypeDef
 ):
     pass
 
+
 HistoricalMetricDataTypeDef = TypedDict(
     "HistoricalMetricDataTypeDef",
     {
         "Metric": HistoricalMetricTypeDef,
         "Value": float,
     },
     total=False,
@@ -7118,20 +7207,22 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateHoursOfOperationRequestRequestTypeDef(
     _RequiredCreateHoursOfOperationRequestRequestTypeDef,
     _OptionalCreateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
+
 HoursOfOperationTypeDef = TypedDict(
     "HoursOfOperationTypeDef",
     {
         "HoursOfOperationId": str,
         "HoursOfOperationArn": str,
         "Name": str,
         "Description": str,
@@ -7156,75 +7247,84 @@
         "Description": str,
         "TimeZone": str,
         "Config": Sequence[HoursOfOperationConfigTypeDef],
     },
     total=False,
 )
 
+
 class UpdateHoursOfOperationRequestRequestTypeDef(
     _RequiredUpdateHoursOfOperationRequestRequestTypeDef,
     _OptionalUpdateHoursOfOperationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInstanceResponseTypeDef = TypedDict(
     "DescribeInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTemplateConstraintsOutputTypeDef = TypedDict(
-    "TaskTemplateConstraintsOutputTypeDef",
-    {
-        "RequiredFields": List[RequiredFieldInfoTypeDef],
-        "ReadOnlyFields": List[ReadOnlyFieldInfoTypeDef],
-        "InvisibleFields": List[InvisibleFieldInfoTypeDef],
-    },
-    total=False,
-)
-
 TaskTemplateConstraintsTypeDef = TypedDict(
     "TaskTemplateConstraintsTypeDef",
     {
         "RequiredFields": Sequence[RequiredFieldInfoTypeDef],
         "ReadOnlyFields": Sequence[ReadOnlyFieldInfoTypeDef],
         "InvisibleFields": Sequence[InvisibleFieldInfoTypeDef],
     },
     total=False,
 )
 
-TaskTemplateDefaultsOutputTypeDef = TypedDict(
-    "TaskTemplateDefaultsOutputTypeDef",
+TaskTemplateDefaultsTypeDef = TypedDict(
+    "TaskTemplateDefaultsTypeDef",
     {
-        "DefaultFieldValues": List[TaskTemplateDefaultFieldValueTypeDef],
+        "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
     },
     total=False,
 )
 
-TaskTemplateDefaultsTypeDef = TypedDict(
-    "TaskTemplateDefaultsTypeDef",
+_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataV2RequestRequestTypeDef",
     {
-        "DefaultFieldValues": Sequence[TaskTemplateDefaultFieldValueTypeDef],
+        "ResourceArn": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Filters": Sequence[FilterV2TypeDef],
+        "Metrics": Sequence[MetricV2TypeDef],
+    },
+)
+_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataV2RequestRequestTypeDef",
+    {
+        "Groupings": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-TaskTemplateFieldUnionTypeDef = Union[TaskTemplateFieldTypeDef, TaskTemplateFieldOutputTypeDef]
+
+class GetMetricDataV2RequestRequestTypeDef(
+    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
+):
+    pass
+
+
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
-        "Metric": MetricV2OutputTypeDef,
+        "Metric": MetricV2TypeDef,
         "Value": float,
     },
     total=False,
 )
 
-MetricV2UnionTypeDef = Union[MetricV2TypeDef, MetricV2OutputTypeDef]
 ChatParticipantRoleConfigTypeDef = TypedDict(
     "ChatParticipantRoleConfigTypeDef",
     {
         "ParticipantTimerConfigList": Sequence[ParticipantTimerConfigurationTypeDef],
     },
 )
 
@@ -7241,20 +7341,22 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQuickConnectRequestRequestTypeDef(
     _RequiredCreateQuickConnectRequestRequestTypeDef,
     _OptionalCreateQuickConnectRequestRequestTypeDef,
 ):
     pass
 
+
 QuickConnectTypeDef = TypedDict(
     "QuickConnectTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "Name": str,
         "Description": str,
@@ -7278,34 +7380,14 @@
     {
         "ReferenceSummaryList": List[ReferenceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRuleActionOutputTypeDef = TypedDict(
-    "_RequiredRuleActionOutputTypeDef",
-    {
-        "ActionType": ActionTypeType,
-    },
-)
-_OptionalRuleActionOutputTypeDef = TypedDict(
-    "_OptionalRuleActionOutputTypeDef",
-    {
-        "TaskAction": TaskActionDefinitionOutputTypeDef,
-        "EventBridgeAction": EventBridgeActionDefinitionTypeDef,
-        "AssignContactCategoryAction": Dict[str, Any],
-        "SendNotificationAction": SendNotificationActionDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
-class RuleActionOutputTypeDef(_RequiredRuleActionOutputTypeDef, _OptionalRuleActionOutputTypeDef):
-    pass
-
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalRuleActionTypeDef = TypedDict(
@@ -7315,17 +7397,19 @@
         "EventBridgeAction": EventBridgeActionDefinitionTypeDef,
         "AssignContactCategoryAction": Mapping[str, Any],
         "SendNotificationAction": SendNotificationActionDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class RuleActionTypeDef(_RequiredRuleActionTypeDef, _OptionalRuleActionTypeDef):
     pass
 
+
 _RequiredSearchResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestRequestTypeDef = TypedDict(
@@ -7335,20 +7419,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SearchCriteria": ResourceTagsSearchCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class SearchResourceTagsRequestRequestTypeDef(
     _RequiredSearchResourceTagsRequestRequestTypeDef,
     _OptionalSearchResourceTagsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
     "_RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef = TypedDict(
@@ -7357,20 +7443,22 @@
         "ResourceTypes": Sequence[str],
         "SearchCriteria": ResourceTagsSearchCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(
     _RequiredSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
     _OptionalSearchResourceTagsRequestSearchResourceTagsPaginateTypeDef,
 ):
     pass
 
+
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "Users": List[UserSearchSummaryTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -7390,20 +7478,22 @@
         "MaxResults": int,
         "SearchFilter": HoursOfOperationSearchFilterTypeDef,
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchHoursOfOperationsRequestRequestTypeDef(
     _RequiredSearchHoursOfOperationsRequestRequestTypeDef,
     _OptionalSearchHoursOfOperationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
     "_RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef = TypedDict(
@@ -7412,20 +7502,22 @@
         "SearchFilter": HoursOfOperationSearchFilterTypeDef,
         "SearchCriteria": "HoursOfOperationSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(
     _RequiredSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
     _OptionalSearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchPromptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestRequestTypeDef = TypedDict(
@@ -7435,19 +7527,21 @@
         "MaxResults": int,
         "SearchFilter": PromptSearchFilterTypeDef,
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchPromptsRequestRequestTypeDef(
     _RequiredSearchPromptsRequestRequestTypeDef, _OptionalSearchPromptsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
     "_RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef = TypedDict(
@@ -7456,20 +7550,22 @@
         "SearchFilter": PromptSearchFilterTypeDef,
         "SearchCriteria": "PromptSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchPromptsRequestSearchPromptsPaginateTypeDef(
     _RequiredSearchPromptsRequestSearchPromptsPaginateTypeDef,
     _OptionalSearchPromptsRequestSearchPromptsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestRequestTypeDef = TypedDict(
@@ -7479,19 +7575,21 @@
         "MaxResults": int,
         "SearchFilter": QueueSearchFilterTypeDef,
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchQueuesRequestRequestTypeDef(
     _RequiredSearchQueuesRequestRequestTypeDef, _OptionalSearchQueuesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
     "_RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef = TypedDict(
@@ -7500,20 +7598,22 @@
         "SearchFilter": QueueSearchFilterTypeDef,
         "SearchCriteria": "QueueSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchQueuesRequestSearchQueuesPaginateTypeDef(
     _RequiredSearchQueuesRequestSearchQueuesPaginateTypeDef,
     _OptionalSearchQueuesRequestSearchQueuesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuickConnectsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestRequestTypeDef = TypedDict(
@@ -7523,20 +7623,22 @@
         "MaxResults": int,
         "SearchFilter": QuickConnectSearchFilterTypeDef,
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchQuickConnectsRequestRequestTypeDef(
     _RequiredSearchQuickConnectsRequestRequestTypeDef,
     _OptionalSearchQuickConnectsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
     "_RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef = TypedDict(
@@ -7545,20 +7647,22 @@
         "SearchFilter": QuickConnectSearchFilterTypeDef,
         "SearchCriteria": "QuickConnectSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(
     _RequiredSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
     _OptionalSearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestRequestTypeDef = TypedDict(
@@ -7568,20 +7672,22 @@
         "MaxResults": int,
         "SearchFilter": RoutingProfileSearchFilterTypeDef,
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
     },
     total=False,
 )
 
+
 class SearchRoutingProfilesRequestRequestTypeDef(
     _RequiredSearchRoutingProfilesRequestRequestTypeDef,
     _OptionalSearchRoutingProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef = TypedDict(
@@ -7590,20 +7696,22 @@
         "SearchFilter": RoutingProfileSearchFilterTypeDef,
         "SearchCriteria": "RoutingProfileSearchCriteriaTypeDef",
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(
     _RequiredSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
     _OptionalSearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestRequestTypeDef = TypedDict(
@@ -7613,20 +7721,22 @@
         "MaxResults": int,
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": SecurityProfilesSearchFilterTypeDef,
     },
     total=False,
 )
 
+
 class SearchSecurityProfilesRequestRequestTypeDef(
     _RequiredSearchSecurityProfilesRequestRequestTypeDef,
     _OptionalSearchSecurityProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
     "_RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef = TypedDict(
@@ -7635,20 +7745,22 @@
         "SearchCriteria": "SecurityProfileSearchCriteriaTypeDef",
         "SearchFilter": SecurityProfilesSearchFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(
     _RequiredSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
     _OptionalSearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef,
 ):
     pass
 
+
 SearchUsersRequestRequestTypeDef = TypedDict(
     "SearchUsersRequestRequestTypeDef",
     {
         "InstanceId": str,
         "NextToken": str,
         "MaxResults": int,
         "SearchFilter": UserSearchFilterTypeDef,
@@ -7729,35 +7841,14 @@
         "InstanceId": str,
         "AssociationId": str,
         "ResourceType": InstanceStorageResourceTypeType,
         "StorageConfig": InstanceStorageConfigTypeDef,
     },
 )
 
-_RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
-    {
-        "Options": List[EvaluationFormSingleSelectQuestionOptionTypeDef],
-    },
-)
-_OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef",
-    {
-        "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
-        "Automation": EvaluationFormSingleSelectQuestionAutomationOutputTypeDef,
-    },
-    total=False,
-)
-
-class EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef(
-    _RequiredEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
-    _OptionalEvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
     "_RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef",
     {
         "Options": Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],
     },
 )
 _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef = TypedDict(
@@ -7765,20 +7856,22 @@
     {
         "DisplayAs": EvaluationFormSingleSelectQuestionDisplayModeType,
         "Automation": EvaluationFormSingleSelectQuestionAutomationTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
+
 DescribeContactEvaluationResponseTypeDef = TypedDict(
     "DescribeContactEvaluationResponseTypeDef",
     {
         "Evaluation": EvaluationTypeDef,
         "EvaluationForm": EvaluationFormContentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7825,65 +7918,20 @@
         "HoursOfOperations": List[HoursOfOperationTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTemplateConstraintsUnionTypeDef = Union[
-    TaskTemplateConstraintsTypeDef, TaskTemplateConstraintsOutputTypeDef
-]
-GetTaskTemplateResponseTypeDef = TypedDict(
-    "GetTaskTemplateResponseTypeDef",
-    {
-        "InstanceId": str,
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsOutputTypeDef,
-        "Defaults": TaskTemplateDefaultsOutputTypeDef,
-        "Fields": List[TaskTemplateFieldOutputTypeDef],
-        "Status": TaskTemplateStatusType,
-        "LastModifiedTime": datetime,
-        "CreatedTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTaskTemplateResponseTypeDef = TypedDict(
-    "UpdateTaskTemplateResponseTypeDef",
-    {
-        "InstanceId": str,
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "ContactFlowId": str,
-        "Constraints": TaskTemplateConstraintsOutputTypeDef,
-        "Defaults": TaskTemplateDefaultsOutputTypeDef,
-        "Fields": List[TaskTemplateFieldOutputTypeDef],
-        "Status": TaskTemplateStatusType,
-        "LastModifiedTime": datetime,
-        "CreatedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TaskTemplateDefaultsUnionTypeDef = Union[
-    TaskTemplateDefaultsTypeDef, TaskTemplateDefaultsOutputTypeDef
-]
 _RequiredCreateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskTemplateRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Name": str,
-        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Fields": Sequence[TaskTemplateFieldTypeDef],
     },
 )
 _OptionalCreateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTaskTemplateRequestRequestTypeDef",
     {
         "Description": str,
         "ContactFlowId": str,
@@ -7891,20 +7939,42 @@
         "Defaults": TaskTemplateDefaultsTypeDef,
         "Status": TaskTemplateStatusType,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateTaskTemplateRequestRequestTypeDef(
     _RequiredCreateTaskTemplateRequestRequestTypeDef,
     _OptionalCreateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
+
+GetTaskTemplateResponseTypeDef = TypedDict(
+    "GetTaskTemplateResponseTypeDef",
+    {
+        "InstanceId": str,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "Constraints": TaskTemplateConstraintsTypeDef,
+        "Defaults": TaskTemplateDefaultsTypeDef,
+        "Fields": List[TaskTemplateFieldTypeDef],
+        "Status": TaskTemplateStatusType,
+        "LastModifiedTime": datetime,
+        "CreatedTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateTaskTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskTemplateRequestRequestTypeDef",
     {
         "TaskTemplateId": str,
         "InstanceId": str,
     },
 )
@@ -7913,59 +7983,55 @@
     {
         "Name": str,
         "Description": str,
         "ContactFlowId": str,
         "Constraints": TaskTemplateConstraintsTypeDef,
         "Defaults": TaskTemplateDefaultsTypeDef,
         "Status": TaskTemplateStatusType,
-        "Fields": Sequence[TaskTemplateFieldUnionTypeDef],
+        "Fields": Sequence[TaskTemplateFieldTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTaskTemplateRequestRequestTypeDef(
     _RequiredUpdateTaskTemplateRequestRequestTypeDef,
     _OptionalUpdateTaskTemplateRequestRequestTypeDef,
 ):
     pass
 
-MetricResultV2TypeDef = TypedDict(
-    "MetricResultV2TypeDef",
-    {
-        "Dimensions": Dict[str, str],
-        "Collections": List[MetricDataV2TypeDef],
-    },
-    total=False,
-)
 
-_RequiredGetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataV2RequestRequestTypeDef",
+UpdateTaskTemplateResponseTypeDef = TypedDict(
+    "UpdateTaskTemplateResponseTypeDef",
     {
-        "ResourceArn": str,
-        "StartTime": TimestampTypeDef,
-        "EndTime": TimestampTypeDef,
-        "Filters": Sequence[FilterV2TypeDef],
-        "Metrics": Sequence[MetricV2UnionTypeDef],
+        "InstanceId": str,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "ContactFlowId": str,
+        "Constraints": TaskTemplateConstraintsTypeDef,
+        "Defaults": TaskTemplateDefaultsTypeDef,
+        "Fields": List[TaskTemplateFieldTypeDef],
+        "Status": TaskTemplateStatusType,
+        "LastModifiedTime": datetime,
+        "CreatedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGetMetricDataV2RequestRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataV2RequestRequestTypeDef",
+
+MetricResultV2TypeDef = TypedDict(
+    "MetricResultV2TypeDef",
     {
-        "Groupings": Sequence[str],
-        "NextToken": str,
-        "MaxResults": int,
+        "Dimensions": Dict[str, str],
+        "Collections": List[MetricDataV2TypeDef],
     },
     total=False,
 )
 
-class GetMetricDataV2RequestRequestTypeDef(
-    _RequiredGetMetricDataV2RequestRequestTypeDef, _OptionalGetMetricDataV2RequestRequestTypeDef
-):
-    pass
-
 UpdateParticipantRoleConfigChannelInfoTypeDef = TypedDict(
     "UpdateParticipantRoleConfigChannelInfoTypeDef",
     {
         "Chat": ChatParticipantRoleConfigTypeDef,
     },
     total=False,
 )
@@ -7984,48 +8050,78 @@
         "QuickConnects": List[QuickConnectTypeDef],
         "NextToken": str,
         "ApproximateTotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
+        "Function": str,
+        "Actions": Sequence[RuleActionTypeDef],
+        "PublishStatus": RulePublishStatusType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": RuleTriggerEventSourceTypeDef,
         "Function": str,
-        "Actions": List[RuleActionOutputTypeDef],
+        "Actions": List[RuleActionTypeDef],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
 )
 _OptionalRuleTypeDef = TypedDict(
     "_OptionalRuleTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
-EvaluationFormQuestionTypePropertiesOutputTypeDef = TypedDict(
-    "EvaluationFormQuestionTypePropertiesOutputTypeDef",
+
+UpdateRuleRequestRequestTypeDef = TypedDict(
+    "UpdateRuleRequestRequestTypeDef",
     {
-        "Numeric": EvaluationFormNumericQuestionPropertiesOutputTypeDef,
-        "SingleSelect": EvaluationFormSingleSelectQuestionPropertiesOutputTypeDef,
+        "RuleId": str,
+        "InstanceId": str,
+        "Name": str,
+        "Function": str,
+        "Actions": Sequence[RuleActionTypeDef],
+        "PublishStatus": RulePublishStatusType,
     },
-    total=False,
 )
 
 EvaluationFormQuestionTypePropertiesTypeDef = TypedDict(
     "EvaluationFormQuestionTypePropertiesTypeDef",
     {
         "Numeric": EvaluationFormNumericQuestionPropertiesTypeDef,
         "SingleSelect": EvaluationFormSingleSelectQuestionPropertiesTypeDef,
@@ -8064,74 +8160,14 @@
     "DescribeRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-        "TriggerEventSource": RuleTriggerEventSourceTypeDef,
-        "Function": str,
-        "Actions": Sequence[RuleActionUnionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-UpdateRuleRequestRequestTypeDef = TypedDict(
-    "UpdateRuleRequestRequestTypeDef",
-    {
-        "RuleId": str,
-        "InstanceId": str,
-        "Name": str,
-        "Function": str,
-        "Actions": Sequence[RuleActionUnionTypeDef],
-        "PublishStatus": RulePublishStatusType,
-    },
-)
-
-_RequiredEvaluationFormQuestionOutputTypeDef = TypedDict(
-    "_RequiredEvaluationFormQuestionOutputTypeDef",
-    {
-        "Title": str,
-        "RefId": str,
-        "QuestionType": EvaluationFormQuestionTypeType,
-    },
-)
-_OptionalEvaluationFormQuestionOutputTypeDef = TypedDict(
-    "_OptionalEvaluationFormQuestionOutputTypeDef",
-    {
-        "Instructions": str,
-        "NotApplicableEnabled": bool,
-        "QuestionTypeProperties": EvaluationFormQuestionTypePropertiesOutputTypeDef,
-        "Weight": float,
-    },
-    total=False,
-)
-
-class EvaluationFormQuestionOutputTypeDef(
-    _RequiredEvaluationFormQuestionOutputTypeDef, _OptionalEvaluationFormQuestionOutputTypeDef
-):
-    pass
-
 _RequiredEvaluationFormQuestionTypeDef = TypedDict(
     "_RequiredEvaluationFormQuestionTypeDef",
     {
         "Title": str,
         "RefId": str,
         "QuestionType": EvaluationFormQuestionTypeType,
     },
@@ -8143,27 +8179,20 @@
         "NotApplicableEnabled": bool,
         "QuestionTypeProperties": EvaluationFormQuestionTypePropertiesTypeDef,
         "Weight": float,
     },
     total=False,
 )
 
+
 class EvaluationFormQuestionTypeDef(
     _RequiredEvaluationFormQuestionTypeDef, _OptionalEvaluationFormQuestionTypeDef
 ):
     pass
 
-EvaluationFormItemOutputTypeDef = TypedDict(
-    "EvaluationFormItemOutputTypeDef",
-    {
-        "Section": Dict[str, Any],
-        "Question": EvaluationFormQuestionOutputTypeDef,
-    },
-    total=False,
-)
 
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": EvaluationFormQuestionTypeDef,
     },
```

### Comparing `types-aiobotocore-connect-2.5.2.post1/types_aiobotocore_connect.egg-info/SOURCES.txt` & `types-aiobotocore-connect-2.5.2.post2/types_aiobotocore_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

