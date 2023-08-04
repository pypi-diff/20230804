# Comparing `tmp/types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesis-video-archived-media-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.176643 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14232 2023-08-04 13:59:14.176643 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12633 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.176643 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2219 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.176643 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      964 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1021 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12136 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12119 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9790 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9788 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4118 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4113 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10215 2023-08-04 13:42:00.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10206 2023-08-04 13:42:00.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:59.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.176643 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14232 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1212 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       47 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,83 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_archived_media.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from types_aiobotocore_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/README.md` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/README.md`

 * *Files 20% similar despite different names*

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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,83 +265,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_archived_media.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from types_aiobotocore_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-archived-media",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__main__.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
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
@@ -177,14 +178,15 @@
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
@@ -263,26 +265,28 @@
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -261,26 +263,28 @@
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,83 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_archived_media.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from types_aiobotocore_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post2/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

