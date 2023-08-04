# Comparing `tmp/types-aiobotocore-lex-models-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lex-models-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lex-models-2.5.2.post1.tar` & `types-aiobotocore-lex-models-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.549543 types-aiobotocore-lex-models-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.549543 types-aiobotocore-lex-models-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37378 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37317 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49190 2023-08-02 14:41:52.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49130 2023-08-02 14:41:51.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:50.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.541543 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:33.000000 types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14486 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12943 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2570 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2569 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      981 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37313 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37252 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11245 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11243 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12667 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12655 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    46018 2023-08-04 13:42:32.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    45965 2023-08-04 13:42:32.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14486 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/LICENSE` & `types-aiobotocore-lex-models-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/setup.py` & `types-aiobotocore-lex-models-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-models",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__init__.pyi` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/__main__.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LexModelBuildingService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueUnionTypeDef,
-    FollowUpPromptUnionTypeDef,
+    EnumerationValueTypeDef,
+    FollowUpPromptTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,24 +78,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptUnionTypeDef,
+    PromptTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotUnionTypeDef,
+    SlotTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementUnionTypeDef,
+    StatementTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -524,16 +524,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptUnionTypeDef = ...,
-        abortStatement: StatementUnionTypeDef = ...,
+        clarificationPrompt: PromptTypeDef = ...,
+        abortStatement: StatementTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -565,20 +565,20 @@
         """
 
     async def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotUnionTypeDef] = ...,
+        slots: Sequence[SlotTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptUnionTypeDef = ...,
-        rejectionStatement: StatementUnionTypeDef = ...,
-        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
-        conclusionStatement: StatementUnionTypeDef = ...,
+        confirmationPrompt: PromptTypeDef = ...,
+        rejectionStatement: StatementTypeDef = ...,
+        followUpPrompt: FollowUpPromptTypeDef = ...,
+        conclusionStatement: StatementTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -592,15 +592,15 @@
         """
 
     async def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
+        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/client.pyi` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueUnionTypeDef,
-    FollowUpPromptUnionTypeDef,
+    EnumerationValueTypeDef,
+    FollowUpPromptTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,24 +78,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptUnionTypeDef,
+    PromptTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotUnionTypeDef,
+    SlotTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementUnionTypeDef,
+    StatementTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -482,16 +482,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: PromptUnionTypeDef = ...,
-        abortStatement: StatementUnionTypeDef = ...,
+        clarificationPrompt: PromptTypeDef = ...,
+        abortStatement: StatementTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -521,20 +521,20 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_bot_alias)
         """
     async def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[SlotUnionTypeDef] = ...,
+        slots: Sequence[SlotTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: PromptUnionTypeDef = ...,
-        rejectionStatement: StatementUnionTypeDef = ...,
-        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
-        conclusionStatement: StatementUnionTypeDef = ...,
+        confirmationPrompt: PromptTypeDef = ...,
+        rejectionStatement: StatementTypeDef = ...,
+        followUpPrompt: FollowUpPromptTypeDef = ...,
+        conclusionStatement: StatementTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -547,15 +547,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/client/#put_intent)
         """
     async def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
+        enumerationValues: Sequence[EnumerationValueTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
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
@@ -223,14 +224,15 @@
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
@@ -309,26 +311,28 @@
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

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/literals.pyi` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
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
@@ -221,14 +222,15 @@
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
@@ -307,26 +309,28 @@
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

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/paginator.pyi` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.py` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,25 +63,24 @@
     "IntentTypeDef",
     "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueOutputTypeDef",
+    "EnumerationValueTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
@@ -122,15 +121,14 @@
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
     "GetExportResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartMigrationResponseTypeDef",
-    "EnumerationValueUnionTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
@@ -143,48 +141,39 @@
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "PromptOutputTypeDef",
     "PromptTypeDef",
-    "StatementOutputTypeDef",
     "StatementTypeDef",
-    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
-    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptOutputTypeDef",
-    "GetBotResponseTypeDef",
-    "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
+    "GetBotResponseTypeDef",
     "PutBotRequestRequestTypeDef",
-    "StatementUnionTypeDef",
-    "SlotOutputTypeDef",
+    "PutBotResponseTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
-    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentResponseTypeDef",
-    "SlotUnionTypeDef",
     "PutIntentRequestRequestTypeDef",
+    "PutIntentResponseTypeDef",
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
@@ -400,32 +389,30 @@
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredEnumerationValueOutputTypeDef = TypedDict(
-    "_RequiredEnumerationValueOutputTypeDef",
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueOutputTypeDef = TypedDict(
-    "_OptionalEnumerationValueOutputTypeDef",
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
 
-class EnumerationValueOutputTypeDef(
-    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
-):
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
     pass
 
 
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
@@ -491,33 +478,14 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
-    {
-        "value": str,
-    },
-)
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
-    {
-        "synonyms": Sequence[str],
-    },
-    total=False,
-)
-
-
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
-    pass
-
-
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -1071,15 +1039,14 @@
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
 _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
@@ -1347,38 +1314,18 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPromptOutputTypeDef = TypedDict(
-    "_RequiredPromptOutputTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-        "maxAttempts": int,
-    },
-)
-_OptionalPromptOutputTypeDef = TypedDict(
-    "_OptionalPromptOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-
-class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
-    pass
-
-
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
@@ -1387,37 +1334,18 @@
 )
 
 
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
 
-_RequiredStatementOutputTypeDef = TypedDict(
-    "_RequiredStatementOutputTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-    },
-)
-_OptionalStatementOutputTypeDef = TypedDict(
-    "_OptionalStatementOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-
-class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
-    pass
-
-
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
@@ -1425,25 +1353,18 @@
 )
 
 
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
 
-SlotDefaultValueSpecOutputTypeDef = TypedDict(
-    "SlotDefaultValueSpecOutputTypeDef",
-    {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
-    },
-)
-
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
+        "defaultValueList": List[SlotDefaultValueTypeDef],
     },
 )
 
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
@@ -1528,23 +1449,22 @@
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
@@ -1553,82 +1473,47 @@
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptOutputTypeDef = TypedDict(
-    "FollowUpPromptOutputTypeDef",
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
     {
-        "prompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
-        "createVersion": bool,
         "detectSentiment": bool,
-        "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
-    {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-    },
-)
-
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
         "locale": LocaleType,
         "childDirected": bool,
     },
@@ -1656,43 +1541,41 @@
 
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
 
-StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
-_RequiredSlotOutputTypeDef = TypedDict(
-    "_RequiredSlotOutputTypeDef",
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
     {
         "name": str,
-        "slotConstraint": SlotConstraintType,
-    },
-)
-_OptionalSlotOutputTypeDef = TypedDict(
-    "_OptionalSlotOutputTypeDef",
-    {
         "description": str,
-        "slotType": str,
-        "slotTypeVersion": str,
-        "valueElicitationPrompt": PromptOutputTypeDef,
-        "priority": int,
-        "sampleUtterances": List[str],
-        "responseCard": str,
-        "obfuscationSetting": ObfuscationSettingType,
-        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
+        "intents": List[IntentTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "createVersion": bool,
+        "detectSentiment": bool,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
-    pass
-
-
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1700,15 +1583,15 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": Sequence[str],
+        "sampleUtterances": List[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
@@ -1718,15 +1601,15 @@
 
 
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
@@ -1735,15 +1618,15 @@
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
@@ -1757,15 +1640,15 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
+        "enumerationValues": Sequence[EnumerationValueTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1779,15 +1662,15 @@
 
 
 PutSlotTypeResponseTypeDef = TypedDict(
     "PutSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
@@ -1810,26 +1693,25 @@
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotOutputTypeDef],
+        "slots": List[SlotTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
@@ -1841,72 +1723,45 @@
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotOutputTypeDef],
+        "slots": List[SlotTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotOutputTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "createVersion": bool,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotUnionTypeDef],
+        "slots": Sequence[SlotTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
@@ -1921,7 +1776,34 @@
 )
 
 
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
+
+
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "createVersion": bool,
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models/type_defs.pyi` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,24 @@
     "IntentTypeDef",
     "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
-    "EnumerationValueOutputTypeDef",
+    "EnumerationValueTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
@@ -121,15 +120,14 @@
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
     "GetExportResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartMigrationResponseTypeDef",
-    "EnumerationValueUnionTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
@@ -142,48 +140,39 @@
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "PromptOutputTypeDef",
     "PromptTypeDef",
-    "StatementOutputTypeDef",
     "StatementTypeDef",
-    "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
-    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
-    "FollowUpPromptOutputTypeDef",
-    "GetBotResponseTypeDef",
-    "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
+    "GetBotResponseTypeDef",
     "PutBotRequestRequestTypeDef",
-    "StatementUnionTypeDef",
-    "SlotOutputTypeDef",
+    "PutBotResponseTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
-    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
-    "PutIntentResponseTypeDef",
-    "SlotUnionTypeDef",
     "PutIntentRequestRequestTypeDef",
+    "PutIntentResponseTypeDef",
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
@@ -389,31 +378,29 @@
 
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEnumerationValueOutputTypeDef = TypedDict(
-    "_RequiredEnumerationValueOutputTypeDef",
+_RequiredEnumerationValueTypeDef = TypedDict(
+    "_RequiredEnumerationValueTypeDef",
     {
         "value": str,
     },
 )
-_OptionalEnumerationValueOutputTypeDef = TypedDict(
-    "_OptionalEnumerationValueOutputTypeDef",
+_OptionalEnumerationValueTypeDef = TypedDict(
+    "_OptionalEnumerationValueTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-class EnumerationValueOutputTypeDef(
-    _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
-):
+class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
     pass
 
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
@@ -478,31 +465,14 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-_RequiredEnumerationValueTypeDef = TypedDict(
-    "_RequiredEnumerationValueTypeDef",
-    {
-        "value": str,
-    },
-)
-_OptionalEnumerationValueTypeDef = TypedDict(
-    "_OptionalEnumerationValueTypeDef",
-    {
-        "synonyms": Sequence[str],
-    },
-    total=False,
-)
-
-class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
-    pass
-
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -1042,15 +1012,14 @@
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
 _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
@@ -1306,95 +1275,53 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPromptOutputTypeDef = TypedDict(
-    "_RequiredPromptOutputTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-        "maxAttempts": int,
-    },
-)
-_OptionalPromptOutputTypeDef = TypedDict(
-    "_OptionalPromptOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
-    pass
-
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptTypeDef = TypedDict(
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
-_RequiredStatementOutputTypeDef = TypedDict(
-    "_RequiredStatementOutputTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-    },
-)
-_OptionalStatementOutputTypeDef = TypedDict(
-    "_OptionalStatementOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
-    pass
-
 _RequiredStatementTypeDef = TypedDict(
     "_RequiredStatementTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
     },
 )
 _OptionalStatementTypeDef = TypedDict(
     "_OptionalStatementTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
 class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
-SlotDefaultValueSpecOutputTypeDef = TypedDict(
-    "SlotDefaultValueSpecOutputTypeDef",
-    {
-        "defaultValueList": List[SlotDefaultValueTypeDef],
-    },
-)
-
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
-        "defaultValueList": Sequence[SlotDefaultValueTypeDef],
+        "defaultValueList": List[SlotDefaultValueTypeDef],
     },
 )
 
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
@@ -1477,23 +1404,22 @@
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
@@ -1502,82 +1428,47 @@
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptOutputTypeDef = TypedDict(
-    "FollowUpPromptOutputTypeDef",
+FollowUpPromptTypeDef = TypedDict(
+    "FollowUpPromptTypeDef",
     {
-        "prompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
+        "prompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
-        "status": StatusType,
-        "failureReason": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "idleSessionTTLInSeconds": int,
-        "voiceId": str,
-        "checksum": str,
-        "version": str,
-        "locale": LocaleType,
-        "childDirected": bool,
-        "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutBotResponseTypeDef = TypedDict(
-    "PutBotResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "intents": List[IntentTypeDef],
-        "enableModelImprovements": bool,
-        "nluIntentConfidenceThreshold": float,
-        "clarificationPrompt": PromptOutputTypeDef,
-        "abortStatement": StatementOutputTypeDef,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
-        "createVersion": bool,
         "detectSentiment": bool,
-        "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptTypeDef = TypedDict(
-    "FollowUpPromptTypeDef",
-    {
-        "prompt": PromptTypeDef,
-        "rejectionStatement": StatementTypeDef,
-    },
-)
-
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
         "locale": LocaleType,
         "childDirected": bool,
     },
@@ -1603,41 +1494,41 @@
 )
 
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
-_RequiredSlotOutputTypeDef = TypedDict(
-    "_RequiredSlotOutputTypeDef",
+PutBotResponseTypeDef = TypedDict(
+    "PutBotResponseTypeDef",
     {
         "name": str,
-        "slotConstraint": SlotConstraintType,
-    },
-)
-_OptionalSlotOutputTypeDef = TypedDict(
-    "_OptionalSlotOutputTypeDef",
-    {
         "description": str,
-        "slotType": str,
-        "slotTypeVersion": str,
-        "valueElicitationPrompt": PromptOutputTypeDef,
-        "priority": int,
-        "sampleUtterances": List[str],
-        "responseCard": str,
-        "obfuscationSetting": ObfuscationSettingType,
-        "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
+        "intents": List[IntentTypeDef],
+        "enableModelImprovements": bool,
+        "nluIntentConfidenceThreshold": float,
+        "clarificationPrompt": PromptTypeDef,
+        "abortStatement": StatementTypeDef,
+        "status": StatusType,
+        "failureReason": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "idleSessionTTLInSeconds": int,
+        "voiceId": str,
+        "checksum": str,
+        "version": str,
+        "locale": LocaleType,
+        "childDirected": bool,
+        "createVersion": bool,
+        "detectSentiment": bool,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
-    pass
-
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1645,15 +1536,15 @@
     "_OptionalSlotTypeDef",
     {
         "description": str,
         "slotType": str,
         "slotTypeVersion": str,
         "valueElicitationPrompt": PromptTypeDef,
         "priority": int,
-        "sampleUtterances": Sequence[str],
+        "sampleUtterances": List[str],
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
@@ -1661,15 +1552,15 @@
     pass
 
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
@@ -1678,15 +1569,15 @@
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
@@ -1700,15 +1591,15 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
+        "enumerationValues": Sequence[EnumerationValueTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1720,15 +1611,15 @@
     pass
 
 PutSlotTypeResponseTypeDef = TypedDict(
     "PutSlotTypeResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "enumerationValues": List[EnumerationValueTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
@@ -1751,26 +1642,25 @@
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotOutputTypeDef],
+        "slots": List[SlotTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
@@ -1782,72 +1672,45 @@
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "slots": List[SlotOutputTypeDef],
+        "slots": List[SlotTypeDef],
         "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookTypeDef,
-        "fulfillmentActivity": FulfillmentActivityTypeDef,
-        "parentIntentSignature": str,
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntentResponseTypeDef = TypedDict(
-    "PutIntentResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "slots": List[SlotOutputTypeDef],
-        "sampleUtterances": List[str],
-        "confirmationPrompt": PromptOutputTypeDef,
-        "rejectionStatement": StatementOutputTypeDef,
-        "followUpPrompt": FollowUpPromptOutputTypeDef,
-        "conclusionStatement": StatementOutputTypeDef,
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "createVersion": bool,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[SlotUnionTypeDef],
+        "slots": Sequence[SlotTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
@@ -1861,7 +1724,33 @@
     total=False,
 )
 
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
+
+PutIntentResponseTypeDef = TypedDict(
+    "PutIntentResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "slots": List[SlotTypeDef],
+        "sampleUtterances": List[str],
+        "confirmationPrompt": PromptTypeDef,
+        "rejectionStatement": StatementTypeDef,
+        "followUpPrompt": FollowUpPromptTypeDef,
+        "conclusionStatement": StatementTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
+        "parentIntentSignature": str,
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "createVersion": bool,
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post1/types_aiobotocore_lex_models.egg-info/SOURCES.txt` & `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

