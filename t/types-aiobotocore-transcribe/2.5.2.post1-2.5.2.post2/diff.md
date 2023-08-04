# Comparing `tmp/types-aiobotocore-transcribe-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-transcribe-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transcribe-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-transcribe-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-transcribe-2.5.2.post1.tar` & `types-aiobotocore-transcribe-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31820 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31772 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42322 2023-08-02 14:50:42.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-08-02 14:50:42.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12414 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10877 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      501 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      500 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31836 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31788 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10615 2023-08-04 13:55:11.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10613 2023-08-04 13:55:11.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39556 2023-08-04 13:55:15.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39525 2023-08-04 13:55:15.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12414 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      785 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/LICENSE` & `types-aiobotocore-transcribe-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/setup.py` & `types-aiobotocore-transcribe-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transcribe",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__main__.py` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.TranscribeService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
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

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.py` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsUnionTypeDef,
+    CallAnalyticsJobSettingsTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionUnionTypeDef,
+    ContentRedactionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -61,21 +61,22 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleUnionTypeDef,
+    RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -134,19 +135,15 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#close)
         """
 
     async def create_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[RuleUnionTypeDef],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_call_analytics_category)
         """
@@ -507,15 +504,15 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
+        Settings: CallAnalyticsJobSettingsTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -559,21 +556,22 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionUnionTypeDef = ...,
+        ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
+        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#start_transcription_job)
@@ -593,19 +591,15 @@
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#untag_resource)
         """
 
     async def update_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[RuleUnionTypeDef],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_call_analytics_category)
         """
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.pyi` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsUnionTypeDef,
+    CallAnalyticsJobSettingsTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionUnionTypeDef,
+    ContentRedactionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -61,21 +61,22 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleUnionTypeDef,
+    RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -127,19 +128,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#close)
         """
     async def create_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[RuleUnionTypeDef],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_call_analytics_category)
         """
@@ -469,15 +466,15 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
+        Settings: CallAnalyticsJobSettingsTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -519,21 +516,22 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionUnionTypeDef = ...,
+        ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
+        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#start_transcription_job)
@@ -550,19 +548,15 @@
         """
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#untag_resource)
         """
     async def update_call_analytics_category(
-        self,
-        *,
-        CategoryName: str,
-        Rules: Sequence[RuleUnionTypeDef],
-        InputType: InputTypeType = ...
+        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_call_analytics_category)
         """
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.py` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "ParticipantRoleType",
     "PiiEntityTypeType",
     "RedactionOutputType",
     "RedactionTypeType",
     "SentimentValueType",
     "SpecialtyType",
     "SubtitleFormatType",
+    "ToxicityCategoryType",
     "TranscriptFilterTypeType",
     "TranscriptionJobStatusType",
     "TypeType",
     "VocabularyFilterMethodType",
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
@@ -113,14 +114,15 @@
     "SSN",
 ]
 RedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
 RedactionTypeType = Literal["PII"]
 SentimentValueType = Literal["MIXED", "NEGATIVE", "NEUTRAL", "POSITIVE"]
 SpecialtyType = Literal["PRIMARYCARE"]
 SubtitleFormatType = Literal["srt", "vtt"]
+ToxicityCategoryType = Literal["ALL"]
 TranscriptFilterTypeType = Literal["EXACT"]
 TranscriptionJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
 TypeType = Literal["CONVERSATION", "DICTATION"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VocabularyStateType = Literal["FAILED", "PENDING", "READY"]
 TranscribeServiceServiceName = Literal["transcribe"]
 ServiceName = Literal[
@@ -134,14 +136,15 @@
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
@@ -237,14 +240,15 @@
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
@@ -323,26 +327,28 @@
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

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.pyi` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "ParticipantRoleType",
     "PiiEntityTypeType",
     "RedactionOutputType",
     "RedactionTypeType",
     "SentimentValueType",
     "SpecialtyType",
     "SubtitleFormatType",
+    "ToxicityCategoryType",
     "TranscriptFilterTypeType",
     "TranscriptionJobStatusType",
     "TypeType",
     "VocabularyFilterMethodType",
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
@@ -111,14 +112,15 @@
     "SSN",
 ]
 RedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
 RedactionTypeType = Literal["PII"]
 SentimentValueType = Literal["MIXED", "NEGATIVE", "NEUTRAL", "POSITIVE"]
 SpecialtyType = Literal["PRIMARYCARE"]
 SubtitleFormatType = Literal["srt", "vtt"]
+ToxicityCategoryType = Literal["ALL"]
 TranscriptFilterTypeType = Literal["EXACT"]
 TranscriptionJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
 TypeType = Literal["CONVERSATION", "DICTATION"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VocabularyStateType = Literal["FAILED", "PENDING", "READY"]
 TranscribeServiceServiceName = Literal["transcribe"]
 ServiceName = Literal[
@@ -132,14 +134,15 @@
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
@@ -235,14 +238,15 @@
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
@@ -321,26 +325,28 @@
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

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.py` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_transcribe.type_defs import AbsoluteTimeRangeTypeDef
 
     data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -43,17 +43,16 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
@@ -89,22 +88,21 @@
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
-    "ContentRedactionUnionTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
     "CreateVocabularyFilterResponseTypeDef",
     "CreateVocabularyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
@@ -118,114 +116,87 @@
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
-    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "RuleUnionTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+_RequiredContentRedactionTypeDef = TypedDict(
+    "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
+_OptionalContentRedactionTypeDef = TypedDict(
+    "_OptionalContentRedactionTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
     total=False,
 )
 
 
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
+class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
 
 LanguageIdSettingsTypeDef = TypedDict(
     "LanguageIdSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
     total=False,
 )
 
-_RequiredContentRedactionTypeDef = TypedDict(
-    "_RequiredContentRedactionTypeDef",
-    {
-        "RedactionType": Literal["PII"],
-        "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionTypeDef = TypedDict(
-    "_OptionalContentRedactionTypeDef",
-    {
-        "PiiEntityTypes": Sequence[PiiEntityTypeType],
-    },
-    total=False,
-)
-
-
-class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
-    pass
-
-
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
@@ -623,14 +594,21 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
+)
+
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
@@ -698,43 +676,28 @@
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
-    "CallAnalyticsJobSettingsOutputTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
-    },
-    total=False,
-)
-
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": Sequence[LanguageCodeType],
-        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
-ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
 CreateMedicalVocabularyResponseTypeDef = TypedDict(
     "CreateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
@@ -1015,38 +978,14 @@
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "Negate": bool,
     },
     total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
-    {
-        "Sentiments": List[SentimentValueType],
-    },
-)
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
-    {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
-        "Negate": bool,
-    },
-    total=False,
-)
-
-
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredSentimentFilterTypeDef = TypedDict(
     "_RequiredSentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
     },
 )
 _OptionalSentimentFilterTypeDef = TypedDict(
@@ -1061,39 +1000,14 @@
 )
 
 
 class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
 
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
-    {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
-    },
-)
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
-    {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
-        "Negate": bool,
-    },
-    total=False,
-)
-
-
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
     },
 )
@@ -1205,35 +1119,14 @@
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1253,26 +1146,49 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionTypeDef,
+        "ModelSettings": ModelSettingsTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsTypeDef],
+    },
+    total=False,
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
@@ -1282,23 +1198,24 @@
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "Settings": SettingsTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
@@ -1311,23 +1228,20 @@
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
+        "Settings": CallAnalyticsJobSettingsTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-CallAnalyticsJobSettingsUnionTypeDef = Union[
-    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
-]
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1364,25 +1278,14 @@
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
-        "TranscriptFilter": TranscriptFilterOutputTypeDef,
-        "SentimentFilter": SentimentFilterOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
         "TranscriptFilter": TranscriptFilterTypeDef,
         "SentimentFilter": SentimentFilterTypeDef,
@@ -1448,61 +1351,27 @@
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
     total=False,
 )
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "GetCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
-    "ListCallAnalyticsCategoriesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1517,15 +1386,15 @@
     pass
 
 
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1534,7 +1403,41 @@
 
 
 class UpdateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
+
+
+CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "GetCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
+    "ListCallAnalyticsCategoriesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Categories": List[CategoryPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.pyi` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_transcribe.type_defs import AbsoluteTimeRangeTypeDef
 
     data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -42,17 +42,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
@@ -88,22 +87,21 @@
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
-    "ContentRedactionUnionTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
     "CreateVocabularyFilterResponseTypeDef",
     "CreateVocabularyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
@@ -117,110 +115,85 @@
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
-    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "RuleUnionTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+_RequiredContentRedactionTypeDef = TypedDict(
+    "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
+_OptionalContentRedactionTypeDef = TypedDict(
+    "_OptionalContentRedactionTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
     total=False,
 )
 
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
+class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
 LanguageIdSettingsTypeDef = TypedDict(
     "LanguageIdSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
     total=False,
 )
 
-_RequiredContentRedactionTypeDef = TypedDict(
-    "_RequiredContentRedactionTypeDef",
-    {
-        "RedactionType": Literal["PII"],
-        "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionTypeDef = TypedDict(
-    "_OptionalContentRedactionTypeDef",
-    {
-        "PiiEntityTypes": Sequence[PiiEntityTypeType],
-    },
-    total=False,
-)
-
-class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
-    pass
-
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
@@ -616,14 +589,21 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
+)
+
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
@@ -687,43 +667,28 @@
 )
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
-CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
-    "CallAnalyticsJobSettingsOutputTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
-    },
-    total=False,
-)
-
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": Sequence[LanguageCodeType],
-        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
-ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
 CreateMedicalVocabularyResponseTypeDef = TypedDict(
     "CreateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
@@ -996,36 +961,14 @@
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "Negate": bool,
     },
     total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
-    {
-        "Sentiments": List[SentimentValueType],
-    },
-)
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
-    {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
-        "Negate": bool,
-    },
-    total=False,
-)
-
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
 _RequiredSentimentFilterTypeDef = TypedDict(
     "_RequiredSentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
     },
 )
 _OptionalSentimentFilterTypeDef = TypedDict(
@@ -1038,37 +981,14 @@
     },
     total=False,
 )
 
 class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
-    {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
-    },
-)
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
-    {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
-        "Negate": bool,
-    },
-    total=False,
-)
-
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
-    pass
-
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
     },
 )
@@ -1176,35 +1096,14 @@
 
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1224,24 +1123,47 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionTypeDef,
+        "ModelSettings": ModelSettingsTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsTypeDef],
+    },
+    total=False,
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
@@ -1251,23 +1173,24 @@
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "Settings": SettingsTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
         "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
@@ -1280,23 +1203,20 @@
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
+        "Settings": CallAnalyticsJobSettingsTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-CallAnalyticsJobSettingsUnionTypeDef = Union[
-    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
-]
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1331,25 +1251,14 @@
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
-        "TranscriptFilter": TranscriptFilterOutputTypeDef,
-        "SentimentFilter": SentimentFilterOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
         "TranscriptFilter": TranscriptFilterTypeDef,
         "SentimentFilter": SentimentFilterTypeDef,
@@ -1415,61 +1324,27 @@
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
     total=False,
 )
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "GetCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
-    "ListCallAnalyticsCategoriesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1482,15 +1357,15 @@
 ):
     pass
 
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleUnionTypeDef],
+        "Rules": Sequence[RuleTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
@@ -1498,7 +1373,40 @@
 )
 
 class UpdateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
+
+CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "GetCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
+    "ListCallAnalyticsCategoriesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Categories": List[CategoryPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/SOURCES.txt` & `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

