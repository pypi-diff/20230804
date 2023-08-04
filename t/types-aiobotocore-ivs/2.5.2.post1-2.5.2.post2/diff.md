# Comparing `tmp/types-aiobotocore-ivs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ivs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-ivs-2.5.2.post1.tar` & `types-aiobotocore-ivs-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.893556 types-aiobotocore-ivs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-08-02 14:52:28.893556 types-aiobotocore-ivs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.893556 types-aiobotocore-ivs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23181 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23625 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23604 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:09.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.893556 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:30.000000 types-aiobotocore-ivs-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13284 2023-08-04 13:59:13.266642 types-aiobotocore-ivs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11782 2023-08-04 13:41:30.000000 types-aiobotocore-ivs-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:41:30.000000 types-aiobotocore-ivs-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.266642 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1491 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1490 2023-08-04 13:41:30.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24722 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24678 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9616 2023-08-04 13:41:32.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9614 2023-08-04 13:41:32.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6466 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6459 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:31.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27013 2023-08-04 13:41:32.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26986 2023-08-04 13:41:32.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:30.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.266642 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13284 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/LICENSE` & `types-aiobotocore-ivs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.5.2.post1/README.md` & `types-aiobotocore-ivs-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ivs
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IVS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ivs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ivs"></a>
 
 # types-aiobotocore-ivs
 
 [![PyPI - types-aiobotocore-ivs](https://img.shields.io/pypi/v/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/)
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
 [types-aiobotocore-ivs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,127 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `IVS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/literals/).
+
 ```python
-from types_aiobotocore_ivs.literals import (
-    ChannelLatencyModeType,
-    ChannelTypeType,
-    ListChannelsPaginatorName,
-    ListPlaybackKeyPairsPaginatorName,
-    ListRecordingConfigurationsPaginatorName,
-    ListStreamKeysPaginatorName,
-    ListStreamsPaginatorName,
-    RecordingConfigurationStateType,
-    RecordingModeType,
-    StreamHealthType,
-    StreamStateType,
-    TranscodePresetType,
-    IVSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_ivs.literals import ChannelLatencyModeType
 
 
 def check_value(value: ChannelLatencyModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IVS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/type_defs/).
+
 ```python
-from types_aiobotocore_ivs.type_defs import (
-    AudioConfigurationTypeDef,
-    BatchErrorTypeDef,
-    BatchGetChannelRequestRequestTypeDef,
-    ChannelTypeDef,
-    ResponseMetadataTypeDef,
-    BatchGetStreamKeyRequestRequestTypeDef,
-    StreamKeyTypeDef,
-    ChannelSummaryTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    ThumbnailConfigurationTypeDef,
-    CreateStreamKeyRequestRequestTypeDef,
-    DeleteChannelRequestRequestTypeDef,
-    DeletePlaybackKeyPairRequestRequestTypeDef,
-    DeleteRecordingConfigurationRequestRequestTypeDef,
-    DeleteStreamKeyRequestRequestTypeDef,
-    S3DestinationConfigurationTypeDef,
-    GetChannelRequestRequestTypeDef,
-    GetPlaybackKeyPairRequestRequestTypeDef,
-    PlaybackKeyPairTypeDef,
-    GetRecordingConfigurationRequestRequestTypeDef,
-    GetStreamKeyRequestRequestTypeDef,
-    GetStreamRequestRequestTypeDef,
-    StreamTypeDef,
-    GetStreamSessionRequestRequestTypeDef,
-    ImportPlaybackKeyPairRequestRequestTypeDef,
-    VideoConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestRequestTypeDef,
-    PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestRequestTypeDef,
-    StreamKeySummaryTypeDef,
-    ListStreamSessionsRequestRequestTypeDef,
-    StreamSessionSummaryTypeDef,
-    StreamFiltersTypeDef,
-    StreamSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutMetadataRequestRequestTypeDef,
-    StopStreamRequestRequestTypeDef,
-    StreamEventTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateChannelRequestRequestTypeDef,
-    BatchGetChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    BatchGetStreamKeyResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateStreamKeyResponseTypeDef,
-    GetStreamKeyResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    DestinationConfigurationTypeDef,
-    GetPlaybackKeyPairResponseTypeDef,
-    ImportPlaybackKeyPairResponseTypeDef,
-    GetStreamResponseTypeDef,
-    IngestConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    ListPlaybackKeyPairsResponseTypeDef,
-    ListStreamKeysResponseTypeDef,
-    ListStreamSessionsResponseTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
-    ListStreamsRequestRequestTypeDef,
-    ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
-    RecordingConfigurationSummaryTypeDef,
-    RecordingConfigurationTypeDef,
-    ListRecordingConfigurationsResponseTypeDef,
-    CreateRecordingConfigurationResponseTypeDef,
-    GetRecordingConfigurationResponseTypeDef,
-    StreamSessionTypeDef,
-    GetStreamSessionResponseTypeDef,
-)
+from types_aiobotocore_ivs.type_defs import AudioConfigurationTypeDef
 
 
 def get_value() -> AudioConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/setup.py` & `types-aiobotocore-ivs-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IVS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__init__.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__init__.pyi` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/__main__.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IVS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IVS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
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

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/client.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     ListRecordingConfigurationsPaginator,
     ListStreamKeysPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     BatchGetChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     CreateChannelResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     DestinationConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
@@ -46,14 +48,15 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -117,14 +120,25 @@
         """
         Performs  GetStreamKey on multiple ARNs simultaneously.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_get_stream_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#batch_get_stream_key)
         """
 
+    async def batch_start_viewer_session_revocation(
+        self, *, viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef]
+    ) -> BatchStartViewerSessionRevocationResponseTypeDef:
+        """
+        Performs  StartViewerSessionRevocation on multiple channel ARN and viewer ID
+        pairs simultaneously.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_start_viewer_session_revocation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#batch_start_viewer_session_revocation)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#can_paginate)
         """
@@ -158,14 +172,15 @@
 
     async def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
@@ -376,14 +391,25 @@
         """
         Inserts metadata into the active stream of the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.put_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#put_metadata)
         """
 
+    async def start_viewer_session_revocation(
+        self, *, channelArn: str, viewerId: str, viewerSessionVersionsLessThanOrEqualTo: int = ...
+    ) -> Dict[str, Any]:
+        """
+        Starts the process of revoking the viewer session associated with a specified
+        channel ARN and viewer ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.start_viewer_session_revocation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#start_viewer_session_revocation)
+        """
+
     async def stop_stream(self, *, channelArn: str) -> Dict[str, Any]:
         """
         Disconnects the incoming RTMPS stream for the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.stop_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#stop_stream)
         """
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/client.pyi` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     ListRecordingConfigurationsPaginator,
     ListStreamKeysPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     BatchGetChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
+    BatchStartViewerSessionRevocationResponseTypeDef,
+    BatchStartViewerSessionRevocationViewerSessionTypeDef,
     CreateChannelResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     DestinationConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
@@ -46,14 +48,15 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -110,14 +113,24 @@
     ) -> BatchGetStreamKeyResponseTypeDef:
         """
         Performs  GetStreamKey on multiple ARNs simultaneously.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_get_stream_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#batch_get_stream_key)
         """
+    async def batch_start_viewer_session_revocation(
+        self, *, viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef]
+    ) -> BatchStartViewerSessionRevocationResponseTypeDef:
+        """
+        Performs  StartViewerSessionRevocation on multiple channel ARN and viewer ID
+        pairs simultaneously.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.batch_start_viewer_session_revocation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#batch_start_viewer_session_revocation)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#can_paginate)
         """
@@ -148,14 +161,15 @@
         """
     async def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
@@ -344,14 +358,24 @@
     async def put_metadata(self, *, channelArn: str, metadata: str) -> EmptyResponseMetadataTypeDef:
         """
         Inserts metadata into the active stream of the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.put_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#put_metadata)
         """
+    async def start_viewer_session_revocation(
+        self, *, channelArn: str, viewerId: str, viewerSessionVersionsLessThanOrEqualTo: int = ...
+    ) -> Dict[str, Any]:
+        """
+        Starts the process of revoking the viewer session associated with a specified
+        channel ARN and viewer ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.start_viewer_session_revocation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#start_viewer_session_revocation)
+        """
     async def stop_stream(self, *, channelArn: str) -> Dict[str, Any]:
         """
         Disconnects the incoming RTMPS stream for the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.stop_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs/client/#stop_stream)
         """
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/literals.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     "ListChannelsPaginatorName",
     "ListPlaybackKeyPairsPaginatorName",
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
+    "RenditionConfigurationRenditionSelectionType",
+    "RenditionConfigurationRenditionType",
     "StreamHealthType",
     "StreamStateType",
+    "ThumbnailConfigurationResolutionType",
+    "ThumbnailConfigurationStorageType",
     "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -45,16 +49,20 @@
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
+RenditionConfigurationRenditionSelectionType = Literal["ALL", "CUSTOM", "NONE"]
+RenditionConfigurationRenditionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+ThumbnailConfigurationResolutionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
+ThumbnailConfigurationStorageType = Literal["LATEST", "SEQUENTIAL"]
 TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -64,14 +72,15 @@
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
@@ -167,14 +176,15 @@
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
@@ -253,26 +263,28 @@
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

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/literals.pyi` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     "ListChannelsPaginatorName",
     "ListPlaybackKeyPairsPaginatorName",
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
+    "RenditionConfigurationRenditionSelectionType",
+    "RenditionConfigurationRenditionType",
     "StreamHealthType",
     "StreamStateType",
+    "ThumbnailConfigurationResolutionType",
+    "ThumbnailConfigurationStorageType",
     "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -43,16 +47,20 @@
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
+RenditionConfigurationRenditionSelectionType = Literal["ALL", "CUSTOM", "NONE"]
+RenditionConfigurationRenditionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+ThumbnailConfigurationResolutionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
+ThumbnailConfigurationStorageType = Literal["LATEST", "SEQUENTIAL"]
 TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -62,14 +70,15 @@
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
@@ -165,14 +174,15 @@
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
@@ -251,26 +261,28 @@
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

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/paginator.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/paginator.pyi` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/type_defs.py` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -35,16 +39,19 @@
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
+    "BatchStartViewerSessionRevocationErrorTypeDef",
+    "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
@@ -67,28 +74,31 @@
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
@@ -182,14 +192,61 @@
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
     total=False,
 )
 
+_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "code": str,
+        "message": str,
+    },
+    total=False,
+)
+
+
+class BatchStartViewerSessionRevocationErrorTypeDef(
+    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
+    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
+):
+    pass
+
+
+_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+
+class BatchStartViewerSessionRevocationViewerSessionTypeDef(
+    _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef,
+    _OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef,
+):
+    pass
+
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "arn": str,
         "authorized": bool,
         "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
@@ -213,18 +270,29 @@
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
+RenditionConfigurationTypeDef = TypedDict(
+    "RenditionConfigurationTypeDef",
+    {
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": Sequence[RenditionConfigurationRenditionType],
+    },
+    total=False,
+)
+
 ThumbnailConfigurationTypeDef = TypedDict(
     "ThumbnailConfigurationTypeDef",
     {
         "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": Sequence[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
     total=False,
 )
 
 _RequiredCreateStreamKeyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamKeyRequestRequestTypeDef",
@@ -548,14 +616,37 @@
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
+_RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+
+class StartViewerSessionRevocationRequestRequestTypeDef(
+    _RequiredStartViewerSessionRevocationRequestRequestTypeDef,
+    _OptionalStartViewerSessionRevocationRequestRequestTypeDef,
+):
+    pass
+
+
 StopStreamRequestRequestTypeDef = TypedDict(
     "StopStreamRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
@@ -682,14 +773,29 @@
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    {
+        "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -846,14 +952,15 @@
     },
 )
 _OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
         "tags": Mapping[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 
@@ -897,14 +1004,15 @@
     },
 )
 _OptionalRecordingConfigurationTypeDef = TypedDict(
     "_OptionalRecordingConfigurationTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
         "tags": Dict[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs/type_defs.pyi` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,20 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -34,16 +38,19 @@
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
+    "BatchStartViewerSessionRevocationErrorTypeDef",
+    "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
@@ -66,28 +73,31 @@
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
@@ -181,14 +191,57 @@
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
     total=False,
 )
 
+_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
+    {
+        "code": str,
+        "message": str,
+    },
+    total=False,
+)
+
+class BatchStartViewerSessionRevocationErrorTypeDef(
+    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
+    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
+):
+    pass
+
+_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
+    "_OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+class BatchStartViewerSessionRevocationViewerSessionTypeDef(
+    _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef,
+    _OptionalBatchStartViewerSessionRevocationViewerSessionTypeDef,
+):
+    pass
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "arn": str,
         "authorized": bool,
         "insecureIngest": bool,
         "latencyMode": ChannelLatencyModeType,
@@ -212,18 +265,29 @@
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
+RenditionConfigurationTypeDef = TypedDict(
+    "RenditionConfigurationTypeDef",
+    {
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": Sequence[RenditionConfigurationRenditionType],
+    },
+    total=False,
+)
+
 ThumbnailConfigurationTypeDef = TypedDict(
     "ThumbnailConfigurationTypeDef",
     {
         "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": Sequence[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
     total=False,
 )
 
 _RequiredCreateStreamKeyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamKeyRequestRequestTypeDef",
@@ -537,14 +601,35 @@
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
+_RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "channelArn": str,
+        "viewerId": str,
+    },
+)
+_OptionalStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessionVersionsLessThanOrEqualTo": int,
+    },
+    total=False,
+)
+
+class StartViewerSessionRevocationRequestRequestTypeDef(
+    _RequiredStartViewerSessionRevocationRequestRequestTypeDef,
+    _OptionalStartViewerSessionRevocationRequestRequestTypeDef,
+):
+    pass
+
 StopStreamRequestRequestTypeDef = TypedDict(
     "StopStreamRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
@@ -669,14 +754,29 @@
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationResponseTypeDef",
+    {
+        "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationRequestRequestTypeDef",
+    {
+        "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
+    },
+)
+
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -831,14 +931,15 @@
     },
 )
 _OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
         "tags": Mapping[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 class CreateRecordingConfigurationRequestRequestTypeDef(
@@ -878,14 +979,15 @@
     },
 )
 _OptionalRecordingConfigurationTypeDef = TypedDict(
     "_OptionalRecordingConfigurationTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationTypeDef,
         "tags": Dict[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 class RecordingConfigurationTypeDef(
```

### Comparing `types-aiobotocore-ivs-2.5.2.post1/types_aiobotocore_ivs.egg-info/SOURCES.txt` & `types-aiobotocore-ivs-2.5.2.post2/types_aiobotocore_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

