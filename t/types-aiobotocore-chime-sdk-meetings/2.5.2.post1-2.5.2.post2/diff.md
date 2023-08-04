# Comparing `tmp/types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-chime-sdk-meetings-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:31 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.697642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.697642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.115331 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:00:31.115331 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:31.115331 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/LICENSE` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/PKG-INFO` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-chime-sdk-meetings
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,91 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chime_sdk_meetings.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ChimeSDKMeetings` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/literals/).
+
 ```python
-from types_aiobotocore_chime_sdk_meetings.literals import (
-    MediaCapabilitiesType,
-    MeetingFeatureStatusType,
-    TranscribeContentIdentificationTypeType,
-    TranscribeContentRedactionTypeType,
-    TranscribeLanguageCodeType,
-    TranscribeMedicalContentIdentificationTypeType,
-    TranscribeMedicalLanguageCodeType,
-    TranscribeMedicalRegionType,
-    TranscribeMedicalSpecialtyType,
-    TranscribeMedicalTypeType,
-    TranscribePartialResultsStabilityType,
-    TranscribeRegionType,
-    TranscribeVocabularyFilterMethodType,
-    ChimeSDKMeetingsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_chime_sdk_meetings.literals import MediaCapabilitiesType
 
 
 def check_value(value: MediaCapabilitiesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chime_sdk_meetings.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ChimeSDKMeetings` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/type_defs/).
+
 ```python
-from types_aiobotocore_chime_sdk_meetings.type_defs import (
-    AttendeeCapabilitiesTypeDef,
-    AttendeeIdItemTypeDef,
-    AudioFeaturesTypeDef,
-    CreateAttendeeErrorTypeDef,
-    ResponseMetadataTypeDef,
-    NotificationsConfigurationTypeDef,
-    TagTypeDef,
-    DeleteAttendeeRequestRequestTypeDef,
-    DeleteMeetingRequestRequestTypeDef,
-    EngineTranscribeMedicalSettingsTypeDef,
-    EngineTranscribeSettingsTypeDef,
-    GetAttendeeRequestRequestTypeDef,
-    GetMeetingRequestRequestTypeDef,
-    ListAttendeesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    MediaPlacementTypeDef,
-    StopMeetingTranscriptionRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AttendeeTypeDef,
-    CreateAttendeeRequestItemTypeDef,
-    CreateAttendeeRequestRequestTypeDef,
-    UpdateAttendeeCapabilitiesRequestRequestTypeDef,
-    BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
-    MeetingFeaturesConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TranscriptionConfigurationTypeDef,
-    BatchCreateAttendeeResponseTypeDef,
-    CreateAttendeeResponseTypeDef,
-    GetAttendeeResponseTypeDef,
-    ListAttendeesResponseTypeDef,
-    UpdateAttendeeCapabilitiesResponseTypeDef,
-    BatchCreateAttendeeRequestRequestTypeDef,
-    CreateMeetingRequestRequestTypeDef,
-    CreateMeetingWithAttendeesRequestRequestTypeDef,
-    MeetingTypeDef,
-    StartMeetingTranscriptionRequestRequestTypeDef,
-    CreateMeetingResponseTypeDef,
-    CreateMeetingWithAttendeesResponseTypeDef,
-    GetMeetingResponseTypeDef,
-)
+from types_aiobotocore_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
 
 def get_value() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/README.md` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-chime-sdk-meetings
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,91 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chime_sdk_meetings.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ChimeSDKMeetings` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/literals/).
+
 ```python
-from types_aiobotocore_chime_sdk_meetings.literals import (
-    MediaCapabilitiesType,
-    MeetingFeatureStatusType,
-    TranscribeContentIdentificationTypeType,
-    TranscribeContentRedactionTypeType,
-    TranscribeLanguageCodeType,
-    TranscribeMedicalContentIdentificationTypeType,
-    TranscribeMedicalLanguageCodeType,
-    TranscribeMedicalRegionType,
-    TranscribeMedicalSpecialtyType,
-    TranscribeMedicalTypeType,
-    TranscribePartialResultsStabilityType,
-    TranscribeRegionType,
-    TranscribeVocabularyFilterMethodType,
-    ChimeSDKMeetingsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_chime_sdk_meetings.literals import MediaCapabilitiesType
 
 
 def check_value(value: MediaCapabilitiesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chime_sdk_meetings.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ChimeSDKMeetings` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/type_defs/).
+
 ```python
-from types_aiobotocore_chime_sdk_meetings.type_defs import (
-    AttendeeCapabilitiesTypeDef,
-    AttendeeIdItemTypeDef,
-    AudioFeaturesTypeDef,
-    CreateAttendeeErrorTypeDef,
-    ResponseMetadataTypeDef,
-    NotificationsConfigurationTypeDef,
-    TagTypeDef,
-    DeleteAttendeeRequestRequestTypeDef,
-    DeleteMeetingRequestRequestTypeDef,
-    EngineTranscribeMedicalSettingsTypeDef,
-    EngineTranscribeSettingsTypeDef,
-    GetAttendeeRequestRequestTypeDef,
-    GetMeetingRequestRequestTypeDef,
-    ListAttendeesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    MediaPlacementTypeDef,
-    StopMeetingTranscriptionRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AttendeeTypeDef,
-    CreateAttendeeRequestItemTypeDef,
-    CreateAttendeeRequestRequestTypeDef,
-    UpdateAttendeeCapabilitiesRequestRequestTypeDef,
-    BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
-    MeetingFeaturesConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TranscriptionConfigurationTypeDef,
-    BatchCreateAttendeeResponseTypeDef,
-    CreateAttendeeResponseTypeDef,
-    GetAttendeeResponseTypeDef,
-    ListAttendeesResponseTypeDef,
-    UpdateAttendeeCapabilitiesResponseTypeDef,
-    BatchCreateAttendeeRequestRequestTypeDef,
-    CreateMeetingRequestRequestTypeDef,
-    CreateMeetingWithAttendeesRequestRequestTypeDef,
-    MeetingTypeDef,
-    StartMeetingTranscriptionRequestRequestTypeDef,
-    CreateMeetingResponseTypeDef,
-    CreateMeetingWithAttendeesResponseTypeDef,
-    GetMeetingResponseTypeDef,
-)
+from types_aiobotocore_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
 
 def get_value() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-meetings",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__main__.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post2/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

