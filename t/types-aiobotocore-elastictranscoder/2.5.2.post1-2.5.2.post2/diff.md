# Comparing `tmp/types-aiobotocore-elastictranscoder-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elastictranscoder-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1.tar` & `types-aiobotocore-elastictranscoder-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:38:16.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18610 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.524070 types-aiobotocore-elastictranscoder-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-08-04 12:00:50.520070 types-aiobotocore-elastictranscoder-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.524070 types-aiobotocore-elastictranscoder-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.520070 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22853 2023-08-04 11:45:46.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-08-04 11:45:46.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-04 11:45:45.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.520070 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:50.000000 types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/LICENSE` & `types-aiobotocore-elastictranscoder-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,124 +324,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elastictranscoder.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ElasticTranscoder` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/literals/).
+
 ```python
-from types_aiobotocore_elastictranscoder.literals import (
-    JobCompleteWaiterName,
-    ListJobsByPipelinePaginatorName,
-    ListJobsByStatusPaginatorName,
-    ListPipelinesPaginatorName,
-    ListPresetsPaginatorName,
-    ElasticTranscoderServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_elastictranscoder.literals import JobCompleteWaiterName
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elastictranscoder.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticTranscoder` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/type_defs/).
+
 ```python
-from types_aiobotocore_elastictranscoder.type_defs import (
-    EncryptionTypeDef,
-    AudioCodecOptionsTypeDef,
-    CancelJobRequestRequestTypeDef,
-    TimeSpanTypeDef,
-    HlsContentProtectionTypeDef,
-    PlayReadyDrmTypeDef,
-    ResponseMetadataTypeDef,
-    NotificationsTypeDef,
-    WarningTypeDef,
-    ThumbnailsTypeDef,
-    DeletePipelineRequestRequestTypeDef,
-    DeletePresetRequestRequestTypeDef,
-    DetectedPropertiesTypeDef,
-    TimingTypeDef,
-    PaginatorConfigTypeDef,
-    ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestRequestTypeDef,
-    PermissionOutputTypeDef,
-    PermissionTypeDef,
-    PresetWatermarkTypeDef,
-    WaiterConfigTypeDef,
-    ReadJobRequestRequestTypeDef,
-    ReadPipelineRequestRequestTypeDef,
-    ReadPresetRequestRequestTypeDef,
-    TestRoleRequestRequestTypeDef,
-    UpdatePipelineStatusRequestRequestTypeDef,
-    ArtworkTypeDef,
-    CaptionFormatTypeDef,
-    CaptionSourceTypeDef,
-    JobWatermarkTypeDef,
-    AudioParametersTypeDef,
-    ClipTypeDef,
-    CreateJobPlaylistTypeDef,
-    PlaylistTypeDef,
-    TestRoleResponseTypeDef,
-    UpdatePipelineNotificationsRequestRequestTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
-    PipelineOutputConfigOutputTypeDef,
-    PipelineOutputConfigTypeDef,
-    VideoParametersOutputTypeDef,
-    VideoParametersTypeDef,
-    ReadJobRequestJobCompleteWaitTypeDef,
-    JobAlbumArtOutputTypeDef,
-    JobAlbumArtTypeDef,
-    CaptionsOutputTypeDef,
-    CaptionsTypeDef,
-    InputCaptionsOutputTypeDef,
-    InputCaptionsTypeDef,
-    PipelineTypeDef,
-    CreatePipelineRequestRequestTypeDef,
-    PipelineOutputConfigUnionTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
-    PresetTypeDef,
-    CreatePresetRequestRequestTypeDef,
-    VideoParametersUnionTypeDef,
-    JobOutputTypeDef,
-    CreateJobOutputTypeDef,
-    JobInputOutputTypeDef,
-    JobInputTypeDef,
-    CreatePipelineResponseTypeDef,
-    ListPipelinesResponseTypeDef,
-    ReadPipelineResponseTypeDef,
-    UpdatePipelineNotificationsResponseTypeDef,
-    UpdatePipelineResponseTypeDef,
-    UpdatePipelineStatusResponseTypeDef,
-    CreatePresetResponseTypeDef,
-    ListPresetsResponseTypeDef,
-    ReadPresetResponseTypeDef,
-    JobTypeDef,
-    JobInputUnionTypeDef,
-    CreateJobResponseTypeDef,
-    ListJobsByPipelineResponseTypeDef,
-    ListJobsByStatusResponseTypeDef,
-    ReadJobResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
-)
+from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
 
 def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/README.md` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-elastictranscoder
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore elastictranscoder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,124 +324,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elastictranscoder.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ElasticTranscoder` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/literals/).
+
 ```python
-from types_aiobotocore_elastictranscoder.literals import (
-    JobCompleteWaiterName,
-    ListJobsByPipelinePaginatorName,
-    ListJobsByStatusPaginatorName,
-    ListPipelinesPaginatorName,
-    ListPresetsPaginatorName,
-    ElasticTranscoderServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_elastictranscoder.literals import JobCompleteWaiterName
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elastictranscoder.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticTranscoder` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/type_defs/).
+
 ```python
-from types_aiobotocore_elastictranscoder.type_defs import (
-    EncryptionTypeDef,
-    AudioCodecOptionsTypeDef,
-    CancelJobRequestRequestTypeDef,
-    TimeSpanTypeDef,
-    HlsContentProtectionTypeDef,
-    PlayReadyDrmTypeDef,
-    ResponseMetadataTypeDef,
-    NotificationsTypeDef,
-    WarningTypeDef,
-    ThumbnailsTypeDef,
-    DeletePipelineRequestRequestTypeDef,
-    DeletePresetRequestRequestTypeDef,
-    DetectedPropertiesTypeDef,
-    TimingTypeDef,
-    PaginatorConfigTypeDef,
-    ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestRequestTypeDef,
-    PermissionOutputTypeDef,
-    PermissionTypeDef,
-    PresetWatermarkTypeDef,
-    WaiterConfigTypeDef,
-    ReadJobRequestRequestTypeDef,
-    ReadPipelineRequestRequestTypeDef,
-    ReadPresetRequestRequestTypeDef,
-    TestRoleRequestRequestTypeDef,
-    UpdatePipelineStatusRequestRequestTypeDef,
-    ArtworkTypeDef,
-    CaptionFormatTypeDef,
-    CaptionSourceTypeDef,
-    JobWatermarkTypeDef,
-    AudioParametersTypeDef,
-    ClipTypeDef,
-    CreateJobPlaylistTypeDef,
-    PlaylistTypeDef,
-    TestRoleResponseTypeDef,
-    UpdatePipelineNotificationsRequestRequestTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
-    PipelineOutputConfigOutputTypeDef,
-    PipelineOutputConfigTypeDef,
-    VideoParametersOutputTypeDef,
-    VideoParametersTypeDef,
-    ReadJobRequestJobCompleteWaitTypeDef,
-    JobAlbumArtOutputTypeDef,
-    JobAlbumArtTypeDef,
-    CaptionsOutputTypeDef,
-    CaptionsTypeDef,
-    InputCaptionsOutputTypeDef,
-    InputCaptionsTypeDef,
-    PipelineTypeDef,
-    CreatePipelineRequestRequestTypeDef,
-    PipelineOutputConfigUnionTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
-    PresetTypeDef,
-    CreatePresetRequestRequestTypeDef,
-    VideoParametersUnionTypeDef,
-    JobOutputTypeDef,
-    CreateJobOutputTypeDef,
-    JobInputOutputTypeDef,
-    JobInputTypeDef,
-    CreatePipelineResponseTypeDef,
-    ListPipelinesResponseTypeDef,
-    ReadPipelineResponseTypeDef,
-    UpdatePipelineNotificationsResponseTypeDef,
-    UpdatePipelineResponseTypeDef,
-    UpdatePipelineStatusResponseTypeDef,
-    CreatePresetResponseTypeDef,
-    ListPresetsResponseTypeDef,
-    ReadPresetResponseTypeDef,
-    JobTypeDef,
-    JobInputUnionTypeDef,
-    CreateJobResponseTypeDef,
-    ListJobsByPipelineResponseTypeDef,
-    ListJobsByStatusResponseTypeDef,
-    ReadJobResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
-)
+from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
 
 def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/setup.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastictranscoder",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__main__.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticTranscoder 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputUnionTypeDef,
+    JobInputTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigUnionTypeDef,
+    PipelineOutputConfigTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersUnionTypeDef,
+    VideoParametersTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -121,16 +121,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#close)
         """
 
     async def create_job(
         self,
         *,
         PipelineId: str,
-        Input: JobInputUnionTypeDef = ...,
-        Inputs: Sequence[JobInputUnionTypeDef] = ...,
+        Input: JobInputTypeDef = ...,
+        Inputs: Sequence[JobInputTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
@@ -146,31 +146,31 @@
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
+        ContentConfig: PipelineOutputConfigTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
 
     async def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: VideoParametersUnionTypeDef = ...,
+        Video: VideoParametersTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
@@ -289,16 +289,16 @@
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
+        ContentConfig: PipelineOutputConfigTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputUnionTypeDef,
+    JobInputTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigUnionTypeDef,
+    PipelineOutputConfigTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersUnionTypeDef,
+    VideoParametersTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -113,16 +113,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#close)
         """
     async def create_job(
         self,
         *,
         PipelineId: str,
-        Input: JobInputUnionTypeDef = ...,
-        Inputs: Sequence[JobInputUnionTypeDef] = ...,
+        Input: JobInputTypeDef = ...,
+        Inputs: Sequence[JobInputTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
@@ -137,30 +137,30 @@
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
+        ContentConfig: PipelineOutputConfigTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
     async def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: VideoParametersUnionTypeDef = ...,
+        Video: VideoParametersTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
@@ -267,16 +267,16 @@
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
+        ContentConfig: PipelineOutputConfigTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
     data: EncryptionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -36,15 +36,14 @@
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
     "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "PermissionOutputTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
     "TestRoleRequestRequestTypeDef",
@@ -59,52 +58,43 @@
     "PlaylistTypeDef",
     "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
-    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
-    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
-    "JobAlbumArtOutputTypeDef",
     "JobAlbumArtTypeDef",
-    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
-    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
-    "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
-    "PipelineOutputConfigUnionTypeDef",
+    "PipelineTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "VideoParametersUnionTypeDef",
-    "JobOutputTypeDef",
+    "PresetTypeDef",
     "CreateJobOutputTypeDef",
-    "JobInputOutputTypeDef",
+    "JobOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -318,24 +308,14 @@
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-PermissionOutputTypeDef = TypedDict(
-    "PermissionOutputTypeDef",
-    {
-        "GranteeType": str,
-        "Grantee": str,
-        "Access": List[str],
-    },
-    total=False,
-)
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
@@ -577,56 +557,24 @@
     {
         "Ascending": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PipelineOutputConfigOutputTypeDef = TypedDict(
-    "PipelineOutputConfigOutputTypeDef",
-    {
-        "Bucket": str,
-        "StorageClass": str,
-        "Permissions": List[PermissionOutputTypeDef],
-    },
-    total=False,
-)
-
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
-VideoParametersOutputTypeDef = TypedDict(
-    "VideoParametersOutputTypeDef",
-    {
-        "Codec": str,
-        "CodecOptions": Dict[str, str],
-        "KeyframesMaxDist": str,
-        "FixedGOP": str,
-        "BitRate": str,
-        "FrameRate": str,
-        "MaxFrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "DisplayAspectRatio": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-        "Watermarks": List[PresetWatermarkTypeDef],
-    },
-    total=False,
-)
-
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -662,88 +610,42 @@
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
 
-JobAlbumArtOutputTypeDef = TypedDict(
-    "JobAlbumArtOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "Artwork": List[ArtworkTypeDef],
-    },
-    total=False,
-)
-
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
-CaptionsOutputTypeDef = TypedDict(
-    "CaptionsOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceTypeDef],
-        "CaptionFormats": List[CaptionFormatTypeDef],
-    },
-    total=False,
-)
-
 CaptionsTypeDef = TypedDict(
     "CaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
         "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-InputCaptionsOutputTypeDef = TypedDict(
-    "InputCaptionsOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceTypeDef],
-    },
-    total=False,
-)
-
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigOutputTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -763,17 +665,32 @@
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-PipelineOutputConfigUnionTypeDef = Union[
-    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
-]
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsTypeDef,
+        "ContentConfig": PipelineOutputConfigTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -793,30 +710,14 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersOutputTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
-    },
-    total=False,
-)
-
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -834,39 +735,26 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
     {
         "Id": str,
-        "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtOutputTypeDef,
-        "Composition": List[ClipTypeDef],
-        "Captions": CaptionsOutputTypeDef,
-        "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersTypeDef,
+        "Video": VideoParametersTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
+        "Type": str,
     },
     total=False,
 )
 
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
@@ -881,27 +769,38 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-JobInputOutputTypeDef = TypedDict(
-    "JobInputOutputTypeDef",
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
+        "Id": str,
         "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
         "FrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "Interlaced": str,
-        "Container": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkTypeDef],
+        "AlbumArt": JobAlbumArtTypeDef,
+        "Composition": List[ClipTypeDef],
+        "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
-        "TimeSpan": TimeSpanTypeDef,
-        "InputCaptions": InputCaptionsOutputTypeDef,
-        "DetectedProperties": DetectedPropertiesTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -993,34 +892,60 @@
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
+
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PipelineId": str,
-        "Input": JobInputOutputTypeDef,
-        "Inputs": List[JobInputOutputTypeDef],
+        "Input": JobInputTypeDef,
+        "Inputs": List[JobInputTypeDef],
         "Output": JobOutputTypeDef,
         "Outputs": List[JobOutputTypeDef],
         "OutputKeyPrefix": str,
         "Playlists": List[PlaylistTypeDef],
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
-JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1046,33 +971,7 @@
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[JobInputUnionTypeDef],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
     data: EncryptionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
@@ -35,15 +35,14 @@
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
     "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "PermissionOutputTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
     "TestRoleRequestRequestTypeDef",
@@ -58,52 +57,43 @@
     "PlaylistTypeDef",
     "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
     "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
-    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
-    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
-    "JobAlbumArtOutputTypeDef",
     "JobAlbumArtTypeDef",
-    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
-    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
-    "PipelineTypeDef",
     "CreatePipelineRequestRequestTypeDef",
-    "PipelineOutputConfigUnionTypeDef",
+    "PipelineTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PresetTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "VideoParametersUnionTypeDef",
-    "JobOutputTypeDef",
+    "PresetTypeDef",
     "CreateJobOutputTypeDef",
-    "JobInputOutputTypeDef",
+    "JobOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -313,24 +303,14 @@
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-PermissionOutputTypeDef = TypedDict(
-    "PermissionOutputTypeDef",
-    {
-        "GranteeType": str,
-        "Grantee": str,
-        "Access": List[str],
-    },
-    total=False,
-)
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeType": str,
         "Grantee": str,
         "Access": Sequence[str],
     },
@@ -568,56 +548,24 @@
     {
         "Ascending": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PipelineOutputConfigOutputTypeDef = TypedDict(
-    "PipelineOutputConfigOutputTypeDef",
-    {
-        "Bucket": str,
-        "StorageClass": str,
-        "Permissions": List[PermissionOutputTypeDef],
-    },
-    total=False,
-)
-
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
-VideoParametersOutputTypeDef = TypedDict(
-    "VideoParametersOutputTypeDef",
-    {
-        "Codec": str,
-        "CodecOptions": Dict[str, str],
-        "KeyframesMaxDist": str,
-        "FixedGOP": str,
-        "BitRate": str,
-        "FrameRate": str,
-        "MaxFrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "MaxWidth": str,
-        "MaxHeight": str,
-        "DisplayAspectRatio": str,
-        "SizingPolicy": str,
-        "PaddingPolicy": str,
-        "Watermarks": List[PresetWatermarkTypeDef],
-    },
-    total=False,
-)
-
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -651,88 +599,42 @@
 )
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
-JobAlbumArtOutputTypeDef = TypedDict(
-    "JobAlbumArtOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "Artwork": List[ArtworkTypeDef],
-    },
-    total=False,
-)
-
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
-CaptionsOutputTypeDef = TypedDict(
-    "CaptionsOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceTypeDef],
-        "CaptionFormats": List[CaptionFormatTypeDef],
-    },
-    total=False,
-)
-
 CaptionsTypeDef = TypedDict(
     "CaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
         "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
-InputCaptionsOutputTypeDef = TypedDict(
-    "InputCaptionsOutputTypeDef",
-    {
-        "MergePolicy": str,
-        "CaptionSources": List[CaptionSourceTypeDef],
-    },
-    total=False,
-)
-
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigOutputTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -750,17 +652,32 @@
 )
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-PipelineOutputConfigUnionTypeDef = Union[
-    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
-]
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsTypeDef,
+        "ContentConfig": PipelineOutputConfigTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -778,30 +695,14 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersOutputTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
-    },
-    total=False,
-)
-
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -817,39 +718,26 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
     {
         "Id": str,
-        "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
-        "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtOutputTypeDef,
-        "Composition": List[ClipTypeDef],
-        "Captions": CaptionsOutputTypeDef,
-        "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersTypeDef,
+        "Video": VideoParametersTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
+        "Type": str,
     },
     total=False,
 )
 
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
@@ -864,27 +752,38 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-JobInputOutputTypeDef = TypedDict(
-    "JobInputOutputTypeDef",
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
+        "Id": str,
         "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
         "FrameRate": str,
-        "Resolution": str,
-        "AspectRatio": str,
-        "Interlaced": str,
-        "Container": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkTypeDef],
+        "AlbumArt": JobAlbumArtTypeDef,
+        "Composition": List[ClipTypeDef],
+        "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
-        "TimeSpan": TimeSpanTypeDef,
-        "InputCaptions": InputCaptionsOutputTypeDef,
-        "DetectedProperties": DetectedPropertiesTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -976,34 +875,58 @@
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PipelineId": str,
-        "Input": JobInputOutputTypeDef,
-        "Inputs": List[JobInputOutputTypeDef],
+        "Input": JobInputTypeDef,
+        "Inputs": List[JobInputTypeDef],
         "Output": JobOutputTypeDef,
         "Outputs": List[JobOutputTypeDef],
         "OutputKeyPrefix": str,
         "Playlists": List[PlaylistTypeDef],
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
-JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1029,32 +952,7 @@
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[JobInputUnionTypeDef],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.py` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt` & `types-aiobotocore-elastictranscoder-2.5.2.post2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

