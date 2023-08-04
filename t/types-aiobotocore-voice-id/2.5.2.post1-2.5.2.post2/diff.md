# Comparing `tmp/types-aiobotocore-voice-id-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-voice-id-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-voice-id-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-voice-id-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-voice-id-2.5.2.post1.tar` & `types-aiobotocore-voice-id-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.097431 types-aiobotocore-voice-id-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.097431 types-aiobotocore-voice-id-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-02 14:50:47.000000 types-aiobotocore-voice-id-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33666 2023-08-02 14:50:49.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33629 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13762 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12241 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2078 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1758 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1757 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      945 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25008 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24964 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10153 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10151 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7963 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7955 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32445 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32408 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13762 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/LICENSE` & `types-aiobotocore-voice-id-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/README.md` & `types-aiobotocore-voice-id-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,152 +272,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_voice_id.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `VoiceID` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/literals/).
+
 ```python
-from types_aiobotocore_voice_id.literals import (
-    AuthenticationDecisionType,
-    DomainStatusType,
-    DuplicateRegistrationActionType,
-    ExistingEnrollmentActionType,
-    FraudDetectionActionType,
-    FraudDetectionDecisionType,
-    FraudDetectionReasonType,
-    FraudsterRegistrationJobStatusType,
-    ListDomainsPaginatorName,
-    ListFraudsterRegistrationJobsPaginatorName,
-    ListFraudstersPaginatorName,
-    ListSpeakerEnrollmentJobsPaginatorName,
-    ListSpeakersPaginatorName,
-    ListWatchlistsPaginatorName,
-    ServerSideEncryptionUpdateStatusType,
-    SpeakerEnrollmentJobStatusType,
-    SpeakerStatusType,
-    StreamingStatusType,
-    VoiceIDServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_voice_id.literals import AuthenticationDecisionType
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_voice_id.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `VoiceID` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/type_defs/).
+
 ```python
-from types_aiobotocore_voice_id.type_defs import (
-    AssociateFraudsterRequestRequestTypeDef,
-    FraudsterTypeDef,
-    ResponseMetadataTypeDef,
-    AuthenticationConfigurationTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
-    TagTypeDef,
-    CreateWatchlistRequestRequestTypeDef,
-    WatchlistTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DeleteFraudsterRequestRequestTypeDef,
-    DeleteSpeakerRequestRequestTypeDef,
-    DeleteWatchlistRequestRequestTypeDef,
-    DescribeDomainRequestRequestTypeDef,
-    DescribeFraudsterRegistrationJobRequestRequestTypeDef,
-    DescribeFraudsterRequestRequestTypeDef,
-    DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
-    DescribeSpeakerRequestRequestTypeDef,
-    SpeakerTypeDef,
-    DescribeWatchlistRequestRequestTypeDef,
-    DisassociateFraudsterRequestRequestTypeDef,
-    ServerSideEncryptionUpdateDetailsTypeDef,
-    WatchlistDetailsTypeDef,
-    EnrollmentJobFraudDetectionConfigOutputTypeDef,
-    EnrollmentJobFraudDetectionConfigTypeDef,
-    EvaluateSessionRequestRequestTypeDef,
-    FailureDetailsTypeDef,
-    FraudDetectionConfigurationTypeDef,
-    KnownFraudsterRiskTypeDef,
-    VoiceSpoofingRiskTypeDef,
-    JobProgressTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
-    RegistrationConfigOutputTypeDef,
-    FraudsterSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestRequestTypeDef,
-    SpeakerSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestRequestTypeDef,
-    WatchlistSummaryTypeDef,
-    OptOutSpeakerRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateWatchlistRequestRequestTypeDef,
-    AssociateFraudsterResponseTypeDef,
-    DescribeFraudsterResponseTypeDef,
-    DisassociateFraudsterResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    AuthenticationResultTypeDef,
-    UpdateDomainRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateWatchlistResponseTypeDef,
-    DescribeWatchlistResponseTypeDef,
-    UpdateWatchlistResponseTypeDef,
-    DescribeSpeakerResponseTypeDef,
-    OptOutSpeakerResponseTypeDef,
-    DomainSummaryTypeDef,
-    DomainTypeDef,
-    EnrollmentConfigOutputTypeDef,
-    EnrollmentConfigTypeDef,
-    FraudRiskDetailsTypeDef,
-    FraudsterRegistrationJobSummaryTypeDef,
-    SpeakerEnrollmentJobSummaryTypeDef,
-    FraudsterRegistrationJobTypeDef,
-    ListFraudstersResponseTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    ListSpeakersResponseTypeDef,
-    ListWatchlistsResponseTypeDef,
-    RegistrationConfigUnionTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
-    ListDomainsResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    DescribeDomainResponseTypeDef,
-    UpdateDomainResponseTypeDef,
-    SpeakerEnrollmentJobTypeDef,
-    EnrollmentConfigUnionTypeDef,
-    StartSpeakerEnrollmentJobRequestRequestTypeDef,
-    FraudDetectionResultTypeDef,
-    ListFraudsterRegistrationJobsResponseTypeDef,
-    ListSpeakerEnrollmentJobsResponseTypeDef,
-    DescribeFraudsterRegistrationJobResponseTypeDef,
-    StartFraudsterRegistrationJobResponseTypeDef,
-    DescribeSpeakerEnrollmentJobResponseTypeDef,
-    StartSpeakerEnrollmentJobResponseTypeDef,
-    EvaluateSessionResponseTypeDef,
-)
+from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
 
 def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/setup.py` & `types-aiobotocore-voice-id-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-voice-id",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.pyi` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__main__.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VoiceID 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.VoiceID 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigUnionTypeDef,
+    EnrollmentConfigTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigUnionTypeDef,
+    RegistrationConfigTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -388,15 +388,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
+        RegistrationConfig: RegistrationConfigTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -405,15 +405,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
+        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.pyi` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigUnionTypeDef,
+    EnrollmentConfigTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigUnionTypeDef,
+    RegistrationConfigTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -357,15 +357,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
+        RegistrationConfig: RegistrationConfigTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -373,15 +373,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
+        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -277,26 +279,28 @@
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

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.pyi` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
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
@@ -189,14 +190,15 @@
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
@@ -275,26 +277,28 @@
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

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.pyi` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.py` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
     data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -55,38 +55,36 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
-    "RegistrationConfigOutputTypeDef",
+    "RegistrationConfigTypeDef",
     "FraudsterSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
     "ListFraudstersRequestRequestTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
@@ -97,37 +95,34 @@
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
-    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
-    "RegistrationConfigUnionTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
-    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -339,30 +334,20 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
-    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
-    {
-        "FraudDetectionAction": FraudDetectionActionType,
-        "RiskThreshold": int,
-        "WatchlistIds": List[str],
-    },
-    total=False,
-)
-
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": Sequence[str],
+        "WatchlistIds": List[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -447,16 +432,16 @@
 )
 
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 
-RegistrationConfigOutputTypeDef = TypedDict(
-    "RegistrationConfigOutputTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -645,24 +630,14 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
-    {
-        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
-        "FraudsterSimilarityThreshold": int,
-        "WatchlistIds": Sequence[str],
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -869,23 +844,14 @@
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
-EnrollmentConfigOutputTypeDef = TypedDict(
-    "EnrollmentConfigOutputTypeDef",
-    {
-        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
-        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -939,19 +905,46 @@
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigOutputTypeDef,
+        "RegistrationConfig": RegistrationConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+    },
+)
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
+
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
     {
         "FraudsterSummaries": List[FraudsterSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1096,42 +1089,14 @@
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
-    {
-        "DataAccessRoleArn": str,
-        "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-    },
-)
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
-):
-    pass
-
-
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1164,27 +1129,26 @@
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
+        "EnrollmentConfig": EnrollmentConfigTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
-EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.pyi` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
     data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -54,38 +54,36 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
-    "RegistrationConfigOutputTypeDef",
+    "RegistrationConfigTypeDef",
     "FraudsterSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
     "ListFraudstersRequestRequestTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
@@ -96,37 +94,34 @@
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
-    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
-    "RegistrationConfigUnionTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
-    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -336,30 +331,20 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
-    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
-    {
-        "FraudDetectionAction": FraudDetectionActionType,
-        "RiskThreshold": int,
-        "WatchlistIds": List[str],
-    },
-    total=False,
-)
-
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": Sequence[str],
+        "WatchlistIds": List[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -440,16 +425,16 @@
     },
     total=False,
 )
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-RegistrationConfigOutputTypeDef = TypedDict(
-    "RegistrationConfigOutputTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -628,24 +613,14 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
-    {
-        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
-        "FraudsterSimilarityThreshold": int,
-        "WatchlistIds": Sequence[str],
-    },
-    total=False,
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -846,23 +821,14 @@
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
-EnrollmentConfigOutputTypeDef = TypedDict(
-    "EnrollmentConfigOutputTypeDef",
-    {
-        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
-        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -916,19 +882,44 @@
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigOutputTypeDef,
+        "RegistrationConfig": RegistrationConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+    },
+)
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
     {
         "FraudsterSummaries": List[FraudsterSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1063,40 +1054,14 @@
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
-    {
-        "DataAccessRoleArn": str,
-        "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-    },
-)
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
-    },
-    total=False,
-)
-
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
-):
-    pass
-
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1129,27 +1094,26 @@
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
+        "EnrollmentConfig": EnrollmentConfigTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
-EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/SOURCES.txt` & `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

