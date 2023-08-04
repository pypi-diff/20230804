# Comparing `tmp/types-aiobotocore-lexv2-models-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lexv2-models-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lexv2-models-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lexv2-models-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lexv2-models-2.5.2.post1.tar` & `types-aiobotocore-lexv2-models-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32581 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:42:03.000000 types-aiobotocore-lexv2-models-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.645542 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69636 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69534 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174293 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   174061 2023-08-02 14:42:06.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-02 14:42:04.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.649542 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32581 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.206643 types-aiobotocore-lexv2-models-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14206 2023-08-04 13:59:15.206643 types-aiobotocore-lexv2-models-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12669 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.216643 types-aiobotocore-lexv2-models-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.206643 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2111 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2110 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    76671 2023-08-04 13:42:47.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    76562 2023-08-04 13:42:47.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19551 2023-08-04 13:42:48.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19549 2023-08-04 13:42:47.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   171279 2023-08-04 13:42:53.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   171058 2023-08-04 13:42:50.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:46.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8873 2023-08-04 13:42:47.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8865 2023-08-04 13:42:47.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.206643 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14206 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      902 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/LICENSE` & `types-aiobotocore-lexv2-models-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/setup.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lexv2-models",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexModelsV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__init__.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/__main__.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexModelsV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.LexModelsV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
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

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,29 @@
     SearchOrderType,
     TestExecutionApiModeType,
     TestExecutionModalityType,
 )
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
@@ -43,16 +58,16 @@
     BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
-    CompositeSlotTypeSettingUnionTypeDef,
-    ConversationLogSettingsUnionTypeDef,
+    CompositeSlotTypeSettingTypeDef,
+    ConversationLogSettingsTypeDef,
     CreateBotAliasResponseTypeDef,
     CreateBotLocaleResponseTypeDef,
     CreateBotResponseTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateExportResponseTypeDef,
     CreateIntentResponseTypeDef,
     CreateResourcePolicyResponseTypeDef,
@@ -92,87 +107,97 @@
     DialogCodeHookSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     ExportResourceSpecificationTypeDef,
     ExportSortByTypeDef,
     ExternalSourceSettingTypeDef,
-    FulfillmentCodeHookSettingsUnionTypeDef,
+    FulfillmentCodeHookSettingsTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
     ImportFilterTypeDef,
-    ImportResourceSpecificationUnionTypeDef,
+    ImportResourceSpecificationTypeDef,
     ImportSortByTypeDef,
-    InitialResponseSettingUnionTypeDef,
+    InitialResponseSettingTypeDef,
     InputContextTypeDef,
-    IntentClosingSettingUnionTypeDef,
-    IntentConfirmationSettingUnionTypeDef,
+    IntentClosingSettingTypeDef,
+    IntentConfirmationSettingTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
     KendraConfigurationTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
     ListBotAliasesResponseTypeDef,
     ListBotLocalesResponseTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsResponseTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     ListExportsResponseTypeDef,
     ListImportsResponseTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
     ListIntentsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
     ListSlotsResponseTypeDef,
     ListSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
     ListTestExecutionsResponseTypeDef,
     ListTestSetRecordsResponseTypeDef,
     ListTestSetsResponseTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
     MultipleValuesSettingTypeDef,
     NewCustomVocabularyItemTypeDef,
     ObfuscationSettingTypeDef,
     OutputContextTypeDef,
     PrincipalTypeDef,
     SampleUtteranceTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SessionDataSortByTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
-    SlotTypeValueUnionTypeDef,
-    SlotValueElicitationSettingUnionTypeDef,
+    SlotTypeValueTypeDef,
+    SlotValueElicitationSettingTypeDef,
     SlotValueSelectionSettingTypeDef,
     StartBotRecommendationResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestExecutionResponseTypeDef,
     StartTestSetGenerationResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
-    SubSlotSettingUnionTypeDef,
+    SubSlotSettingTypeDef,
     TestExecutionResultFilterByTypeDef,
     TestExecutionSortByTypeDef,
     TestExecutionTargetTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
-    TestSetGenerationDataSourceUnionTypeDef,
+    TestSetGenerationDataSourceTypeDef,
     TestSetSortByTypeDef,
     TestSetStorageLocationTypeDef,
-    TranscriptSourceSettingUnionTypeDef,
+    TimestampTypeDef,
+    TranscriptSourceSettingTypeDef,
     UpdateBotAliasResponseTypeDef,
     UpdateBotLocaleResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateSlotResponseTypeDef,
     UpdateSlotTypeResponseTypeDef,
     UpdateTestSetResponseTypeDef,
     UtteranceAggregationDurationTypeDef,
+    UtteranceDataSortByTypeDef,
     VoiceSettingsTypeDef,
 )
 from .waiter import (
     BotAliasAvailableWaiter,
     BotAvailableWaiter,
     BotExportCompletedWaiter,
     BotImportCompletedWaiter,
@@ -325,15 +350,15 @@
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
@@ -392,21 +417,21 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
-        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -439,24 +464,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
 
     async def create_slot(
         self,
         *,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingUnionTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -465,19 +490,19 @@
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
@@ -992,14 +1017,71 @@
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_imports)
         """
 
+    async def list_intent_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsIntentMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_metrics)
+        """
+
+    async def list_intent_paths(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        intentPath: str,
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+    ) -> ListIntentPathsResponseTypeDef:
+        """
+        Retrieves summary statistics for a path of intents that users take over sessions
+        with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_paths)
+        """
+
+    async def list_intent_stage_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentStageMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the stages within intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_stage_metrics)
+        """
+
     async def list_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
@@ -1028,14 +1110,52 @@
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_recommended_intents)
         """
 
+    async def list_session_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        sortBy: SessionDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_analytics_data)
+        """
+
+    async def list_session_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsSessionMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_metrics)
+        """
+
     async def list_slot_types(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
@@ -1125,14 +1245,53 @@
         The list of the test sets See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/models.lex.v2-2020-08-07/ListTestSets).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_sets)
         """
 
+    async def list_utterance_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        sortBy: UtteranceDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceAnalyticsDataResponseTypeDef:
+        """
+        .
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_analytics_data)
+        """
+
+    async def list_utterance_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
+        attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceMetricsResponseTypeDef:
+        """
+        .
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_metrics)
+        """
+
     async def search_associated_transcripts(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1150,30 +1309,30 @@
 
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        transcriptSourceSetting: TranscriptSourceSettingUnionTypeDef,
+        transcriptSourceSetting: TranscriptSourceSettingTypeDef,
         encryptionSetting: EncryptionSettingTypeDef = ...
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
         """
 
     async def start_import(
         self,
         *,
         importId: str,
-        resourceSpecification: ImportResourceSpecificationUnionTypeDef,
+        resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
@@ -1197,15 +1356,15 @@
         """
 
     async def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
-        generationDataSource: TestSetGenerationDataSourceUnionTypeDef,
+        generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
         description: str = ...,
         testSetTags: Mapping[str, str] = ...
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
@@ -1263,15 +1422,15 @@
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
@@ -1328,22 +1487,22 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
-        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1359,24 +1518,24 @@
         """
 
     async def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingUnionTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1386,19 +1545,19 @@
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/client.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,29 @@
     SearchOrderType,
     TestExecutionApiModeType,
     TestExecutionModalityType,
 )
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
@@ -43,16 +58,16 @@
     BotMemberTypeDef,
     BotSortByTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInSlotTypeSortByTypeDef,
-    CompositeSlotTypeSettingUnionTypeDef,
-    ConversationLogSettingsUnionTypeDef,
+    CompositeSlotTypeSettingTypeDef,
+    ConversationLogSettingsTypeDef,
     CreateBotAliasResponseTypeDef,
     CreateBotLocaleResponseTypeDef,
     CreateBotResponseTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateExportResponseTypeDef,
     CreateIntentResponseTypeDef,
     CreateResourcePolicyResponseTypeDef,
@@ -92,87 +107,97 @@
     DialogCodeHookSettingsTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     ExportResourceSpecificationTypeDef,
     ExportSortByTypeDef,
     ExternalSourceSettingTypeDef,
-    FulfillmentCodeHookSettingsUnionTypeDef,
+    FulfillmentCodeHookSettingsTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
     ImportFilterTypeDef,
-    ImportResourceSpecificationUnionTypeDef,
+    ImportResourceSpecificationTypeDef,
     ImportSortByTypeDef,
-    InitialResponseSettingUnionTypeDef,
+    InitialResponseSettingTypeDef,
     InputContextTypeDef,
-    IntentClosingSettingUnionTypeDef,
-    IntentConfirmationSettingUnionTypeDef,
+    IntentClosingSettingTypeDef,
+    IntentConfirmationSettingTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
     KendraConfigurationTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
     ListBotAliasesResponseTypeDef,
     ListBotLocalesResponseTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsResponseTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     ListExportsResponseTypeDef,
     ListImportsResponseTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
     ListIntentsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
     ListSlotsResponseTypeDef,
     ListSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
     ListTestExecutionsResponseTypeDef,
     ListTestSetRecordsResponseTypeDef,
     ListTestSetsResponseTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
     MultipleValuesSettingTypeDef,
     NewCustomVocabularyItemTypeDef,
     ObfuscationSettingTypeDef,
     OutputContextTypeDef,
     PrincipalTypeDef,
     SampleUtteranceTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SessionDataSortByTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
-    SlotTypeValueUnionTypeDef,
-    SlotValueElicitationSettingUnionTypeDef,
+    SlotTypeValueTypeDef,
+    SlotValueElicitationSettingTypeDef,
     SlotValueSelectionSettingTypeDef,
     StartBotRecommendationResponseTypeDef,
     StartImportResponseTypeDef,
     StartTestExecutionResponseTypeDef,
     StartTestSetGenerationResponseTypeDef,
     StopBotRecommendationResponseTypeDef,
-    SubSlotSettingUnionTypeDef,
+    SubSlotSettingTypeDef,
     TestExecutionResultFilterByTypeDef,
     TestExecutionSortByTypeDef,
     TestExecutionTargetTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
-    TestSetGenerationDataSourceUnionTypeDef,
+    TestSetGenerationDataSourceTypeDef,
     TestSetSortByTypeDef,
     TestSetStorageLocationTypeDef,
-    TranscriptSourceSettingUnionTypeDef,
+    TimestampTypeDef,
+    TranscriptSourceSettingTypeDef,
     UpdateBotAliasResponseTypeDef,
     UpdateBotLocaleResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateSlotResponseTypeDef,
     UpdateSlotTypeResponseTypeDef,
     UpdateTestSetResponseTypeDef,
     UtteranceAggregationDurationTypeDef,
+    UtteranceDataSortByTypeDef,
     VoiceSettingsTypeDef,
 )
 from .waiter import (
     BotAliasAvailableWaiter,
     BotAvailableWaiter,
     BotExportCompletedWaiter,
     BotImportCompletedWaiter,
@@ -313,15 +338,15 @@
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
@@ -376,21 +401,21 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
-        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_intent)
         """
@@ -420,24 +445,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_resource_policy_statement)
         """
     async def create_slot(
         self,
         *,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingUnionTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#create_slot)
         """
@@ -445,19 +470,19 @@
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
     ) -> CreateSlotTypeResponseTypeDef:
         """
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
@@ -926,14 +951,68 @@
     ) -> ListImportsResponseTypeDef:
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_imports)
         """
+    async def list_intent_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsIntentMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_metrics)
+        """
+    async def list_intent_paths(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        intentPath: str,
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+    ) -> ListIntentPathsResponseTypeDef:
+        """
+        Retrieves summary statistics for a path of intents that users take over sessions
+        with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_paths)
+        """
+    async def list_intent_stage_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentStageMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the stages within intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_intent_stage_metrics)
+        """
     async def list_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
@@ -960,14 +1039,50 @@
         """
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_recommended_intents)
         """
+    async def list_session_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        sortBy: SessionDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_analytics_data)
+        """
+    async def list_session_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsSessionMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_session_metrics)
+        """
     async def list_slot_types(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
@@ -1050,14 +1165,51 @@
         """
         The list of the test sets See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/models.lex.v2-2020-08-07/ListTestSets).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_test_sets)
         """
+    async def list_utterance_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        sortBy: UtteranceDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceAnalyticsDataResponseTypeDef:
+        """
+        .
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_analytics_data)
+        """
+    async def list_utterance_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: TimestampTypeDef,
+        endDateTime: TimestampTypeDef,
+        metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
+        attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceMetricsResponseTypeDef:
+        """
+        .
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#list_utterance_metrics)
+        """
     async def search_associated_transcripts(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1074,29 +1226,29 @@
         """
     async def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
-        transcriptSourceSetting: TranscriptSourceSettingUnionTypeDef,
+        transcriptSourceSetting: TranscriptSourceSettingTypeDef,
         encryptionSetting: EncryptionSettingTypeDef = ...
     ) -> StartBotRecommendationResponseTypeDef:
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_bot_recommendation)
         """
     async def start_import(
         self,
         *,
         importId: str,
-        resourceSpecification: ImportResourceSpecificationUnionTypeDef,
+        resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
@@ -1118,15 +1270,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#start_test_execution)
         """
     async def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
-        generationDataSource: TestSetGenerationDataSourceUnionTypeDef,
+        generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
         description: str = ...,
         testSetTags: Mapping[str, str] = ...
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
@@ -1179,15 +1331,15 @@
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
         botAliasLocaleSettings: Mapping[str, BotAliasLocaleSettingsTypeDef] = ...,
-        conversationLogSettings: ConversationLogSettingsUnionTypeDef = ...,
+        conversationLogSettings: ConversationLogSettingsTypeDef = ...,
         sentimentAnalysisSettings: SentimentAnalysisSettingsTypeDef = ...
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_bot_alias)
@@ -1240,22 +1392,22 @@
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
         parentIntentSignature: str = ...,
         sampleUtterances: Sequence[SampleUtteranceTypeDef] = ...,
         dialogCodeHook: DialogCodeHookSettingsTypeDef = ...,
-        fulfillmentCodeHook: FulfillmentCodeHookSettingsUnionTypeDef = ...,
+        fulfillmentCodeHook: FulfillmentCodeHookSettingsTypeDef = ...,
         slotPriorities: Sequence[SlotPriorityTypeDef] = ...,
-        intentConfirmationSetting: IntentConfirmationSettingUnionTypeDef = ...,
-        intentClosingSetting: IntentClosingSettingUnionTypeDef = ...,
+        intentConfirmationSetting: IntentConfirmationSettingTypeDef = ...,
+        intentClosingSetting: IntentClosingSettingTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
         outputContexts: Sequence[OutputContextTypeDef] = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
-        initialResponseSetting: InitialResponseSettingUnionTypeDef = ...
+        initialResponseSetting: InitialResponseSettingTypeDef = ...
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_intent)
         """
@@ -1269,24 +1421,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_resource_policy)
         """
     async def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
-        valueElicitationSetting: SlotValueElicitationSettingUnionTypeDef,
+        valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
         description: str = ...,
         slotTypeId: str = ...,
         obfuscationSetting: ObfuscationSettingTypeDef = ...,
         multipleValuesSetting: MultipleValuesSettingTypeDef = ...,
-        subSlotSetting: SubSlotSettingUnionTypeDef = ...
+        subSlotSetting: SubSlotSettingTypeDef = ...
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot)
         """
@@ -1295,19 +1447,19 @@
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
         description: str = ...,
-        slotTypeValues: Sequence[SlotTypeValueUnionTypeDef] = ...,
+        slotTypeValues: Sequence[SlotTypeValueTypeDef] = ...,
         valueSelectionSetting: SlotValueSelectionSettingTypeDef = ...,
         parentSlotTypeSignature: str = ...,
         externalSourceSetting: ExternalSourceSettingTypeDef = ...,
-        compositeSlotTypeSetting: CompositeSlotTypeSettingUnionTypeDef = ...
+        compositeSlotTypeSetting: CompositeSlotTypeSettingTypeDef = ...
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_models/client/#update_slot_type)
         """
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/literals.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,37 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AggregatedUtterancesFilterNameType",
     "AggregatedUtterancesFilterOperatorType",
     "AggregatedUtterancesSortAttributeType",
+    "AnalyticsBinByNameType",
+    "AnalyticsCommonFilterNameType",
+    "AnalyticsFilterOperatorType",
+    "AnalyticsIntentFieldType",
+    "AnalyticsIntentFilterNameType",
+    "AnalyticsIntentMetricNameType",
+    "AnalyticsIntentStageFieldType",
+    "AnalyticsIntentStageFilterNameType",
+    "AnalyticsIntentStageMetricNameType",
+    "AnalyticsIntervalType",
+    "AnalyticsMetricStatisticType",
+    "AnalyticsModalityType",
+    "AnalyticsNodeTypeType",
+    "AnalyticsSessionFieldType",
+    "AnalyticsSessionFilterNameType",
+    "AnalyticsSessionMetricNameType",
+    "AnalyticsSessionSortByNameType",
+    "AnalyticsSortOrderType",
+    "AnalyticsUtteranceAttributeNameType",
+    "AnalyticsUtteranceFieldType",
+    "AnalyticsUtteranceFilterNameType",
+    "AnalyticsUtteranceMetricNameType",
+    "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
@@ -43,14 +66,15 @@
     "BotSortAttributeType",
     "BotStatusType",
     "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
+    "ConversationEndStateType",
     "ConversationLogsInputModeFilterType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
     "ErrorCodeType",
     "ExportFilterNameType",
     "ExportFilterOperatorType",
@@ -61,14 +85,15 @@
     "ImportFilterOperatorType",
     "ImportResourceTypeType",
     "ImportSortAttributeType",
     "ImportStatusType",
     "IntentFilterNameType",
     "IntentFilterOperatorType",
     "IntentSortAttributeType",
+    "IntentStateType",
     "MergeStrategyType",
     "MessageSelectionStrategyType",
     "ObfuscationSettingTypeType",
     "PromptAttemptType",
     "SearchOrderType",
     "SlotConstraintType",
     "SlotFilterNameType",
@@ -90,26 +115,95 @@
     "TestSetDiscrepancyReportStatusType",
     "TestSetGenerationStatusType",
     "TestSetModalityType",
     "TestSetSortAttributeType",
     "TestSetStatusType",
     "TimeDimensionType",
     "TranscriptFormatType",
+    "UtteranceContentTypeType",
     "VoiceEngineType",
     "LexModelsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "WaiterName",
     "RegionName",
 )
 
 
 AggregatedUtterancesFilterNameType = Literal["Utterance"]
 AggregatedUtterancesFilterOperatorType = Literal["CO", "EQ"]
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
+AnalyticsBinByNameType = Literal["ConversationStartTime", "UtteranceTimestamp"]
+AnalyticsCommonFilterNameType = Literal[
+    "BotAliasId", "BotVersion", "Channel", "LocaleId", "Modality"
+]
+AnalyticsFilterOperatorType = Literal["EQ", "GT", "LT"]
+AnalyticsIntentFieldType = Literal["IntentEndState", "IntentLevel", "IntentName"]
+AnalyticsIntentFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentEndState",
+    "IntentName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentMetricNameType = Literal["Count", "Dropped", "Failure", "Success", "Switched"]
+AnalyticsIntentStageFieldType = Literal["IntentStageName", "SwitchedToIntent"]
+AnalyticsIntentStageFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentName",
+    "IntentStageName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentStageMetricNameType = Literal["Count", "Dropped", "Failed", "Retry", "Success"]
+AnalyticsIntervalType = Literal["OneDay", "OneHour"]
+AnalyticsMetricStatisticType = Literal["Avg", "Max", "Sum"]
+AnalyticsModalityType = Literal["DTMF", "MultiMode", "Speech", "Text"]
+AnalyticsNodeTypeType = Literal["Exit", "Inner"]
+AnalyticsSessionFieldType = Literal["ConversationEndState", "LocaleId"]
+AnalyticsSessionFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "ConversationEndState",
+    "Duration",
+    "IntentPath",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsSessionMetricNameType = Literal[
+    "Concurrency", "Count", "Dropped", "Duration", "Failure", "Success", "TurnsPerConversation"
+]
+AnalyticsSessionSortByNameType = Literal["ConversationStartTime", "Duration", "NumberOfTurns"]
+AnalyticsSortOrderType = Literal["Ascending", "Descending"]
+AnalyticsUtteranceAttributeNameType = Literal["LastUsedIntent"]
+AnalyticsUtteranceFieldType = Literal["UtteranceState", "UtteranceText"]
+AnalyticsUtteranceFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+    "UtteranceState",
+    "UtteranceText",
+]
+AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
+AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
@@ -148,14 +242,15 @@
     "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
 BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
+ConversationEndStateType = Literal["Dropped", "Failure", "Success"]
 ConversationLogsInputModeFilterType = Literal["Speech", "Text"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
     "ConfirmIntent",
     "ElicitIntent",
     "ElicitSlot",
@@ -181,14 +276,17 @@
 ImportFilterOperatorType = Literal["CO", "EQ"]
 ImportResourceTypeType = Literal["Bot", "BotLocale", "CustomVocabulary", "TestSet"]
 ImportSortAttributeType = Literal["LastUpdatedDateTime"]
 ImportStatusType = Literal["Completed", "Deleting", "Failed", "InProgress"]
 IntentFilterNameType = Literal["IntentName"]
 IntentFilterOperatorType = Literal["CO", "EQ"]
 IntentSortAttributeType = Literal["IntentName", "LastUpdatedDateTime"]
+IntentStateType = Literal[
+    "Failed", "Fulfilled", "FulfillmentInProgress", "InProgress", "ReadyForFulfillment", "Waiting"
+]
 MergeStrategyType = Literal["Append", "FailOnConflict", "Overwrite"]
 MessageSelectionStrategyType = Literal["Ordered", "Random"]
 ObfuscationSettingTypeType = Literal["DefaultObfuscation", "None"]
 PromptAttemptType = Literal["Initial", "Retry1", "Retry2", "Retry3", "Retry4", "Retry5"]
 SearchOrderType = Literal["Ascending", "Descending"]
 SlotConstraintType = Literal["Optional", "Required"]
 SlotFilterNameType = Literal["SlotName"]
@@ -220,14 +318,15 @@
 TestSetModalityType = Literal["Audio", "Text"]
 TestSetSortAttributeType = Literal["LastUpdatedDateTime", "TestSetName"]
 TestSetStatusType = Literal[
     "Deleting", "Importing", "PendingAnnotation", "Ready", "ValidationError"
 ]
 TimeDimensionType = Literal["Days", "Hours", "Weeks"]
 TranscriptFormatType = Literal["Lex"]
+UtteranceContentTypeType = Literal["CustomPayload", "ImageResponseCard", "PlainText", "SSML"]
 VoiceEngineType = Literal["neural", "standard"]
 LexModelsV2ServiceName = Literal["lexv2-models"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -237,14 +336,15 @@
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
@@ -340,14 +440,15 @@
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
@@ -426,26 +527,28 @@
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

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/literals.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/literals.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,37 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AggregatedUtterancesFilterNameType",
     "AggregatedUtterancesFilterOperatorType",
     "AggregatedUtterancesSortAttributeType",
+    "AnalyticsBinByNameType",
+    "AnalyticsCommonFilterNameType",
+    "AnalyticsFilterOperatorType",
+    "AnalyticsIntentFieldType",
+    "AnalyticsIntentFilterNameType",
+    "AnalyticsIntentMetricNameType",
+    "AnalyticsIntentStageFieldType",
+    "AnalyticsIntentStageFilterNameType",
+    "AnalyticsIntentStageMetricNameType",
+    "AnalyticsIntervalType",
+    "AnalyticsMetricStatisticType",
+    "AnalyticsModalityType",
+    "AnalyticsNodeTypeType",
+    "AnalyticsSessionFieldType",
+    "AnalyticsSessionFilterNameType",
+    "AnalyticsSessionMetricNameType",
+    "AnalyticsSessionSortByNameType",
+    "AnalyticsSortOrderType",
+    "AnalyticsUtteranceAttributeNameType",
+    "AnalyticsUtteranceFieldType",
+    "AnalyticsUtteranceFilterNameType",
+    "AnalyticsUtteranceMetricNameType",
+    "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
@@ -42,14 +65,15 @@
     "BotSortAttributeType",
     "BotStatusType",
     "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
+    "ConversationEndStateType",
     "ConversationLogsInputModeFilterType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
     "ErrorCodeType",
     "ExportFilterNameType",
     "ExportFilterOperatorType",
@@ -60,14 +84,15 @@
     "ImportFilterOperatorType",
     "ImportResourceTypeType",
     "ImportSortAttributeType",
     "ImportStatusType",
     "IntentFilterNameType",
     "IntentFilterOperatorType",
     "IntentSortAttributeType",
+    "IntentStateType",
     "MergeStrategyType",
     "MessageSelectionStrategyType",
     "ObfuscationSettingTypeType",
     "PromptAttemptType",
     "SearchOrderType",
     "SlotConstraintType",
     "SlotFilterNameType",
@@ -89,25 +114,94 @@
     "TestSetDiscrepancyReportStatusType",
     "TestSetGenerationStatusType",
     "TestSetModalityType",
     "TestSetSortAttributeType",
     "TestSetStatusType",
     "TimeDimensionType",
     "TranscriptFormatType",
+    "UtteranceContentTypeType",
     "VoiceEngineType",
     "LexModelsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "WaiterName",
     "RegionName",
 )
 
 AggregatedUtterancesFilterNameType = Literal["Utterance"]
 AggregatedUtterancesFilterOperatorType = Literal["CO", "EQ"]
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
+AnalyticsBinByNameType = Literal["ConversationStartTime", "UtteranceTimestamp"]
+AnalyticsCommonFilterNameType = Literal[
+    "BotAliasId", "BotVersion", "Channel", "LocaleId", "Modality"
+]
+AnalyticsFilterOperatorType = Literal["EQ", "GT", "LT"]
+AnalyticsIntentFieldType = Literal["IntentEndState", "IntentLevel", "IntentName"]
+AnalyticsIntentFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentEndState",
+    "IntentName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentMetricNameType = Literal["Count", "Dropped", "Failure", "Success", "Switched"]
+AnalyticsIntentStageFieldType = Literal["IntentStageName", "SwitchedToIntent"]
+AnalyticsIntentStageFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentName",
+    "IntentStageName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentStageMetricNameType = Literal["Count", "Dropped", "Failed", "Retry", "Success"]
+AnalyticsIntervalType = Literal["OneDay", "OneHour"]
+AnalyticsMetricStatisticType = Literal["Avg", "Max", "Sum"]
+AnalyticsModalityType = Literal["DTMF", "MultiMode", "Speech", "Text"]
+AnalyticsNodeTypeType = Literal["Exit", "Inner"]
+AnalyticsSessionFieldType = Literal["ConversationEndState", "LocaleId"]
+AnalyticsSessionFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "ConversationEndState",
+    "Duration",
+    "IntentPath",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsSessionMetricNameType = Literal[
+    "Concurrency", "Count", "Dropped", "Duration", "Failure", "Success", "TurnsPerConversation"
+]
+AnalyticsSessionSortByNameType = Literal["ConversationStartTime", "Duration", "NumberOfTurns"]
+AnalyticsSortOrderType = Literal["Ascending", "Descending"]
+AnalyticsUtteranceAttributeNameType = Literal["LastUsedIntent"]
+AnalyticsUtteranceFieldType = Literal["UtteranceState", "UtteranceText"]
+AnalyticsUtteranceFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+    "UtteranceState",
+    "UtteranceText",
+]
+AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
+AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
@@ -146,14 +240,15 @@
     "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
 BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
+ConversationEndStateType = Literal["Dropped", "Failure", "Success"]
 ConversationLogsInputModeFilterType = Literal["Speech", "Text"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
     "ConfirmIntent",
     "ElicitIntent",
     "ElicitSlot",
@@ -179,14 +274,17 @@
 ImportFilterOperatorType = Literal["CO", "EQ"]
 ImportResourceTypeType = Literal["Bot", "BotLocale", "CustomVocabulary", "TestSet"]
 ImportSortAttributeType = Literal["LastUpdatedDateTime"]
 ImportStatusType = Literal["Completed", "Deleting", "Failed", "InProgress"]
 IntentFilterNameType = Literal["IntentName"]
 IntentFilterOperatorType = Literal["CO", "EQ"]
 IntentSortAttributeType = Literal["IntentName", "LastUpdatedDateTime"]
+IntentStateType = Literal[
+    "Failed", "Fulfilled", "FulfillmentInProgress", "InProgress", "ReadyForFulfillment", "Waiting"
+]
 MergeStrategyType = Literal["Append", "FailOnConflict", "Overwrite"]
 MessageSelectionStrategyType = Literal["Ordered", "Random"]
 ObfuscationSettingTypeType = Literal["DefaultObfuscation", "None"]
 PromptAttemptType = Literal["Initial", "Retry1", "Retry2", "Retry3", "Retry4", "Retry5"]
 SearchOrderType = Literal["Ascending", "Descending"]
 SlotConstraintType = Literal["Optional", "Required"]
 SlotFilterNameType = Literal["SlotName"]
@@ -218,14 +316,15 @@
 TestSetModalityType = Literal["Audio", "Text"]
 TestSetSortAttributeType = Literal["LastUpdatedDateTime", "TestSetName"]
 TestSetStatusType = Literal[
     "Deleting", "Importing", "PendingAnnotation", "Ready", "ValidationError"
 ]
 TimeDimensionType = Literal["Days", "Hours", "Weeks"]
 TranscriptFormatType = Literal["Lex"]
+UtteranceContentTypeType = Literal["CustomPayload", "ImageResponseCard", "PlainText", "SSML"]
 VoiceEngineType = Literal["neural", "standard"]
 LexModelsV2ServiceName = Literal["lexv2-models"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -235,14 +334,15 @@
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
@@ -338,14 +438,15 @@
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
@@ -424,26 +525,28 @@
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

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,59 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportStatusType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterOperatorType,
@@ -63,14 +86,15 @@
     TestResultTypeFilterType,
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
+    UtteranceContentTypeType,
     VoiceEngineType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -85,14 +109,40 @@
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
     "AggregatedUtterancesSummaryTypeDef",
     "AllowedInputTypesTypeDef",
+    "AnalyticsBinBySpecificationTypeDef",
+    "AnalyticsBinKeyTypeDef",
+    "AnalyticsIntentFilterTypeDef",
+    "AnalyticsIntentGroupByKeyTypeDef",
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    "AnalyticsIntentMetricResultTypeDef",
+    "AnalyticsIntentMetricTypeDef",
+    "AnalyticsIntentNodeSummaryTypeDef",
+    "AnalyticsIntentStageFilterTypeDef",
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    "AnalyticsIntentStageMetricResultTypeDef",
+    "AnalyticsIntentStageMetricTypeDef",
+    "AnalyticsPathFilterTypeDef",
+    "AnalyticsSessionFilterTypeDef",
+    "AnalyticsSessionGroupByKeyTypeDef",
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    "AnalyticsSessionMetricResultTypeDef",
+    "AnalyticsSessionMetricTypeDef",
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    "AnalyticsUtteranceAttributeTypeDef",
+    "AnalyticsUtteranceFilterTypeDef",
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    "AnalyticsUtteranceMetricResultTypeDef",
+    "AnalyticsUtteranceMetricTypeDef",
     "AssociatedTranscriptFilterTypeDef",
     "AssociatedTranscriptTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemTypeDef",
@@ -130,30 +180,29 @@
     "LambdaCodeHookTypeDef",
     "SubSlotTypeCompositionTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
-    "ConversationLogsDataSourceFilterByOutputTypeDef",
-    "TimestampTypeDef",
+    "ConversationLogsDataSourceFilterByTypeDef",
     "SentimentAnalysisSettingsTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
     "PrincipalTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
-    "DateRangeFilterOutputTypeDef",
+    "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
     "DeleteExportRequestRequestTypeDef",
     "DeleteImportRequestRequestTypeDef",
@@ -182,47 +231,49 @@
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionTypeDef",
-    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
     "IntentSortByTypeDef",
+    "InvokedIntentSampleTypeDef",
     "ListBotAliasesRequestRequestTypeDef",
     "ListBotRecommendationsRequestRequestTypeDef",
     "ListCustomVocabularyItemsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListRecommendedIntentsRequestRequestTypeDef",
     "RecommendedIntentSummaryTypeDef",
+    "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
+    "UtteranceDataSortByTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
-    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
@@ -238,14 +289,18 @@
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
+    "AnalyticsIntentResultTypeDef",
+    "AnalyticsIntentStageResultTypeDef",
+    "AnalyticsSessionResultTypeDef",
+    "AnalyticsUtteranceResultTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
@@ -264,22 +319,22 @@
     "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementResponseTypeDef",
     "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetTestExecutionArtifactsUrlResponseTypeDef",
     "ListCustomVocabularyItemsResponseTypeDef",
+    "ListIntentPathsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetTypeDef",
-    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
@@ -298,220 +353,183 @@
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
-    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "TextLogDestinationTypeDef",
     "CodeHookSpecificationTypeDef",
-    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
-    "ConversationLogsDataSourceOutputTypeDef",
-    "ConversationLogsDataSourceFilterByTypeDef",
-    "DateRangeFilterTypeDef",
+    "ConversationLogsDataSourceTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
-    "LexTranscriptFilterOutputTypeDef",
+    "LexTranscriptFilterTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
-    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
     "IntentClassificationTestResultItemTypeDef",
     "ListIntentsRequestRequestTypeDef",
+    "SessionSpecificationTypeDef",
+    "ListIntentMetricsRequestRequestTypeDef",
+    "ListIntentPathsRequestRequestTypeDef",
+    "ListIntentStageMetricsRequestRequestTypeDef",
+    "ListSessionMetricsRequestRequestTypeDef",
+    "ListUtteranceMetricsRequestRequestTypeDef",
     "ListRecommendedIntentsResponseTypeDef",
+    "ListSessionAnalyticsDataRequestRequestTypeDef",
     "ListSlotTypesRequestRequestTypeDef",
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
+    "ListUtteranceAnalyticsDataRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
-    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
-    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
-    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
-    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
+    "ListIntentMetricsResponseTypeDef",
+    "ListIntentStageMetricsResponseTypeDef",
+    "ListSessionMetricsResponseTypeDef",
+    "ListUtteranceMetricsResponseTypeDef",
     "PromptAttemptSpecificationTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
     "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
     "BotRecommendationResultsTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
+    "UtteranceBotResponseTypeDef",
     "TextLogSettingTypeDef",
     "BotAliasLocaleSettingsTypeDef",
-    "CompositeSlotTypeSettingUnionTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
-    "TestSetGenerationDataSourceOutputTypeDef",
-    "ConversationLogsDataSourceTypeDef",
-    "LexTranscriptFilterTypeDef",
+    "TestSetGenerationDataSourceTypeDef",
     "ListIntentsResponseTypeDef",
-    "TranscriptFilterOutputTypeDef",
+    "TranscriptFilterTypeDef",
     "ListTestSetsResponseTypeDef",
     "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
+    "ListSessionAnalyticsDataResponseTypeDef",
     "ListAggregatedUtterancesRequestRequestTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
-    "SlotTypeValueUnionTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
-    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
-    "MessageGroupOutputTypeDef",
     "MessageGroupTypeDef",
-    "ConversationLogSettingsOutputTypeDef",
+    "UtteranceSpecificationTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
-    "TestSetGenerationDataSourceTypeDef",
-    "TranscriptFilterTypeDef",
-    "S3BucketTranscriptSourceOutputTypeDef",
+    "S3BucketTranscriptSourceTypeDef",
     "ListExportsResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeResponseTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportResponseTypeDef",
-    "ImportResourceSpecificationUnionTypeDef",
     "StartImportRequestRequestTypeDef",
+    "StartImportResponseTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
-    "FulfillmentStartResponseSpecificationOutputTypeDef",
-    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
-    "PromptSpecificationOutputTypeDef",
-    "ResponseSpecificationOutputTypeDef",
-    "StillWaitingResponseSpecificationOutputTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
+    "ListUtteranceAnalyticsDataResponseTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasResponseTypeDef",
-    "ConversationLogSettingsUnionTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasRequestRequestTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
-    "TestSetGenerationDataSourceUnionTypeDef",
-    "S3BucketTranscriptSourceTypeDef",
-    "TranscriptSourceSettingOutputTypeDef",
+    "UpdateBotAliasResponseTypeDef",
+    "TranscriptSourceSettingTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationOutputTypeDef",
-    "SlotSummaryTypeDef",
-    "ConditionalBranchOutputTypeDef",
-    "DefaultConditionalBranchOutputTypeDef",
-    "WaitAndContinueSpecificationOutputTypeDef",
     "FulfillmentUpdatesSpecificationTypeDef",
+    "SlotSummaryTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
-    "TranscriptSourceSettingTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
-    "ConditionalSpecificationOutputTypeDef",
-    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
-    "TranscriptSourceSettingUnionTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
-    "IntentClosingSettingOutputTypeDef",
-    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
-    "PostFulfillmentStatusSpecificationOutputTypeDef",
-    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
-    "DialogCodeHookInvocationSettingOutputTypeDef",
-    "FulfillmentCodeHookSettingsOutputTypeDef",
-    "SubSlotSettingOutputTypeDef",
-    "IntentClosingSettingUnionTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
-    "InitialResponseSettingOutputTypeDef",
-    "IntentConfirmationSettingOutputTypeDef",
-    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "FulfillmentCodeHookSettingsUnionTypeDef",
-    "SubSlotSettingUnionTypeDef",
+    "CreateIntentRequestRequestTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentResponseTypeDef",
-    "SlotValueElicitationSettingOutputTypeDef",
-    "InitialResponseSettingUnionTypeDef",
-    "CreateIntentRequestRequestTypeDef",
-    "IntentConfirmationSettingUnionTypeDef",
     "UpdateIntentRequestRequestTypeDef",
+    "UpdateIntentResponseTypeDef",
     "SlotValueElicitationSettingTypeDef",
+    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotResponseTypeDef",
-    "CreateSlotRequestRequestTypeDef",
-    "SlotValueElicitationSettingUnionTypeDef",
     "UpdateSlotRequestRequestTypeDef",
+    "UpdateSlotResponseTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
@@ -574,14 +592,309 @@
     "AllowedInputTypesTypeDef",
     {
         "allowAudioInput": bool,
         "allowDTMFInput": bool,
     },
 )
 
+_RequiredAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_RequiredAnalyticsBinBySpecificationTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "interval": AnalyticsIntervalType,
+    },
+)
+_OptionalAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_OptionalAnalyticsBinBySpecificationTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsBinBySpecificationTypeDef(
+    _RequiredAnalyticsBinBySpecificationTypeDef, _OptionalAnalyticsBinBySpecificationTypeDef
+):
+    pass
+
+
+AnalyticsBinKeyTypeDef = TypedDict(
+    "AnalyticsBinKeyTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "value": int,
+    },
+    total=False,
+)
+
+AnalyticsIntentFilterTypeDef = TypedDict(
+    "AnalyticsIntentFilterTypeDef",
+    {
+        "name": AnalyticsIntentFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsIntentGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+    },
+)
+
+AnalyticsIntentMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsIntentMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentMetricTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsIntentMetricTypeDef(
+    _RequiredAnalyticsIntentMetricTypeDef, _OptionalAnalyticsIntentMetricTypeDef
+):
+    pass
+
+
+AnalyticsIntentNodeSummaryTypeDef = TypedDict(
+    "AnalyticsIntentNodeSummaryTypeDef",
+    {
+        "intentName": str,
+        "intentPath": str,
+        "intentCount": int,
+        "intentLevel": int,
+        "nodeType": AnalyticsNodeTypeType,
+    },
+    total=False,
+)
+
+AnalyticsIntentStageFilterTypeDef = TypedDict(
+    "AnalyticsIntentStageFilterTypeDef",
+    {
+        "name": AnalyticsIntentStageFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentStageGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsIntentStageGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+    },
+)
+
+AnalyticsIntentStageMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentStageMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentStageMetricTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentStageMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsIntentStageMetricTypeDef(
+    _RequiredAnalyticsIntentStageMetricTypeDef, _OptionalAnalyticsIntentStageMetricTypeDef
+):
+    pass
+
+
+AnalyticsPathFilterTypeDef = TypedDict(
+    "AnalyticsPathFilterTypeDef",
+    {
+        "name": AnalyticsCommonFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionFilterTypeDef = TypedDict(
+    "AnalyticsSessionFilterTypeDef",
+    {
+        "name": AnalyticsSessionFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionGroupByKeyTypeDef = TypedDict(
+    "AnalyticsSessionGroupByKeyTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsSessionGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+    },
+)
+
+AnalyticsSessionMetricResultTypeDef = TypedDict(
+    "AnalyticsSessionMetricResultTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsSessionMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsSessionMetricTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsSessionMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsSessionMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsSessionMetricTypeDef(
+    _RequiredAnalyticsSessionMetricTypeDef, _OptionalAnalyticsSessionMetricTypeDef
+):
+    pass
+
+
+AnalyticsUtteranceAttributeResultTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    {
+        "lastUsedIntent": str,
+    },
+    total=False,
+)
+
+AnalyticsUtteranceAttributeTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeTypeDef",
+    {
+        "name": Literal["LastUsedIntent"],
+    },
+)
+
+AnalyticsUtteranceFilterTypeDef = TypedDict(
+    "AnalyticsUtteranceFilterTypeDef",
+    {
+        "name": AnalyticsUtteranceFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsUtteranceGroupByKeyTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsUtteranceGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+    },
+)
+
+AnalyticsUtteranceMetricResultTypeDef = TypedDict(
+    "AnalyticsUtteranceMetricResultTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsUtteranceMetricTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsUtteranceMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsUtteranceMetricTypeDef(
+    _RequiredAnalyticsUtteranceMetricTypeDef, _OptionalAnalyticsUtteranceMetricTypeDef
+):
+    pass
+
+
 AssociatedTranscriptFilterTypeDef = TypedDict(
     "AssociatedTranscriptFilterTypeDef",
     {
         "name": AssociatedTranscriptFilterNameType,
         "values": Sequence[str],
     },
 )
@@ -1053,24 +1366,23 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByOutputTypeDef",
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
@@ -1179,16 +1491,16 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterOutputTypeDef = TypedDict(
-    "DateRangeFilterOutputTypeDef",
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
@@ -1611,23 +1923,14 @@
 )
 
 
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
 
-IntentOverrideOutputTypeDef = TypedDict(
-    "IntentOverrideOutputTypeDef",
-    {
-        "name": str,
-        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
-    },
-    total=False,
-)
-
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
     total=False,
@@ -1784,14 +2087,22 @@
     "IntentSortByTypeDef",
     {
         "attribute": IntentSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+InvokedIntentSampleTypeDef = TypedDict(
+    "InvokedIntentSampleTypeDef",
+    {
+        "intentName": str,
+    },
+    total=False,
+)
+
 _RequiredListBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotAliasesRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotAliasesRequestRequestTypeDef = TypedDict(
@@ -1856,14 +2167,15 @@
 class ListCustomVocabularyItemsRequestRequestTypeDef(
     _RequiredListCustomVocabularyItemsRequestRequestTypeDef,
     _OptionalListCustomVocabularyItemsRequestRequestTypeDef,
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredListRecommendedIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendedIntentsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -1892,14 +2204,22 @@
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
     total=False,
 )
 
+SessionDataSortByTypeDef = TypedDict(
+    "SessionDataSortByTypeDef",
+    {
+        "name": AnalyticsSessionSortByNameType,
+        "order": AnalyticsSortOrderType,
+    },
+)
+
 SlotTypeFilterTypeDef = TypedDict(
     "SlotTypeFilterTypeDef",
     {
         "name": SlotTypeFilterNameType,
         "values": Sequence[str],
         "operator": SlotTypeFilterOperatorType,
     },
@@ -1985,14 +2305,22 @@
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+UtteranceDataSortByTypeDef = TypedDict(
+    "UtteranceDataSortByTypeDef",
+    {
+        "name": Literal["UtteranceTimestamp"],
+        "order": AnalyticsSortOrderType,
+    },
+)
+
 PlainTextMessageTypeDef = TypedDict(
     "PlainTextMessageTypeDef",
     {
         "value": str,
     },
 )
 
@@ -2022,26 +2350,18 @@
 
 class OverallTestResultItemTypeDef(
     _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
 ):
     pass
 
 
-PathFormatOutputTypeDef = TypedDict(
-    "PathFormatOutputTypeDef",
-    {
-        "objectPrefixes": List[str],
-    },
-    total=False,
-)
-
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": Sequence[str],
+        "objectPrefixes": List[str],
     },
     total=False,
 )
 
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
@@ -2298,14 +2618,55 @@
 )
 
 
 class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
     pass
 
 
+AnalyticsIntentResultTypeDef = TypedDict(
+    "AnalyticsIntentResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsIntentStageResultTypeDef = TypedDict(
+    "AnalyticsIntentStageResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsSessionResultTypeDef = TypedDict(
+    "AnalyticsSessionResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsSessionGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsSessionMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsUtteranceResultTypeDef = TypedDict(
+    "AnalyticsUtteranceResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsUtteranceGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsUtteranceMetricResultTypeDef],
+        "attributeResults": List[AnalyticsUtteranceAttributeResultTypeDef],
+    },
+    total=False,
+)
+
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2588,14 +2949,22 @@
         "localeId": str,
         "customVocabularyItems": List[CustomVocabularyItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2659,53 +3028,28 @@
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
-_RequiredBotImportSpecificationOutputTypeDef = TypedDict(
-    "_RequiredBotImportSpecificationOutputTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-    },
-)
-_OptionalBotImportSpecificationOutputTypeDef = TypedDict(
-    "_OptionalBotImportSpecificationOutputTypeDef",
-    {
-        "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class BotImportSpecificationOutputTypeDef(
-    _RequiredBotImportSpecificationOutputTypeDef, _OptionalBotImportSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
     },
     total=False,
 )
 
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
@@ -3165,37 +3509,14 @@
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
-    pass
-
-
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
@@ -3225,22 +3546,14 @@
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
-CompositeSlotTypeSettingOutputTypeDef = TypedDict(
-    "CompositeSlotTypeSettingOutputTypeDef",
-    {
-        "subSlots": List[SubSlotTypeCompositionTypeDef],
-    },
-    total=False,
-)
-
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
@@ -3286,38 +3599,21 @@
 
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
 
-ConversationLogsDataSourceOutputTypeDef = TypedDict(
-    "ConversationLogsDataSourceOutputTypeDef",
+ConversationLogsDataSourceTypeDef = TypedDict(
+    "ConversationLogsDataSourceTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
-    },
-)
-
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
-    {
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-        "inputMode": ConversationLogsInputModeFilterType,
-    },
-)
-
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
-    {
-        "startDateTime": TimestampTypeDef,
-        "endDateTime": TimestampTypeDef,
+        "filter": ConversationLogsDataSourceFilterByTypeDef,
     },
 )
 
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
@@ -3354,18 +3650,18 @@
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
 
-LexTranscriptFilterOutputTypeDef = TypedDict(
-    "LexTranscriptFilterOutputTypeDef",
+LexTranscriptFilterTypeDef = TypedDict(
+    "LexTranscriptFilterTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterOutputTypeDef,
+        "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
@@ -3628,24 +3924,14 @@
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialogStateOutputTypeDef = TypedDict(
-    "DialogStateOutputTypeDef",
-    {
-        "dialogAction": DialogActionTypeDef,
-        "intent": IntentOverrideOutputTypeDef,
-        "sessionAttributes": Dict[str, str],
-    },
-    total=False,
-)
-
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
         "sessionAttributes": Mapping[str, str],
     },
@@ -3752,27 +4038,214 @@
 
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
 
+SessionSpecificationTypeDef = TypedDict(
+    "SessionSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "channel": str,
+        "sessionId": str,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "conversationDurationSeconds": int,
+        "conversationEndState": ConversationEndStateType,
+        "mode": AnalyticsModalityType,
+        "numberOfTurns": int,
+        "invokedIntentSamples": List[InvokedIntentSampleTypeDef],
+        "originatingRequestId": str,
+    },
+    total=False,
+)
+
+_RequiredListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsIntentMetricTypeDef],
+    },
+)
+_OptionalListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListIntentMetricsRequestRequestTypeDef(
+    _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentPathsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "intentPath": str,
+    },
+)
+_OptionalListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentPathsRequestRequestTypeDef",
+    {
+        "filters": Sequence[AnalyticsPathFilterTypeDef],
+    },
+    total=False,
+)
+
+
+class ListIntentPathsRequestRequestTypeDef(
+    _RequiredListIntentPathsRequestRequestTypeDef, _OptionalListIntentPathsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsIntentStageMetricTypeDef],
+    },
+)
+_OptionalListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentStageFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListIntentStageMetricsRequestRequestTypeDef(
+    _RequiredListIntentStageMetricsRequestRequestTypeDef,
+    _OptionalListIntentStageMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsSessionMetricTypeDef],
+    },
+)
+_OptionalListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsSessionGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListSessionMetricsRequestRequestTypeDef(
+    _RequiredListSessionMetricsRequestRequestTypeDef,
+    _OptionalListSessionMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsUtteranceMetricTypeDef],
+    },
+)
+_OptionalListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef],
+        "attributes": Sequence[AnalyticsUtteranceAttributeTypeDef],
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListUtteranceMetricsRequestRequestTypeDef(
+    _RequiredListUtteranceMetricsRequestRequestTypeDef,
+    _OptionalListUtteranceMetricsRequestRequestTypeDef,
+):
+    pass
+
+
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+    },
+)
+_OptionalListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": SessionDataSortByTypeDef,
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListSessionAnalyticsDataRequestRequestTypeDef(
+    _RequiredListSessionAnalyticsDataRequestRequestTypeDef,
+    _OptionalListSessionAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3850,14 +4323,41 @@
         "sortBy": TestSetSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+    },
+)
+_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": UtteranceDataSortByTypeDef,
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListUtteranceAnalyticsDataRequestRequestTypeDef(
+    _RequiredListUtteranceAnalyticsDataRequestRequestTypeDef,
+    _OptionalListUtteranceAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
+
 OverallTestResultsTypeDef = TypedDict(
     "OverallTestResultsTypeDef",
     {
         "items": List[OverallTestResultItemTypeDef],
     },
 )
 
@@ -3873,39 +4373,23 @@
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
-SlotTypeValueOutputTypeDef = TypedDict(
-    "SlotTypeValueOutputTypeDef",
-    {
-        "sampleValue": SampleValueTypeDef,
-        "synonyms": List[SampleValueTypeDef],
-    },
-    total=False,
-)
-
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
-SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
-    "SlotDefaultValueSpecificationOutputTypeDef",
-    {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
-    },
-)
-
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3913,24 +4397,14 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
-SlotValueOverrideOutputTypeDef = TypedDict(
-    "SlotValueOverrideOutputTypeDef",
-    {
-        "shape": SlotShapeType,
-        "value": SlotValueTypeDef,
-        "values": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
@@ -3971,56 +4445,29 @@
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
-_RequiredTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
-    "_RequiredTestSetImportResourceSpecificationOutputTypeDef",
-    {
-        "testSetName": str,
-        "roleArn": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "importInputLocation": TestSetImportInputLocationTypeDef,
-        "modality": TestSetModalityType,
-    },
-)
-_OptionalTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
-    "_OptionalTestSetImportResourceSpecificationOutputTypeDef",
-    {
-        "description": str,
-        "testSetTags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class TestSetImportResourceSpecificationOutputTypeDef(
-    _RequiredTestSetImportResourceSpecificationOutputTypeDef,
-    _OptionalTestSetImportResourceSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Mapping[str, str],
+        "testSetTags": Dict[str, str],
     },
     total=False,
 )
 
 
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
@@ -4056,14 +4503,54 @@
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
     total=False,
 )
 
+ListIntentMetricsResponseTypeDef = TypedDict(
+    "ListIntentMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIntentStageMetricsResponseTypeDef = TypedDict(
+    "ListIntentStageMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentStageResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionMetricsResponseTypeDef = TypedDict(
+    "ListSessionMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsSessionResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUtteranceMetricsResponseTypeDef = TypedDict(
+    "ListUtteranceMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsUtteranceResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPromptAttemptSpecificationTypeDef = TypedDict(
     "_RequiredPromptAttemptSpecificationTypeDef",
     {
         "allowedInputTypes": AllowedInputTypesTypeDef,
     },
 )
 _OptionalPromptAttemptSpecificationTypeDef = TypedDict(
@@ -4167,31 +4654,30 @@
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
     total=False,
 )
 
-MessageOutputTypeDef = TypedDict(
-    "MessageOutputTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
-        "imageResponseCard": ImageResponseCardOutputTypeDef,
+        "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+UtteranceBotResponseTypeDef = TypedDict(
+    "UtteranceBotResponseTypeDef",
     {
-        "plainTextMessage": PlainTextMessageTypeDef,
-        "customPayload": CustomPayloadTypeDef,
-        "ssmlMessage": SSMLMessageTypeDef,
+        "content": str,
+        "contentType": UtteranceContentTypeType,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
 TextLogSettingTypeDef = TypedDict(
     "TextLogSettingTypeDef",
@@ -4218,17 +4704,14 @@
 
 class BotAliasLocaleSettingsTypeDef(
     _RequiredBotAliasLocaleSettingsTypeDef, _OptionalBotAliasLocaleSettingsTypeDef
 ):
     pass
 
 
-CompositeSlotTypeSettingUnionTypeDef = Union[
-    CompositeSlotTypeSettingTypeDef, CompositeSlotTypeSettingOutputTypeDef
-]
 ConversationLevelTestResultsTypeDef = TypedDict(
     "ConversationLevelTestResultsTypeDef",
     {
         "items": List[ConversationLevelTestResultItemTypeDef],
     },
 )
 
@@ -4252,36 +4735,18 @@
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
 
-TestSetGenerationDataSourceOutputTypeDef = TypedDict(
-    "TestSetGenerationDataSourceOutputTypeDef",
-    {
-        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
-    },
-    total=False,
-)
-
-ConversationLogsDataSourceTypeDef = TypedDict(
-    "ConversationLogsDataSourceTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByTypeDef,
-    },
-)
-
-LexTranscriptFilterTypeDef = TypedDict(
-    "LexTranscriptFilterTypeDef",
+TestSetGenerationDataSourceTypeDef = TypedDict(
+    "TestSetGenerationDataSourceTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterTypeDef,
+        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
 
 ListIntentsResponseTypeDef = TypedDict(
     "ListIntentsResponseTypeDef",
     {
@@ -4290,18 +4755,18 @@
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TranscriptFilterOutputTypeDef = TypedDict(
-    "TranscriptFilterOutputTypeDef",
+TranscriptFilterTypeDef = TypedDict(
+    "TranscriptFilterTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
+        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
     total=False,
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
@@ -4397,14 +4862,24 @@
 IntentClassificationTestResultsTypeDef = TypedDict(
     "IntentClassificationTestResultsTypeDef",
     {
         "items": List[IntentClassificationTestResultItemTypeDef],
     },
 )
 
+ListSessionAnalyticsDataResponseTypeDef = TypedDict(
+    "ListSessionAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "sessions": List[SessionSpecificationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
     },
@@ -4443,15 +4918,14 @@
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeValueUnionTypeDef = Union[SlotTypeValueTypeDef, SlotTypeValueOutputTypeDef]
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
@@ -4488,25 +4962,14 @@
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportResourceSpecificationOutputTypeDef = TypedDict(
-    "ImportResourceSpecificationOutputTypeDef",
-    {
-        "botImportSpecification": BotImportSpecificationOutputTypeDef,
-        "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
-        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
-        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
         "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
         "testSetImportResourceSpecification": TestSetImportResourceSpecificationTypeDef,
@@ -4541,35 +5004,14 @@
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageGroupOutputTypeDef = TypedDict(
-    "_RequiredMessageGroupOutputTypeDef",
-    {
-        "message": MessageOutputTypeDef,
-    },
-)
-_OptionalMessageGroupOutputTypeDef = TypedDict(
-    "_OptionalMessageGroupOutputTypeDef",
-    {
-        "variations": List[MessageOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class MessageGroupOutputTypeDef(
-    _RequiredMessageGroupOutputTypeDef, _OptionalMessageGroupOutputTypeDef
-):
-    pass
-
-
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
@@ -4581,19 +5023,39 @@
 )
 
 
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
 
-ConversationLogSettingsOutputTypeDef = TypedDict(
-    "ConversationLogSettingsOutputTypeDef",
+UtteranceSpecificationTypeDef = TypedDict(
+    "UtteranceSpecificationTypeDef",
     {
-        "textLogSettings": List[TextLogSettingTypeDef],
-        "audioLogSettings": List[AudioLogSettingTypeDef],
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "sessionId": str,
+        "channel": str,
+        "mode": AnalyticsModalityType,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "utterance": str,
+        "utteranceTimestamp": datetime,
+        "audioVoiceDurationMillis": int,
+        "utteranceUnderstood": bool,
+        "inputType": str,
+        "outputType": str,
+        "associatedIntentName": str,
+        "associatedSlotName": str,
+        "intentState": IntentStateType,
+        "dialogActionType": str,
+        "botResponseAudioVoiceId": str,
+        "slotsFilledInSession": str,
+        "utteranceRequestId": str,
+        "botResponses": List[UtteranceBotResponseTypeDef],
     },
     total=False,
 )
 
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
@@ -4609,74 +5071,84 @@
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
-        "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-TestSetGenerationDataSourceTypeDef = TypedDict(
-    "TestSetGenerationDataSourceTypeDef",
+_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
     {
-        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
+        "description": str,
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
-TranscriptFilterTypeDef = TypedDict(
-    "TranscriptFilterTypeDef",
+
+class StartTestSetGenerationRequestRequestTypeDef(
+    _RequiredStartTestSetGenerationRequestRequestTypeDef,
+    _OptionalStartTestSetGenerationRequestRequestTypeDef,
+):
+    pass
+
+
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
+        "testSetName": str,
+        "description": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredS3BucketTranscriptSourceOutputTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceOutputTypeDef",
+_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceTypeDef",
     {
         "s3BucketName": str,
         "transcriptFormat": Literal["Lex"],
     },
 )
-_OptionalS3BucketTranscriptSourceOutputTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceOutputTypeDef",
+_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceTypeDef",
     {
-        "pathFormat": PathFormatOutputTypeDef,
-        "transcriptFilter": TranscriptFilterOutputTypeDef,
+        "pathFormat": PathFormatTypeDef,
+        "transcriptFilter": TranscriptFilterTypeDef,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
 
-class S3BucketTranscriptSourceOutputTypeDef(
-    _RequiredS3BucketTranscriptSourceOutputTypeDef, _OptionalS3BucketTranscriptSourceOutputTypeDef
+class S3BucketTranscriptSourceTypeDef(
+    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
 ):
     pass
 
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
@@ -4685,170 +5157,155 @@
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
+    },
+)
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
+):
+    pass
+
+
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
 
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
-    {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
-):
-    pass
-
-
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "resourceSpecification": ImportResourceSpecificationTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportResourceSpecificationUnionTypeDef = Union[
-    ImportResourceSpecificationTypeDef, ImportResourceSpecificationOutputTypeDef
-]
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4864,14 +5321,26 @@
 
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
 
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUserTurnResultTypeDef = TypedDict(
     "_RequiredUserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
     },
 )
@@ -4898,129 +5367,14 @@
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
-_RequiredFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentStartResponseSpecificationOutputTypeDef",
-    {
-        "delayInSeconds": int,
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentStartResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-
-class FulfillmentStartResponseSpecificationOutputTypeDef(
-    _RequiredFulfillmentStartResponseSpecificationOutputTypeDef,
-    _OptionalFulfillmentStartResponseSpecificationOutputTypeDef,
-):
-    pass
-
-
-_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef",
-    {
-        "frequencyInSeconds": int,
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-
-class FulfillmentUpdateResponseSpecificationOutputTypeDef(
-    _RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef,
-    _OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef,
-):
-    pass
-
-
-_RequiredPromptSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPromptSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-        "maxRetries": int,
-    },
-)
-_OptionalPromptSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPromptSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-        "messageSelectionStrategy": MessageSelectionStrategyType,
-        "promptAttemptsSpecification": Dict[PromptAttemptType, PromptAttemptSpecificationTypeDef],
-    },
-    total=False,
-)
-
-
-class PromptSpecificationOutputTypeDef(
-    _RequiredPromptSpecificationOutputTypeDef, _OptionalPromptSpecificationOutputTypeDef
-):
-    pass
-
-
-_RequiredResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredResponseSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-
-class ResponseSpecificationOutputTypeDef(
-    _RequiredResponseSpecificationOutputTypeDef, _OptionalResponseSpecificationOutputTypeDef
-):
-    pass
-
-
-_RequiredStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredStillWaitingResponseSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-        "frequencyInSeconds": int,
-        "timeoutInSeconds": int,
-    },
-)
-_OptionalStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalStillWaitingResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-
-class StillWaitingResponseSpecificationOutputTypeDef(
-    _RequiredStillWaitingResponseSpecificationOutputTypeDef,
-    _OptionalStillWaitingResponseSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -5130,100 +5484,89 @@
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
 
-CreateBotAliasResponseTypeDef = TypedDict(
-    "CreateBotAliasResponseTypeDef",
+ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
+    "ListUtteranceAnalyticsDataResponseTypeDef",
     {
-        "botAliasId": str,
-        "botAliasName": str,
-        "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
         "botId": str,
-        "creationDateTime": datetime,
-        "tags": Dict[str, str],
+        "nextToken": str,
+        "utterances": List[UtteranceSpecificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBotAliasResponseTypeDef = TypedDict(
-    "DescribeBotAliasResponseTypeDef",
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
     {
-        "botAliasId": str,
         "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
+    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
+):
+    pass
+
+
+CreateBotAliasResponseTypeDef = TypedDict(
+    "CreateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConversationLogSettingsUnionTypeDef = Union[
-    ConversationLogSettingsTypeDef, ConversationLogSettingsOutputTypeDef
-]
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
+DescribeBotAliasResponseTypeDef = TypedDict(
+    "DescribeBotAliasResponseTypeDef",
     {
+        "botAliasId": str,
         "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
+        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "botId": str,
     },
@@ -5243,71 +5586,36 @@
 
 class UpdateBotAliasRequestRequestTypeDef(
     _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
-    {
-        "testSetName": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-    },
-)
-_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
     {
+        "botAliasId": str,
+        "botAliasName": str,
         "description": str,
-        "testSetTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartTestSetGenerationRequestRequestTypeDef(
-    _RequiredStartTestSetGenerationRequestRequestTypeDef,
-    _OptionalStartTestSetGenerationRequestRequestTypeDef,
-):
-    pass
-
-
-TestSetGenerationDataSourceUnionTypeDef = Union[
-    TestSetGenerationDataSourceTypeDef, TestSetGenerationDataSourceOutputTypeDef
-]
-_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceTypeDef",
-    {
-        "s3BucketName": str,
-        "transcriptFormat": Literal["Lex"],
-    },
-)
-_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceTypeDef",
-    {
-        "pathFormat": PathFormatTypeDef,
-        "transcriptFilter": TranscriptFilterTypeDef,
-        "kmsKeyArn": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class S3BucketTranscriptSourceTypeDef(
-    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
-):
-    pass
-
-
-TranscriptSourceSettingOutputTypeDef = TypedDict(
-    "TranscriptSourceSettingOutputTypeDef",
+TranscriptSourceSettingTypeDef = TypedDict(
+    "TranscriptSourceSettingTypeDef",
     {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
     },
     total=False,
 )
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
@@ -5322,131 +5630,51 @@
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationOutputTypeDef",
+_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
     {
         "active": bool,
     },
 )
-_OptionalFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationOutputTypeDef",
+_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
     {
-        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
+        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
 
-class FulfillmentUpdatesSpecificationOutputTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationOutputTypeDef,
-    _OptionalFulfillmentUpdatesSpecificationOutputTypeDef,
+class FulfillmentUpdatesSpecificationTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
 ):
     pass
 
 
 SlotSummaryTypeDef = TypedDict(
     "SlotSummaryTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotConstraint": SlotConstraintType,
         "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
+        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredConditionalBranchOutputTypeDef = TypedDict(
-    "_RequiredConditionalBranchOutputTypeDef",
-    {
-        "name": str,
-        "condition": ConditionTypeDef,
-        "nextStep": DialogStateOutputTypeDef,
-    },
-)
-_OptionalConditionalBranchOutputTypeDef = TypedDict(
-    "_OptionalConditionalBranchOutputTypeDef",
-    {
-        "response": ResponseSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ConditionalBranchOutputTypeDef(
-    _RequiredConditionalBranchOutputTypeDef, _OptionalConditionalBranchOutputTypeDef
-):
-    pass
-
-
-DefaultConditionalBranchOutputTypeDef = TypedDict(
-    "DefaultConditionalBranchOutputTypeDef",
-    {
-        "nextStep": DialogStateOutputTypeDef,
-        "response": ResponseSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredWaitAndContinueSpecificationOutputTypeDef = TypedDict(
-    "_RequiredWaitAndContinueSpecificationOutputTypeDef",
-    {
-        "waitingResponse": ResponseSpecificationOutputTypeDef,
-        "continueResponse": ResponseSpecificationOutputTypeDef,
-    },
-)
-_OptionalWaitAndContinueSpecificationOutputTypeDef = TypedDict(
-    "_OptionalWaitAndContinueSpecificationOutputTypeDef",
-    {
-        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
-        "active": bool,
-    },
-    total=False,
-)
-
-
-class WaitAndContinueSpecificationOutputTypeDef(
-    _RequiredWaitAndContinueSpecificationOutputTypeDef,
-    _OptionalWaitAndContinueSpecificationOutputTypeDef,
-):
-    pass
-
-
-_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
-    {
-        "active": bool,
-    },
-)
-_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
-    {
-        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
-        "timeoutInSeconds": int,
-    },
-    total=False,
-)
-
-
-class FulfillmentUpdatesSpecificationTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
-):
-    pass
-
-
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -5494,50 +5722,67 @@
 
 class WaitAndContinueSpecificationTypeDef(
     _RequiredWaitAndContinueSpecificationTypeDef, _OptionalWaitAndContinueSpecificationTypeDef
 ):
     pass
 
 
-TranscriptSourceSettingTypeDef = TypedDict(
-    "TranscriptSourceSettingTypeDef",
-    {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
-    },
-    total=False,
-)
-
 DescribeBotRecommendationResponseTypeDef = TypedDict(
     "DescribeBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+    },
+)
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
+    {
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+    total=False,
+)
+
+
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
+):
+    pass
+
+
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
@@ -5545,15 +5790,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
     "_RequiredUtteranceLevelTestResultItemTypeDef",
@@ -5609,47 +5854,14 @@
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionalSpecificationOutputTypeDef = TypedDict(
-    "ConditionalSpecificationOutputTypeDef",
-    {
-        "active": bool,
-        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
-        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
-    },
-)
-
-_RequiredSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_RequiredSubSlotValueElicitationSettingOutputTypeDef",
-    {
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-    },
-)
-_OptionalSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_OptionalSubSlotValueElicitationSettingOutputTypeDef",
-    {
-        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SubSlotValueElicitationSettingOutputTypeDef(
-    _RequiredSubSlotValueElicitationSettingOutputTypeDef,
-    _OptionalSubSlotValueElicitationSettingOutputTypeDef,
-):
-    pass
-
-
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
     },
@@ -5674,42 +5886,14 @@
 
 class SubSlotValueElicitationSettingTypeDef(
     _RequiredSubSlotValueElicitationSettingTypeDef, _OptionalSubSlotValueElicitationSettingTypeDef
 ):
     pass
 
 
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-    },
-)
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
-
-TranscriptSourceSettingUnionTypeDef = Union[
-    TranscriptSourceSettingTypeDef, TranscriptSourceSettingOutputTypeDef
-]
 UtteranceLevelTestResultsTypeDef = TypedDict(
     "UtteranceLevelTestResultsTypeDef",
     {
         "items": List[UtteranceLevelTestResultItemTypeDef],
     },
 )
 
@@ -5718,65 +5902,14 @@
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntentClosingSettingOutputTypeDef = TypedDict(
-    "IntentClosingSettingOutputTypeDef",
-    {
-        "closingResponse": ResponseSpecificationOutputTypeDef,
-        "active": bool,
-        "nextStep": DialogStateOutputTypeDef,
-        "conditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
-    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
-    {
-        "successResponse": ResponseSpecificationOutputTypeDef,
-        "successNextStep": DialogStateOutputTypeDef,
-        "successConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "timeoutResponse": ResponseSpecificationOutputTypeDef,
-        "timeoutNextStep": DialogStateOutputTypeDef,
-        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
-    "PostFulfillmentStatusSpecificationOutputTypeDef",
-    {
-        "successResponse": ResponseSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "timeoutResponse": ResponseSpecificationOutputTypeDef,
-        "successNextStep": DialogStateOutputTypeDef,
-        "successConditional": ConditionalSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "timeoutNextStep": DialogStateOutputTypeDef,
-        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-SpecificationsOutputTypeDef = TypedDict(
-    "SpecificationsOutputTypeDef",
-    {
-        "slotTypeId": str,
-        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
-    },
-)
-
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
         "active": bool,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
@@ -5832,74 +5965,14 @@
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
     total=False,
 )
 
-_RequiredDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
-    "_RequiredDialogCodeHookInvocationSettingOutputTypeDef",
-    {
-        "enableCodeHookInvocation": bool,
-        "active": bool,
-        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
-    },
-)
-_OptionalDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
-    "_OptionalDialogCodeHookInvocationSettingOutputTypeDef",
-    {
-        "invocationLabel": str,
-    },
-    total=False,
-)
-
-
-class DialogCodeHookInvocationSettingOutputTypeDef(
-    _RequiredDialogCodeHookInvocationSettingOutputTypeDef,
-    _OptionalDialogCodeHookInvocationSettingOutputTypeDef,
-):
-    pass
-
-
-_RequiredFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentCodeHookSettingsOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentCodeHookSettingsOutputTypeDef",
-    {
-        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
-        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
-        "active": bool,
-    },
-    total=False,
-)
-
-
-class FulfillmentCodeHookSettingsOutputTypeDef(
-    _RequiredFulfillmentCodeHookSettingsOutputTypeDef,
-    _OptionalFulfillmentCodeHookSettingsOutputTypeDef,
-):
-    pass
-
-
-SubSlotSettingOutputTypeDef = TypedDict(
-    "SubSlotSettingOutputTypeDef",
-    {
-        "expression": str,
-        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
-    },
-    total=False,
-)
-
-IntentClosingSettingUnionTypeDef = Union[
-    IntentClosingSettingTypeDef, IntentClosingSettingOutputTypeDef
-]
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
         "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationTypeDef,
     },
@@ -5956,72 +6029,14 @@
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitialResponseSettingOutputTypeDef = TypedDict(
-    "InitialResponseSettingOutputTypeDef",
-    {
-        "initialResponse": ResponseSpecificationOutputTypeDef,
-        "nextStep": DialogStateOutputTypeDef,
-        "conditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredIntentConfirmationSettingOutputTypeDef = TypedDict(
-    "_RequiredIntentConfirmationSettingOutputTypeDef",
-    {
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-    },
-)
-_OptionalIntentConfirmationSettingOutputTypeDef = TypedDict(
-    "_OptionalIntentConfirmationSettingOutputTypeDef",
-    {
-        "declinationResponse": ResponseSpecificationOutputTypeDef,
-        "active": bool,
-        "confirmationResponse": ResponseSpecificationOutputTypeDef,
-        "confirmationNextStep": DialogStateOutputTypeDef,
-        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
-        "declinationNextStep": DialogStateOutputTypeDef,
-        "declinationConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class IntentConfirmationSettingOutputTypeDef(
-    _RequiredIntentConfirmationSettingOutputTypeDef, _OptionalIntentConfirmationSettingOutputTypeDef
-):
-    pass
-
-
-SlotCaptureSettingOutputTypeDef = TypedDict(
-    "SlotCaptureSettingOutputTypeDef",
-    {
-        "captureResponse": ResponseSpecificationOutputTypeDef,
-        "captureNextStep": DialogStateOutputTypeDef,
-        "captureConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
-    },
-    total=False,
-)
-
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
@@ -6072,196 +6087,160 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-FulfillmentCodeHookSettingsUnionTypeDef = Union[
-    FulfillmentCodeHookSettingsTypeDef, FulfillmentCodeHookSettingsOutputTypeDef
-]
-SubSlotSettingUnionTypeDef = Union[SubSlotSettingTypeDef, SubSlotSettingOutputTypeDef]
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
+):
+    pass
+
+
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
         "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_RequiredSlotValueElicitationSettingOutputTypeDef",
-    {
-        "slotConstraint": SlotConstraintType,
-    },
-)
-_OptionalSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_OptionalSlotValueElicitationSettingOutputTypeDef",
-    {
-        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
-        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SlotValueElicitationSettingOutputTypeDef(
-    _RequiredSlotValueElicitationSettingOutputTypeDef,
-    _OptionalSlotValueElicitationSettingOutputTypeDef,
-):
-    pass
-
-
-InitialResponseSettingUnionTypeDef = Union[
-    InitialResponseSettingTypeDef, InitialResponseSettingOutputTypeDef
-]
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
+        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
 
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
 ):
     pass
 
 
-IntentConfirmationSettingUnionTypeDef = Union[
-    IntentConfirmationSettingTypeDef, IntentConfirmationSettingOutputTypeDef
-]
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
-    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
+        "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
+        "slotPriorities": List[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -6279,131 +6258,129 @@
 
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
 
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
+    },
+)
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
+):
+    pass
+
+
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
+        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
 
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
 ):
     pass
 
 
-SlotValueElicitationSettingUnionTypeDef = Union[
-    SlotValueElicitationSettingTypeDef, SlotValueElicitationSettingOutputTypeDef
-]
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
+        "description": str,
+        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-    },
-)
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/type_defs.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,59 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportStatusType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterOperatorType,
@@ -63,14 +86,15 @@
     TestResultTypeFilterType,
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
+    UtteranceContentTypeType,
     VoiceEngineType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -84,14 +108,40 @@
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
     "AggregatedUtterancesSummaryTypeDef",
     "AllowedInputTypesTypeDef",
+    "AnalyticsBinBySpecificationTypeDef",
+    "AnalyticsBinKeyTypeDef",
+    "AnalyticsIntentFilterTypeDef",
+    "AnalyticsIntentGroupByKeyTypeDef",
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    "AnalyticsIntentMetricResultTypeDef",
+    "AnalyticsIntentMetricTypeDef",
+    "AnalyticsIntentNodeSummaryTypeDef",
+    "AnalyticsIntentStageFilterTypeDef",
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    "AnalyticsIntentStageMetricResultTypeDef",
+    "AnalyticsIntentStageMetricTypeDef",
+    "AnalyticsPathFilterTypeDef",
+    "AnalyticsSessionFilterTypeDef",
+    "AnalyticsSessionGroupByKeyTypeDef",
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    "AnalyticsSessionMetricResultTypeDef",
+    "AnalyticsSessionMetricTypeDef",
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    "AnalyticsUtteranceAttributeTypeDef",
+    "AnalyticsUtteranceFilterTypeDef",
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    "AnalyticsUtteranceMetricResultTypeDef",
+    "AnalyticsUtteranceMetricTypeDef",
     "AssociatedTranscriptFilterTypeDef",
     "AssociatedTranscriptTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemTypeDef",
@@ -129,30 +179,29 @@
     "LambdaCodeHookTypeDef",
     "SubSlotTypeCompositionTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
-    "ConversationLogsDataSourceFilterByOutputTypeDef",
-    "TimestampTypeDef",
+    "ConversationLogsDataSourceFilterByTypeDef",
     "SentimentAnalysisSettingsTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
     "PrincipalTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
-    "DateRangeFilterOutputTypeDef",
+    "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
     "DeleteExportRequestRequestTypeDef",
     "DeleteImportRequestRequestTypeDef",
@@ -181,47 +230,49 @@
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionTypeDef",
-    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
     "IntentSortByTypeDef",
+    "InvokedIntentSampleTypeDef",
     "ListBotAliasesRequestRequestTypeDef",
     "ListBotRecommendationsRequestRequestTypeDef",
     "ListCustomVocabularyItemsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListRecommendedIntentsRequestRequestTypeDef",
     "RecommendedIntentSummaryTypeDef",
+    "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
+    "UtteranceDataSortByTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
-    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
@@ -237,14 +288,18 @@
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
+    "AnalyticsIntentResultTypeDef",
+    "AnalyticsIntentStageResultTypeDef",
+    "AnalyticsSessionResultTypeDef",
+    "AnalyticsUtteranceResultTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
@@ -263,22 +318,22 @@
     "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementResponseTypeDef",
     "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetTestExecutionArtifactsUrlResponseTypeDef",
     "ListCustomVocabularyItemsResponseTypeDef",
+    "ListIntentPathsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetTypeDef",
-    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
     "BotLocaleImportSpecificationTypeDef",
     "CreateBotLocaleRequestRequestTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
     "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
@@ -297,220 +352,183 @@
     "CreateBotVersionResponseTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
-    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "TextLogDestinationTypeDef",
     "CodeHookSpecificationTypeDef",
-    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
-    "ConversationLogsDataSourceOutputTypeDef",
-    "ConversationLogsDataSourceFilterByTypeDef",
-    "DateRangeFilterTypeDef",
+    "ConversationLogsDataSourceTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
-    "LexTranscriptFilterOutputTypeDef",
+    "LexTranscriptFilterTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
     "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
-    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
     "IntentClassificationTestResultItemTypeDef",
     "ListIntentsRequestRequestTypeDef",
+    "SessionSpecificationTypeDef",
+    "ListIntentMetricsRequestRequestTypeDef",
+    "ListIntentPathsRequestRequestTypeDef",
+    "ListIntentStageMetricsRequestRequestTypeDef",
+    "ListSessionMetricsRequestRequestTypeDef",
+    "ListUtteranceMetricsRequestRequestTypeDef",
     "ListRecommendedIntentsResponseTypeDef",
+    "ListSessionAnalyticsDataRequestRequestTypeDef",
     "ListSlotTypesRequestRequestTypeDef",
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
+    "ListUtteranceAnalyticsDataRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
-    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
-    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
-    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
-    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
+    "ListIntentMetricsResponseTypeDef",
+    "ListIntentStageMetricsResponseTypeDef",
+    "ListSessionMetricsResponseTypeDef",
+    "ListUtteranceMetricsResponseTypeDef",
     "PromptAttemptSpecificationTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
     "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
     "BotRecommendationResultsTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
+    "UtteranceBotResponseTypeDef",
     "TextLogSettingTypeDef",
     "BotAliasLocaleSettingsTypeDef",
-    "CompositeSlotTypeSettingUnionTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
-    "TestSetGenerationDataSourceOutputTypeDef",
-    "ConversationLogsDataSourceTypeDef",
-    "LexTranscriptFilterTypeDef",
+    "TestSetGenerationDataSourceTypeDef",
     "ListIntentsResponseTypeDef",
-    "TranscriptFilterOutputTypeDef",
+    "TranscriptFilterTypeDef",
     "ListTestSetsResponseTypeDef",
     "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
+    "ListSessionAnalyticsDataResponseTypeDef",
     "ListAggregatedUtterancesRequestRequestTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
-    "SlotTypeValueUnionTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
-    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
-    "MessageGroupOutputTypeDef",
     "MessageGroupTypeDef",
-    "ConversationLogSettingsOutputTypeDef",
+    "UtteranceSpecificationTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
-    "TestSetGenerationDataSourceTypeDef",
-    "TranscriptFilterTypeDef",
-    "S3BucketTranscriptSourceOutputTypeDef",
+    "S3BucketTranscriptSourceTypeDef",
     "ListExportsResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeResponseTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportResponseTypeDef",
-    "ImportResourceSpecificationUnionTypeDef",
     "StartImportRequestRequestTypeDef",
+    "StartImportResponseTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
-    "FulfillmentStartResponseSpecificationOutputTypeDef",
-    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
-    "PromptSpecificationOutputTypeDef",
-    "ResponseSpecificationOutputTypeDef",
-    "StillWaitingResponseSpecificationOutputTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
+    "ListUtteranceAnalyticsDataResponseTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasResponseTypeDef",
-    "ConversationLogSettingsUnionTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasRequestRequestTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
-    "TestSetGenerationDataSourceUnionTypeDef",
-    "S3BucketTranscriptSourceTypeDef",
-    "TranscriptSourceSettingOutputTypeDef",
+    "UpdateBotAliasResponseTypeDef",
+    "TranscriptSourceSettingTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationOutputTypeDef",
-    "SlotSummaryTypeDef",
-    "ConditionalBranchOutputTypeDef",
-    "DefaultConditionalBranchOutputTypeDef",
-    "WaitAndContinueSpecificationOutputTypeDef",
     "FulfillmentUpdatesSpecificationTypeDef",
+    "SlotSummaryTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
-    "TranscriptSourceSettingTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
-    "ConditionalSpecificationOutputTypeDef",
-    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
-    "TranscriptSourceSettingUnionTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
-    "IntentClosingSettingOutputTypeDef",
-    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
-    "PostFulfillmentStatusSpecificationOutputTypeDef",
-    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
-    "DialogCodeHookInvocationSettingOutputTypeDef",
-    "FulfillmentCodeHookSettingsOutputTypeDef",
-    "SubSlotSettingOutputTypeDef",
-    "IntentClosingSettingUnionTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
-    "InitialResponseSettingOutputTypeDef",
-    "IntentConfirmationSettingOutputTypeDef",
-    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "FulfillmentCodeHookSettingsUnionTypeDef",
-    "SubSlotSettingUnionTypeDef",
+    "CreateIntentRequestRequestTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentResponseTypeDef",
-    "SlotValueElicitationSettingOutputTypeDef",
-    "InitialResponseSettingUnionTypeDef",
-    "CreateIntentRequestRequestTypeDef",
-    "IntentConfirmationSettingUnionTypeDef",
     "UpdateIntentRequestRequestTypeDef",
+    "UpdateIntentResponseTypeDef",
     "SlotValueElicitationSettingTypeDef",
+    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotResponseTypeDef",
-    "CreateSlotRequestRequestTypeDef",
-    "SlotValueElicitationSettingUnionTypeDef",
     "UpdateSlotRequestRequestTypeDef",
+    "UpdateSlotResponseTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
@@ -573,14 +591,299 @@
     "AllowedInputTypesTypeDef",
     {
         "allowAudioInput": bool,
         "allowDTMFInput": bool,
     },
 )
 
+_RequiredAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_RequiredAnalyticsBinBySpecificationTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "interval": AnalyticsIntervalType,
+    },
+)
+_OptionalAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_OptionalAnalyticsBinBySpecificationTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsBinBySpecificationTypeDef(
+    _RequiredAnalyticsBinBySpecificationTypeDef, _OptionalAnalyticsBinBySpecificationTypeDef
+):
+    pass
+
+AnalyticsBinKeyTypeDef = TypedDict(
+    "AnalyticsBinKeyTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "value": int,
+    },
+    total=False,
+)
+
+AnalyticsIntentFilterTypeDef = TypedDict(
+    "AnalyticsIntentFilterTypeDef",
+    {
+        "name": AnalyticsIntentFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsIntentGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+    },
+)
+
+AnalyticsIntentMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsIntentMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentMetricTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsIntentMetricTypeDef(
+    _RequiredAnalyticsIntentMetricTypeDef, _OptionalAnalyticsIntentMetricTypeDef
+):
+    pass
+
+AnalyticsIntentNodeSummaryTypeDef = TypedDict(
+    "AnalyticsIntentNodeSummaryTypeDef",
+    {
+        "intentName": str,
+        "intentPath": str,
+        "intentCount": int,
+        "intentLevel": int,
+        "nodeType": AnalyticsNodeTypeType,
+    },
+    total=False,
+)
+
+AnalyticsIntentStageFilterTypeDef = TypedDict(
+    "AnalyticsIntentStageFilterTypeDef",
+    {
+        "name": AnalyticsIntentStageFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentStageGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsIntentStageGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+    },
+)
+
+AnalyticsIntentStageMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentStageMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentStageMetricTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentStageMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsIntentStageMetricTypeDef(
+    _RequiredAnalyticsIntentStageMetricTypeDef, _OptionalAnalyticsIntentStageMetricTypeDef
+):
+    pass
+
+AnalyticsPathFilterTypeDef = TypedDict(
+    "AnalyticsPathFilterTypeDef",
+    {
+        "name": AnalyticsCommonFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionFilterTypeDef = TypedDict(
+    "AnalyticsSessionFilterTypeDef",
+    {
+        "name": AnalyticsSessionFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionGroupByKeyTypeDef = TypedDict(
+    "AnalyticsSessionGroupByKeyTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsSessionGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+    },
+)
+
+AnalyticsSessionMetricResultTypeDef = TypedDict(
+    "AnalyticsSessionMetricResultTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsSessionMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsSessionMetricTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsSessionMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsSessionMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsSessionMetricTypeDef(
+    _RequiredAnalyticsSessionMetricTypeDef, _OptionalAnalyticsSessionMetricTypeDef
+):
+    pass
+
+AnalyticsUtteranceAttributeResultTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    {
+        "lastUsedIntent": str,
+    },
+    total=False,
+)
+
+AnalyticsUtteranceAttributeTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeTypeDef",
+    {
+        "name": Literal["LastUsedIntent"],
+    },
+)
+
+AnalyticsUtteranceFilterTypeDef = TypedDict(
+    "AnalyticsUtteranceFilterTypeDef",
+    {
+        "name": AnalyticsUtteranceFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsUtteranceGroupByKeyTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+        "value": str,
+    },
+    total=False,
+)
+
+AnalyticsUtteranceGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+    },
+)
+
+AnalyticsUtteranceMetricResultTypeDef = TypedDict(
+    "AnalyticsUtteranceMetricResultTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+    total=False,
+)
+
+_RequiredAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsUtteranceMetricTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsUtteranceMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsUtteranceMetricTypeDef(
+    _RequiredAnalyticsUtteranceMetricTypeDef, _OptionalAnalyticsUtteranceMetricTypeDef
+):
+    pass
+
 AssociatedTranscriptFilterTypeDef = TypedDict(
     "AssociatedTranscriptFilterTypeDef",
     {
         "name": AssociatedTranscriptFilterNameType,
         "values": Sequence[str],
     },
 )
@@ -1040,24 +1343,23 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByOutputTypeDef",
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
@@ -1164,16 +1466,16 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterOutputTypeDef = TypedDict(
-    "DateRangeFilterOutputTypeDef",
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
@@ -1578,23 +1880,14 @@
     },
     total=False,
 )
 
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-IntentOverrideOutputTypeDef = TypedDict(
-    "IntentOverrideOutputTypeDef",
-    {
-        "name": str,
-        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
-    },
-    total=False,
-)
-
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
     total=False,
@@ -1745,14 +2038,22 @@
     "IntentSortByTypeDef",
     {
         "attribute": IntentSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+InvokedIntentSampleTypeDef = TypedDict(
+    "InvokedIntentSampleTypeDef",
+    {
+        "intentName": str,
+    },
+    total=False,
+)
+
 _RequiredListBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotAliasesRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotAliasesRequestRequestTypeDef = TypedDict(
@@ -1811,14 +2112,15 @@
 
 class ListCustomVocabularyItemsRequestRequestTypeDef(
     _RequiredListCustomVocabularyItemsRequestRequestTypeDef,
     _OptionalListCustomVocabularyItemsRequestRequestTypeDef,
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredListRecommendedIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendedIntentsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -1845,14 +2147,22 @@
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
     total=False,
 )
 
+SessionDataSortByTypeDef = TypedDict(
+    "SessionDataSortByTypeDef",
+    {
+        "name": AnalyticsSessionSortByNameType,
+        "order": AnalyticsSortOrderType,
+    },
+)
+
 SlotTypeFilterTypeDef = TypedDict(
     "SlotTypeFilterTypeDef",
     {
         "name": SlotTypeFilterNameType,
         "values": Sequence[str],
         "operator": SlotTypeFilterOperatorType,
     },
@@ -1936,14 +2246,22 @@
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+UtteranceDataSortByTypeDef = TypedDict(
+    "UtteranceDataSortByTypeDef",
+    {
+        "name": Literal["UtteranceTimestamp"],
+        "order": AnalyticsSortOrderType,
+    },
+)
+
 PlainTextMessageTypeDef = TypedDict(
     "PlainTextMessageTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1971,26 +2289,18 @@
 )
 
 class OverallTestResultItemTypeDef(
     _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
 ):
     pass
 
-PathFormatOutputTypeDef = TypedDict(
-    "PathFormatOutputTypeDef",
-    {
-        "objectPrefixes": List[str],
-    },
-    total=False,
-)
-
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": Sequence[str],
+        "objectPrefixes": List[str],
     },
     total=False,
 )
 
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
@@ -2235,14 +2545,55 @@
     },
     total=False,
 )
 
 class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
     pass
 
+AnalyticsIntentResultTypeDef = TypedDict(
+    "AnalyticsIntentResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsIntentStageResultTypeDef = TypedDict(
+    "AnalyticsIntentStageResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsSessionResultTypeDef = TypedDict(
+    "AnalyticsSessionResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsSessionGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsSessionMetricResultTypeDef],
+    },
+    total=False,
+)
+
+AnalyticsUtteranceResultTypeDef = TypedDict(
+    "AnalyticsUtteranceResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsUtteranceGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsUtteranceMetricResultTypeDef],
+        "attributeResults": List[AnalyticsUtteranceAttributeResultTypeDef],
+    },
+    total=False,
+)
+
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2521,14 +2872,22 @@
         "localeId": str,
         "customVocabularyItems": List[CustomVocabularyItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2592,51 +2951,28 @@
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
-_RequiredBotImportSpecificationOutputTypeDef = TypedDict(
-    "_RequiredBotImportSpecificationOutputTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-    },
-)
-_OptionalBotImportSpecificationOutputTypeDef = TypedDict(
-    "_OptionalBotImportSpecificationOutputTypeDef",
-    {
-        "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
-    },
-    total=False,
-)
-
-class BotImportSpecificationOutputTypeDef(
-    _RequiredBotImportSpecificationOutputTypeDef, _OptionalBotImportSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
     },
     total=False,
 )
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
@@ -3074,35 +3410,14 @@
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
-    pass
-
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
@@ -3130,22 +3445,14 @@
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
-CompositeSlotTypeSettingOutputTypeDef = TypedDict(
-    "CompositeSlotTypeSettingOutputTypeDef",
-    {
-        "subSlots": List[SubSlotTypeCompositionTypeDef],
-    },
-    total=False,
-)
-
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
@@ -3187,38 +3494,21 @@
 )
 
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
-ConversationLogsDataSourceOutputTypeDef = TypedDict(
-    "ConversationLogsDataSourceOutputTypeDef",
+ConversationLogsDataSourceTypeDef = TypedDict(
+    "ConversationLogsDataSourceTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
-    },
-)
-
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
-    {
-        "startTime": TimestampTypeDef,
-        "endTime": TimestampTypeDef,
-        "inputMode": ConversationLogsInputModeFilterType,
-    },
-)
-
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
-    {
-        "startDateTime": TimestampTypeDef,
-        "endDateTime": TimestampTypeDef,
+        "filter": ConversationLogsDataSourceFilterByTypeDef,
     },
 )
 
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
@@ -3253,18 +3543,18 @@
 
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-LexTranscriptFilterOutputTypeDef = TypedDict(
-    "LexTranscriptFilterOutputTypeDef",
+LexTranscriptFilterTypeDef = TypedDict(
+    "LexTranscriptFilterTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterOutputTypeDef,
+        "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef = TypedDict(
     "_RequiredDescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     {
@@ -3511,24 +3801,14 @@
         "storageLocation": TestSetStorageLocationTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialogStateOutputTypeDef = TypedDict(
-    "DialogStateOutputTypeDef",
-    {
-        "dialogAction": DialogActionTypeDef,
-        "intent": IntentOverrideOutputTypeDef,
-        "sessionAttributes": Dict[str, str],
-    },
-    total=False,
-)
-
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
         "sessionAttributes": Mapping[str, str],
     },
@@ -3633,27 +3913,202 @@
 )
 
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
+SessionSpecificationTypeDef = TypedDict(
+    "SessionSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "channel": str,
+        "sessionId": str,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "conversationDurationSeconds": int,
+        "conversationEndState": ConversationEndStateType,
+        "mode": AnalyticsModalityType,
+        "numberOfTurns": int,
+        "invokedIntentSamples": List[InvokedIntentSampleTypeDef],
+        "originatingRequestId": str,
+    },
+    total=False,
+)
+
+_RequiredListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsIntentMetricTypeDef],
+    },
+)
+_OptionalListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListIntentMetricsRequestRequestTypeDef(
+    _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentPathsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "intentPath": str,
+    },
+)
+_OptionalListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentPathsRequestRequestTypeDef",
+    {
+        "filters": Sequence[AnalyticsPathFilterTypeDef],
+    },
+    total=False,
+)
+
+class ListIntentPathsRequestRequestTypeDef(
+    _RequiredListIntentPathsRequestRequestTypeDef, _OptionalListIntentPathsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsIntentStageMetricTypeDef],
+    },
+)
+_OptionalListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentStageFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListIntentStageMetricsRequestRequestTypeDef(
+    _RequiredListIntentStageMetricsRequestRequestTypeDef,
+    _OptionalListIntentStageMetricsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsSessionMetricTypeDef],
+    },
+)
+_OptionalListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsSessionGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListSessionMetricsRequestRequestTypeDef(
+    _RequiredListSessionMetricsRequestRequestTypeDef,
+    _OptionalListSessionMetricsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+        "metrics": Sequence[AnalyticsUtteranceMetricTypeDef],
+    },
+)
+_OptionalListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef],
+        "attributes": Sequence[AnalyticsUtteranceAttributeTypeDef],
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListUtteranceMetricsRequestRequestTypeDef(
+    _RequiredListUtteranceMetricsRequestRequestTypeDef,
+    _OptionalListUtteranceMetricsRequestRequestTypeDef,
+):
+    pass
+
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+    },
+)
+_OptionalListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": SessionDataSortByTypeDef,
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListSessionAnalyticsDataRequestRequestTypeDef(
+    _RequiredListSessionAnalyticsDataRequestRequestTypeDef,
+    _OptionalListSessionAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3727,14 +4182,39 @@
         "sortBy": TestSetSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
+    },
+)
+_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": UtteranceDataSortByTypeDef,
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListUtteranceAnalyticsDataRequestRequestTypeDef(
+    _RequiredListUtteranceAnalyticsDataRequestRequestTypeDef,
+    _OptionalListUtteranceAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
 OverallTestResultsTypeDef = TypedDict(
     "OverallTestResultsTypeDef",
     {
         "items": List[OverallTestResultItemTypeDef],
     },
 )
 
@@ -3750,39 +4230,23 @@
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
-SlotTypeValueOutputTypeDef = TypedDict(
-    "SlotTypeValueOutputTypeDef",
-    {
-        "sampleValue": SampleValueTypeDef,
-        "synonyms": List[SampleValueTypeDef],
-    },
-    total=False,
-)
-
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
-SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
-    "SlotDefaultValueSpecificationOutputTypeDef",
-    {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
-    },
-)
-
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3790,24 +4254,14 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
-SlotValueOverrideOutputTypeDef = TypedDict(
-    "SlotValueOverrideOutputTypeDef",
-    {
-        "shape": SlotShapeType,
-        "value": SlotValueTypeDef,
-        "values": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
@@ -3846,54 +4300,29 @@
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
-_RequiredTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
-    "_RequiredTestSetImportResourceSpecificationOutputTypeDef",
-    {
-        "testSetName": str,
-        "roleArn": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "importInputLocation": TestSetImportInputLocationTypeDef,
-        "modality": TestSetModalityType,
-    },
-)
-_OptionalTestSetImportResourceSpecificationOutputTypeDef = TypedDict(
-    "_OptionalTestSetImportResourceSpecificationOutputTypeDef",
-    {
-        "description": str,
-        "testSetTags": Dict[str, str],
-    },
-    total=False,
-)
-
-class TestSetImportResourceSpecificationOutputTypeDef(
-    _RequiredTestSetImportResourceSpecificationOutputTypeDef,
-    _OptionalTestSetImportResourceSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Mapping[str, str],
+        "testSetTags": Dict[str, str],
     },
     total=False,
 )
 
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
     _OptionalTestSetImportResourceSpecificationTypeDef,
@@ -3925,14 +4354,54 @@
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
     total=False,
 )
 
+ListIntentMetricsResponseTypeDef = TypedDict(
+    "ListIntentMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIntentStageMetricsResponseTypeDef = TypedDict(
+    "ListIntentStageMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentStageResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionMetricsResponseTypeDef = TypedDict(
+    "ListSessionMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsSessionResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUtteranceMetricsResponseTypeDef = TypedDict(
+    "ListUtteranceMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsUtteranceResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPromptAttemptSpecificationTypeDef = TypedDict(
     "_RequiredPromptAttemptSpecificationTypeDef",
     {
         "allowedInputTypes": AllowedInputTypesTypeDef,
     },
 )
 _OptionalPromptAttemptSpecificationTypeDef = TypedDict(
@@ -4032,31 +4501,30 @@
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
     total=False,
 )
 
-MessageOutputTypeDef = TypedDict(
-    "MessageOutputTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
-        "imageResponseCard": ImageResponseCardOutputTypeDef,
+        "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+UtteranceBotResponseTypeDef = TypedDict(
+    "UtteranceBotResponseTypeDef",
     {
-        "plainTextMessage": PlainTextMessageTypeDef,
-        "customPayload": CustomPayloadTypeDef,
-        "ssmlMessage": SSMLMessageTypeDef,
+        "content": str,
+        "contentType": UtteranceContentTypeType,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
 TextLogSettingTypeDef = TypedDict(
     "TextLogSettingTypeDef",
@@ -4081,17 +4549,14 @@
 )
 
 class BotAliasLocaleSettingsTypeDef(
     _RequiredBotAliasLocaleSettingsTypeDef, _OptionalBotAliasLocaleSettingsTypeDef
 ):
     pass
 
-CompositeSlotTypeSettingUnionTypeDef = Union[
-    CompositeSlotTypeSettingTypeDef, CompositeSlotTypeSettingOutputTypeDef
-]
 ConversationLevelTestResultsTypeDef = TypedDict(
     "ConversationLevelTestResultsTypeDef",
     {
         "items": List[ConversationLevelTestResultItemTypeDef],
     },
 )
 
@@ -4113,36 +4578,18 @@
 
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
-TestSetGenerationDataSourceOutputTypeDef = TypedDict(
-    "TestSetGenerationDataSourceOutputTypeDef",
-    {
-        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
-    },
-    total=False,
-)
-
-ConversationLogsDataSourceTypeDef = TypedDict(
-    "ConversationLogsDataSourceTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "filter": ConversationLogsDataSourceFilterByTypeDef,
-    },
-)
-
-LexTranscriptFilterTypeDef = TypedDict(
-    "LexTranscriptFilterTypeDef",
+TestSetGenerationDataSourceTypeDef = TypedDict(
+    "TestSetGenerationDataSourceTypeDef",
     {
-        "dateRangeFilter": DateRangeFilterTypeDef,
+        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
 
 ListIntentsResponseTypeDef = TypedDict(
     "ListIntentsResponseTypeDef",
     {
@@ -4151,18 +4598,18 @@
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TranscriptFilterOutputTypeDef = TypedDict(
-    "TranscriptFilterOutputTypeDef",
+TranscriptFilterTypeDef = TypedDict(
+    "TranscriptFilterTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
+        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
     total=False,
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
@@ -4256,14 +4703,24 @@
 IntentClassificationTestResultsTypeDef = TypedDict(
     "IntentClassificationTestResultsTypeDef",
     {
         "items": List[IntentClassificationTestResultItemTypeDef],
     },
 )
 
+ListSessionAnalyticsDataResponseTypeDef = TypedDict(
+    "ListSessionAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "sessions": List[SessionSpecificationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
     },
@@ -4300,15 +4757,14 @@
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeValueUnionTypeDef = Union[SlotTypeValueTypeDef, SlotTypeValueOutputTypeDef]
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
@@ -4345,25 +4801,14 @@
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportResourceSpecificationOutputTypeDef = TypedDict(
-    "ImportResourceSpecificationOutputTypeDef",
-    {
-        "botImportSpecification": BotImportSpecificationOutputTypeDef,
-        "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
-        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
-        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
         "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
         "testSetImportResourceSpecification": TestSetImportResourceSpecificationTypeDef,
@@ -4396,33 +4841,14 @@
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageGroupOutputTypeDef = TypedDict(
-    "_RequiredMessageGroupOutputTypeDef",
-    {
-        "message": MessageOutputTypeDef,
-    },
-)
-_OptionalMessageGroupOutputTypeDef = TypedDict(
-    "_OptionalMessageGroupOutputTypeDef",
-    {
-        "variations": List[MessageOutputTypeDef],
-    },
-    total=False,
-)
-
-class MessageGroupOutputTypeDef(
-    _RequiredMessageGroupOutputTypeDef, _OptionalMessageGroupOutputTypeDef
-):
-    pass
-
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
@@ -4432,19 +4858,39 @@
     },
     total=False,
 )
 
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
-ConversationLogSettingsOutputTypeDef = TypedDict(
-    "ConversationLogSettingsOutputTypeDef",
+UtteranceSpecificationTypeDef = TypedDict(
+    "UtteranceSpecificationTypeDef",
     {
-        "textLogSettings": List[TextLogSettingTypeDef],
-        "audioLogSettings": List[AudioLogSettingTypeDef],
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "sessionId": str,
+        "channel": str,
+        "mode": AnalyticsModalityType,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "utterance": str,
+        "utteranceTimestamp": datetime,
+        "audioVoiceDurationMillis": int,
+        "utteranceUnderstood": bool,
+        "inputType": str,
+        "outputType": str,
+        "associatedIntentName": str,
+        "associatedSlotName": str,
+        "intentState": IntentStateType,
+        "dialogActionType": str,
+        "botResponseAudioVoiceId": str,
+        "slotsFilledInSession": str,
+        "utteranceRequestId": str,
+        "botResponses": List[UtteranceBotResponseTypeDef],
     },
     total=False,
 )
 
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
@@ -4460,73 +4906,81 @@
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
-        "description": str,
         "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-TestSetGenerationDataSourceTypeDef = TypedDict(
-    "TestSetGenerationDataSourceTypeDef",
+_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
     {
-        "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
+        "description": str,
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
-TranscriptFilterTypeDef = TypedDict(
-    "TranscriptFilterTypeDef",
+class StartTestSetGenerationRequestRequestTypeDef(
+    _RequiredStartTestSetGenerationRequestRequestTypeDef,
+    _OptionalStartTestSetGenerationRequestRequestTypeDef,
+):
+    pass
+
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
     {
-        "lexTranscriptFilter": LexTranscriptFilterTypeDef,
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
+        "testSetName": str,
+        "description": str,
+        "storageLocation": TestSetStorageLocationTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredS3BucketTranscriptSourceOutputTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceOutputTypeDef",
+_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_RequiredS3BucketTranscriptSourceTypeDef",
     {
         "s3BucketName": str,
         "transcriptFormat": Literal["Lex"],
     },
 )
-_OptionalS3BucketTranscriptSourceOutputTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceOutputTypeDef",
+_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
+    "_OptionalS3BucketTranscriptSourceTypeDef",
     {
-        "pathFormat": PathFormatOutputTypeDef,
-        "transcriptFilter": TranscriptFilterOutputTypeDef,
+        "pathFormat": PathFormatTypeDef,
+        "transcriptFilter": TranscriptFilterTypeDef,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-class S3BucketTranscriptSourceOutputTypeDef(
-    _RequiredS3BucketTranscriptSourceOutputTypeDef, _OptionalS3BucketTranscriptSourceOutputTypeDef
+class S3BucketTranscriptSourceTypeDef(
+    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
 ):
     pass
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "botId": str,
@@ -4534,166 +4988,151 @@
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
+    },
+)
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
+):
+    pass
+
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
-    {
         "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueUnionTypeDef],
+        "slotTypeValues": List[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
-):
-    pass
-
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "resourceSpecification": ImportResourceSpecificationTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportResourceSpecificationUnionTypeDef = Union[
-    ImportResourceSpecificationTypeDef, ImportResourceSpecificationOutputTypeDef
-]
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4707,14 +5146,26 @@
 )
 
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUserTurnResultTypeDef = TypedDict(
     "_RequiredUserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
     },
 )
@@ -4739,119 +5190,14 @@
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
-_RequiredFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentStartResponseSpecificationOutputTypeDef",
-    {
-        "delayInSeconds": int,
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalFulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentStartResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-class FulfillmentStartResponseSpecificationOutputTypeDef(
-    _RequiredFulfillmentStartResponseSpecificationOutputTypeDef,
-    _OptionalFulfillmentStartResponseSpecificationOutputTypeDef,
-):
-    pass
-
-_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef",
-    {
-        "frequencyInSeconds": int,
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-class FulfillmentUpdateResponseSpecificationOutputTypeDef(
-    _RequiredFulfillmentUpdateResponseSpecificationOutputTypeDef,
-    _OptionalFulfillmentUpdateResponseSpecificationOutputTypeDef,
-):
-    pass
-
-_RequiredPromptSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPromptSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-        "maxRetries": int,
-    },
-)
-_OptionalPromptSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPromptSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-        "messageSelectionStrategy": MessageSelectionStrategyType,
-        "promptAttemptsSpecification": Dict[PromptAttemptType, PromptAttemptSpecificationTypeDef],
-    },
-    total=False,
-)
-
-class PromptSpecificationOutputTypeDef(
-    _RequiredPromptSpecificationOutputTypeDef, _OptionalPromptSpecificationOutputTypeDef
-):
-    pass
-
-_RequiredResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredResponseSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-    },
-)
-_OptionalResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-class ResponseSpecificationOutputTypeDef(
-    _RequiredResponseSpecificationOutputTypeDef, _OptionalResponseSpecificationOutputTypeDef
-):
-    pass
-
-_RequiredStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
-    "_RequiredStillWaitingResponseSpecificationOutputTypeDef",
-    {
-        "messageGroups": List[MessageGroupOutputTypeDef],
-        "frequencyInSeconds": int,
-        "timeoutInSeconds": int,
-    },
-)
-_OptionalStillWaitingResponseSpecificationOutputTypeDef = TypedDict(
-    "_OptionalStillWaitingResponseSpecificationOutputTypeDef",
-    {
-        "allowInterrupt": bool,
-    },
-    total=False,
-)
-
-class StillWaitingResponseSpecificationOutputTypeDef(
-    _RequiredStillWaitingResponseSpecificationOutputTypeDef,
-    _OptionalStillWaitingResponseSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4951,98 +5297,87 @@
 
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
-CreateBotAliasResponseTypeDef = TypedDict(
-    "CreateBotAliasResponseTypeDef",
+ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
+    "ListUtteranceAnalyticsDataResponseTypeDef",
     {
-        "botAliasId": str,
-        "botAliasName": str,
-        "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
         "botId": str,
-        "creationDateTime": datetime,
-        "tags": Dict[str, str],
+        "nextToken": str,
+        "utterances": List[UtteranceSpecificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBotAliasResponseTypeDef = TypedDict(
-    "DescribeBotAliasResponseTypeDef",
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
     {
-        "botAliasId": str,
         "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
+    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
+):
+    pass
+
+CreateBotAliasResponseTypeDef = TypedDict(
+    "CreateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConversationLogSettingsUnionTypeDef = Union[
-    ConversationLogSettingsTypeDef, ConversationLogSettingsOutputTypeDef
-]
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
+DescribeBotAliasResponseTypeDef = TypedDict(
+    "DescribeBotAliasResponseTypeDef",
     {
+        "botAliasId": str,
         "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
+        "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "parentBotNetworks": List[ParentBotNetworkTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "botId": str,
     },
@@ -5060,67 +5395,36 @@
 )
 
 class UpdateBotAliasRequestRequestTypeDef(
     _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestSetGenerationRequestRequestTypeDef",
-    {
-        "testSetName": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-    },
-)
-_OptionalStartTestSetGenerationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestSetGenerationRequestRequestTypeDef",
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
     {
+        "botAliasId": str,
+        "botAliasName": str,
         "description": str,
-        "testSetTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartTestSetGenerationRequestRequestTypeDef(
-    _RequiredStartTestSetGenerationRequestRequestTypeDef,
-    _OptionalStartTestSetGenerationRequestRequestTypeDef,
-):
-    pass
-
-TestSetGenerationDataSourceUnionTypeDef = Union[
-    TestSetGenerationDataSourceTypeDef, TestSetGenerationDataSourceOutputTypeDef
-]
-_RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_RequiredS3BucketTranscriptSourceTypeDef",
-    {
-        "s3BucketName": str,
-        "transcriptFormat": Literal["Lex"],
-    },
-)
-_OptionalS3BucketTranscriptSourceTypeDef = TypedDict(
-    "_OptionalS3BucketTranscriptSourceTypeDef",
-    {
-        "pathFormat": PathFormatTypeDef,
-        "transcriptFilter": TranscriptFilterTypeDef,
-        "kmsKeyArn": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "conversationLogSettings": ConversationLogSettingsTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasStatus": BotAliasStatusType,
+        "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class S3BucketTranscriptSourceTypeDef(
-    _RequiredS3BucketTranscriptSourceTypeDef, _OptionalS3BucketTranscriptSourceTypeDef
-):
-    pass
-
-TranscriptSourceSettingOutputTypeDef = TypedDict(
-    "TranscriptSourceSettingOutputTypeDef",
+TranscriptSourceSettingTypeDef = TypedDict(
+    "TranscriptSourceSettingTypeDef",
     {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
     },
     total=False,
 )
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
@@ -5135,123 +5439,49 @@
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationOutputTypeDef",
+_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
     {
         "active": bool,
     },
 )
-_OptionalFulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationOutputTypeDef",
+_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
+    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
     {
-        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
+        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
         "timeoutInSeconds": int,
     },
     total=False,
 )
 
-class FulfillmentUpdatesSpecificationOutputTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationOutputTypeDef,
-    _OptionalFulfillmentUpdatesSpecificationOutputTypeDef,
+class FulfillmentUpdatesSpecificationTypeDef(
+    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
 ):
     pass
 
 SlotSummaryTypeDef = TypedDict(
     "SlotSummaryTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotConstraint": SlotConstraintType,
         "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
+        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
         "lastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredConditionalBranchOutputTypeDef = TypedDict(
-    "_RequiredConditionalBranchOutputTypeDef",
-    {
-        "name": str,
-        "condition": ConditionTypeDef,
-        "nextStep": DialogStateOutputTypeDef,
-    },
-)
-_OptionalConditionalBranchOutputTypeDef = TypedDict(
-    "_OptionalConditionalBranchOutputTypeDef",
-    {
-        "response": ResponseSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ConditionalBranchOutputTypeDef(
-    _RequiredConditionalBranchOutputTypeDef, _OptionalConditionalBranchOutputTypeDef
-):
-    pass
-
-DefaultConditionalBranchOutputTypeDef = TypedDict(
-    "DefaultConditionalBranchOutputTypeDef",
-    {
-        "nextStep": DialogStateOutputTypeDef,
-        "response": ResponseSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredWaitAndContinueSpecificationOutputTypeDef = TypedDict(
-    "_RequiredWaitAndContinueSpecificationOutputTypeDef",
-    {
-        "waitingResponse": ResponseSpecificationOutputTypeDef,
-        "continueResponse": ResponseSpecificationOutputTypeDef,
-    },
-)
-_OptionalWaitAndContinueSpecificationOutputTypeDef = TypedDict(
-    "_OptionalWaitAndContinueSpecificationOutputTypeDef",
-    {
-        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
-        "active": bool,
-    },
-    total=False,
-)
-
-class WaitAndContinueSpecificationOutputTypeDef(
-    _RequiredWaitAndContinueSpecificationOutputTypeDef,
-    _OptionalWaitAndContinueSpecificationOutputTypeDef,
-):
-    pass
-
-_RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_RequiredFulfillmentUpdatesSpecificationTypeDef",
-    {
-        "active": bool,
-    },
-)
-_OptionalFulfillmentUpdatesSpecificationTypeDef = TypedDict(
-    "_OptionalFulfillmentUpdatesSpecificationTypeDef",
-    {
-        "startResponse": FulfillmentStartResponseSpecificationTypeDef,
-        "updateResponse": FulfillmentUpdateResponseSpecificationTypeDef,
-        "timeoutInSeconds": int,
-    },
-    total=False,
-)
-
-class FulfillmentUpdatesSpecificationTypeDef(
-    _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
-):
-    pass
-
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -5295,50 +5525,65 @@
 )
 
 class WaitAndContinueSpecificationTypeDef(
     _RequiredWaitAndContinueSpecificationTypeDef, _OptionalWaitAndContinueSpecificationTypeDef
 ):
     pass
 
-TranscriptSourceSettingTypeDef = TypedDict(
-    "TranscriptSourceSettingTypeDef",
-    {
-        "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
-    },
-    total=False,
-)
-
 DescribeBotRecommendationResponseTypeDef = TypedDict(
     "DescribeBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
+    },
+)
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
+    {
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+    total=False,
+)
+
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
+):
+    pass
+
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
@@ -5346,15 +5591,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
         "encryptionSetting": EncryptionSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
     "_RequiredUtteranceLevelTestResultItemTypeDef",
@@ -5406,45 +5651,14 @@
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionalSpecificationOutputTypeDef = TypedDict(
-    "ConditionalSpecificationOutputTypeDef",
-    {
-        "active": bool,
-        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
-        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
-    },
-)
-
-_RequiredSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_RequiredSubSlotValueElicitationSettingOutputTypeDef",
-    {
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-    },
-)
-_OptionalSubSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_OptionalSubSlotValueElicitationSettingOutputTypeDef",
-    {
-        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-class SubSlotValueElicitationSettingOutputTypeDef(
-    _RequiredSubSlotValueElicitationSettingOutputTypeDef,
-    _OptionalSubSlotValueElicitationSettingOutputTypeDef,
-):
-    pass
-
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
     },
@@ -5467,40 +5681,14 @@
 )
 
 class SubSlotValueElicitationSettingTypeDef(
     _RequiredSubSlotValueElicitationSettingTypeDef, _OptionalSubSlotValueElicitationSettingTypeDef
 ):
     pass
 
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-    },
-)
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
-TranscriptSourceSettingUnionTypeDef = Union[
-    TranscriptSourceSettingTypeDef, TranscriptSourceSettingOutputTypeDef
-]
 UtteranceLevelTestResultsTypeDef = TypedDict(
     "UtteranceLevelTestResultsTypeDef",
     {
         "items": List[UtteranceLevelTestResultItemTypeDef],
     },
 )
 
@@ -5509,65 +5697,14 @@
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IntentClosingSettingOutputTypeDef = TypedDict(
-    "IntentClosingSettingOutputTypeDef",
-    {
-        "closingResponse": ResponseSpecificationOutputTypeDef,
-        "active": bool,
-        "nextStep": DialogStateOutputTypeDef,
-        "conditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
-    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
-    {
-        "successResponse": ResponseSpecificationOutputTypeDef,
-        "successNextStep": DialogStateOutputTypeDef,
-        "successConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "timeoutResponse": ResponseSpecificationOutputTypeDef,
-        "timeoutNextStep": DialogStateOutputTypeDef,
-        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
-    "PostFulfillmentStatusSpecificationOutputTypeDef",
-    {
-        "successResponse": ResponseSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "timeoutResponse": ResponseSpecificationOutputTypeDef,
-        "successNextStep": DialogStateOutputTypeDef,
-        "successConditional": ConditionalSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "timeoutNextStep": DialogStateOutputTypeDef,
-        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
-SpecificationsOutputTypeDef = TypedDict(
-    "SpecificationsOutputTypeDef",
-    {
-        "slotTypeId": str,
-        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
-    },
-)
-
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
         "active": bool,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
@@ -5623,70 +5760,14 @@
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
     total=False,
 )
 
-_RequiredDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
-    "_RequiredDialogCodeHookInvocationSettingOutputTypeDef",
-    {
-        "enableCodeHookInvocation": bool,
-        "active": bool,
-        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
-    },
-)
-_OptionalDialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
-    "_OptionalDialogCodeHookInvocationSettingOutputTypeDef",
-    {
-        "invocationLabel": str,
-    },
-    total=False,
-)
-
-class DialogCodeHookInvocationSettingOutputTypeDef(
-    _RequiredDialogCodeHookInvocationSettingOutputTypeDef,
-    _OptionalDialogCodeHookInvocationSettingOutputTypeDef,
-):
-    pass
-
-_RequiredFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentCodeHookSettingsOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalFulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentCodeHookSettingsOutputTypeDef",
-    {
-        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
-        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
-        "active": bool,
-    },
-    total=False,
-)
-
-class FulfillmentCodeHookSettingsOutputTypeDef(
-    _RequiredFulfillmentCodeHookSettingsOutputTypeDef,
-    _OptionalFulfillmentCodeHookSettingsOutputTypeDef,
-):
-    pass
-
-SubSlotSettingOutputTypeDef = TypedDict(
-    "SubSlotSettingOutputTypeDef",
-    {
-        "expression": str,
-        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
-    },
-    total=False,
-)
-
-IntentClosingSettingUnionTypeDef = Union[
-    IntentClosingSettingTypeDef, IntentClosingSettingOutputTypeDef
-]
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
         "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationTypeDef,
     },
@@ -5739,70 +5820,14 @@
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitialResponseSettingOutputTypeDef = TypedDict(
-    "InitialResponseSettingOutputTypeDef",
-    {
-        "initialResponse": ResponseSpecificationOutputTypeDef,
-        "nextStep": DialogStateOutputTypeDef,
-        "conditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredIntentConfirmationSettingOutputTypeDef = TypedDict(
-    "_RequiredIntentConfirmationSettingOutputTypeDef",
-    {
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-    },
-)
-_OptionalIntentConfirmationSettingOutputTypeDef = TypedDict(
-    "_OptionalIntentConfirmationSettingOutputTypeDef",
-    {
-        "declinationResponse": ResponseSpecificationOutputTypeDef,
-        "active": bool,
-        "confirmationResponse": ResponseSpecificationOutputTypeDef,
-        "confirmationNextStep": DialogStateOutputTypeDef,
-        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
-        "declinationNextStep": DialogStateOutputTypeDef,
-        "declinationConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
-    },
-    total=False,
-)
-
-class IntentConfirmationSettingOutputTypeDef(
-    _RequiredIntentConfirmationSettingOutputTypeDef, _OptionalIntentConfirmationSettingOutputTypeDef
-):
-    pass
-
-SlotCaptureSettingOutputTypeDef = TypedDict(
-    "SlotCaptureSettingOutputTypeDef",
-    {
-        "captureResponse": ResponseSpecificationOutputTypeDef,
-        "captureNextStep": DialogStateOutputTypeDef,
-        "captureConditional": ConditionalSpecificationOutputTypeDef,
-        "failureResponse": ResponseSpecificationOutputTypeDef,
-        "failureNextStep": DialogStateOutputTypeDef,
-        "failureConditional": ConditionalSpecificationOutputTypeDef,
-        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
-        "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
-    },
-    total=False,
-)
-
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
@@ -5851,190 +5876,156 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-FulfillmentCodeHookSettingsUnionTypeDef = Union[
-    FulfillmentCodeHookSettingsTypeDef, FulfillmentCodeHookSettingsOutputTypeDef
-]
-SubSlotSettingUnionTypeDef = Union[SubSlotSettingTypeDef, SubSlotSettingOutputTypeDef]
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
+):
+    pass
+
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
         "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
-        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
+        "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "initialResponseSetting": InitialResponseSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_RequiredSlotValueElicitationSettingOutputTypeDef",
-    {
-        "slotConstraint": SlotConstraintType,
-    },
-)
-_OptionalSlotValueElicitationSettingOutputTypeDef = TypedDict(
-    "_OptionalSlotValueElicitationSettingOutputTypeDef",
-    {
-        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
-        "promptSpecification": PromptSpecificationOutputTypeDef,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
-        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
-    },
-    total=False,
-)
-
-class SlotValueElicitationSettingOutputTypeDef(
-    _RequiredSlotValueElicitationSettingOutputTypeDef,
-    _OptionalSlotValueElicitationSettingOutputTypeDef,
-):
-    pass
-
-InitialResponseSettingUnionTypeDef = Union[
-    InitialResponseSettingTypeDef, InitialResponseSettingOutputTypeDef
-]
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
+        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
 ):
     pass
 
-IntentConfirmationSettingUnionTypeDef = Union[
-    IntentConfirmationSettingTypeDef, IntentConfirmationSettingOutputTypeDef
-]
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-    },
-)
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
-    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
+        "sampleUtterances": List[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
+        "slotPriorities": List[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
-):
-    pass
-
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -6050,128 +6041,125 @@
 )
 
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
+    },
+)
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
     },
+    total=False,
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
+):
+    pass
+
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
+        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
 ):
     pass
 
-SlotValueElicitationSettingUnionTypeDef = Union[
-    SlotValueElicitationSettingTypeDef, SlotValueElicitationSettingOutputTypeDef
-]
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
+        "description": str,
+        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-    },
-)
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.py` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models/waiter.pyi` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-models-2.5.2.post1/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt` & `types-aiobotocore-lexv2-models-2.5.2.post2/types_aiobotocore_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

