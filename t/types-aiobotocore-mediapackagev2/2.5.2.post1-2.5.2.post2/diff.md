# Comparing `tmp/types-aiobotocore-mediapackagev2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediapackagev2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackagev2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackagev2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1.tar` & `types-aiobotocore-mediapackagev2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:39.069525 types-aiobotocore-mediapackagev2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-08-02 14:52:39.069525 types-aiobotocore-mediapackagev2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:39.069525 types-aiobotocore-mediapackagev2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:39.065525 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-08-02 14:43:26.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:25.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:39.065525 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.816643 types-aiobotocore-mediapackagev2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13653 2023-08-04 13:59:17.816643 types-aiobotocore-mediapackagev2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12107 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.816643 types-aiobotocore-mediapackagev2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.806643 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1147 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1146 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21959 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21923 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9563 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9561 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4446 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4441 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26958 2023-08-04 13:44:38.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26917 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:37.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.816643 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13653 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/LICENSE` & `types-aiobotocore-mediapackagev2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/README.md` & `types-aiobotocore-mediapackagev2-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mediapackagev2
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.mediapackagev2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mediapackagev2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediapackagev2"></a>
 
 # types-aiobotocore-mediapackagev2
 
 [![PyPI - types-aiobotocore-mediapackagev2](https://img.shields.io/pypi/v/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackagev2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/)
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
 [types-aiobotocore-mediapackagev2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,116 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediapackagev2.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `mediapackagev2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/literals/).
+
 ```python
-from types_aiobotocore_mediapackagev2.literals import (
-    AdMarkerHlsType,
-    CmafEncryptionMethodType,
-    ContainerTypeType,
-    DrmSystemType,
-    ListChannelGroupsPaginatorName,
-    ListChannelsPaginatorName,
-    ListOriginEndpointsPaginatorName,
-    PresetSpeke20AudioType,
-    PresetSpeke20VideoType,
-    ScteFilterType,
-    TsEncryptionMethodType,
-    mediapackagev2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediapackagev2.literals import AdMarkerHlsType
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediapackagev2.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `mediapackagev2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2/type_defs/).
+
 ```python
-from types_aiobotocore_mediapackagev2.type_defs import (
-    ChannelGroupListConfigurationTypeDef,
-    ChannelListConfigurationTypeDef,
-    CreateChannelGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    IngestEndpointTypeDef,
-    ScteHlsTypeDef,
-    DeleteChannelGroupRequestRequestTypeDef,
-    DeleteChannelPolicyRequestRequestTypeDef,
-    DeleteChannelRequestRequestTypeDef,
-    DeleteOriginEndpointPolicyRequestRequestTypeDef,
-    DeleteOriginEndpointRequestRequestTypeDef,
-    EncryptionContractConfigurationTypeDef,
-    EncryptionMethodTypeDef,
-    GetChannelGroupRequestRequestTypeDef,
-    GetChannelPolicyRequestRequestTypeDef,
-    GetChannelRequestRequestTypeDef,
-    GetOriginEndpointPolicyRequestRequestTypeDef,
-    GetOriginEndpointRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListChannelGroupsRequestRequestTypeDef,
-    ListChannelsRequestRequestTypeDef,
-    ListHlsManifestConfigurationTypeDef,
-    ListLowLatencyHlsManifestConfigurationTypeDef,
-    ListOriginEndpointsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutChannelPolicyRequestRequestTypeDef,
-    PutOriginEndpointPolicyRequestRequestTypeDef,
-    ScteOutputTypeDef,
-    ScteTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateChannelGroupRequestRequestTypeDef,
-    UpdateChannelRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelGroupResponseTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
-    ListChannelGroupsResponseTypeDef,
-    ListChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateChannelGroupResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    GetChannelResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    CreateHlsManifestConfigurationTypeDef,
-    CreateLowLatencyHlsManifestConfigurationTypeDef,
-    GetHlsManifestConfigurationTypeDef,
-    GetLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    OriginEndpointListConfigurationTypeDef,
-    EncryptionOutputTypeDef,
-    EncryptionTypeDef,
-    ListOriginEndpointsResponseTypeDef,
-    SegmentOutputTypeDef,
-    SegmentTypeDef,
-    CreateOriginEndpointResponseTypeDef,
-    GetOriginEndpointResponseTypeDef,
-    UpdateOriginEndpointResponseTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
-    SegmentUnionTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
-)
+from types_aiobotocore_mediapackagev2.type_defs import ChannelGroupListConfigurationTypeDef
 
 
 def get_value() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/setup.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackagev2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.mediapackagev2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__init__.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__init__.pyi` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/__main__.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.mediapackagev2 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackagev2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
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

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/client.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     GetChannelResponseTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SegmentUnionTypeDef,
+    SegmentTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -143,15 +143,15 @@
     async def create_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: SegmentUnionTypeDef = ...,
+        Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
@@ -392,15 +392,15 @@
     async def update_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: SegmentUnionTypeDef = ...,
+        Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/client.pyi` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     GetChannelResponseTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SegmentUnionTypeDef,
+    SegmentTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -134,15 +134,15 @@
     async def create_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: SegmentUnionTypeDef = ...,
+        Segment: SegmentTypeDef = ...,
         ClientToken: str = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
@@ -361,15 +361,15 @@
     async def update_origin_endpoint(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
         OriginEndpointName: str,
         ContainerType: ContainerTypeType,
-        Segment: SegmentUnionTypeDef = ...,
+        Segment: SegmentTypeDef = ...,
         Description: str = ...,
         StartoverWindowSeconds: int = ...,
         HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,
         LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Update the specified origin endpoint.
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/literals.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -188,14 +189,15 @@
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
@@ -274,26 +276,28 @@
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
@@ -440,14 +444,15 @@
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/literals.pyi` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
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
@@ -186,14 +187,15 @@
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
@@ -272,26 +274,28 @@
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
@@ -438,14 +442,15 @@
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/paginator.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/paginator.pyi` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/type_defs.py` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_mediapackagev2.type_defs import ChannelGroupListConfigurationTypeDef
 
     data: ChannelGroupListConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     CmafEncryptionMethodType,
     ContainerTypeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -60,15 +60,14 @@
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
-    "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "CreateChannelGroupResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -82,31 +81,27 @@
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
-    "SegmentOutputTypeDef",
     "SegmentTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
-    "UpdateOriginEndpointResponseTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
-    "SegmentUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointResponseTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
@@ -461,22 +456,14 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
     },
 )
 
-ScteOutputTypeDef = TypedDict(
-    "ScteOutputTypeDef",
-    {
-        "ScteFilter": List[ScteFilterType],
-    },
-    total=False,
-)
-
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -778,25 +765,14 @@
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
 
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": List[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
         "ResourceId": str,
         "DrmSystems": Sequence[DrmSystemType],
         "RoleArn": str,
@@ -882,35 +858,14 @@
 
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
 
-_RequiredEncryptionOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOutputTypeDef",
-    {
-        "EncryptionMethod": EncryptionMethodTypeDef,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalEncryptionOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "KeyRotationIntervalSeconds": int,
-    },
-    total=False,
-)
-
-
-class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
-    pass
-
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -933,154 +888,140 @@
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentOutputTypeDef = TypedDict(
-    "SegmentOutputTypeDef",
-    {
-        "SegmentDurationSeconds": int,
-        "SegmentName": str,
-        "TsUseAudioRenditionGroup": bool,
-        "IncludeIframeOnlyStreams": bool,
-        "TsIncludeDvbSubtitles": bool,
-        "Scte": ScteOutputTypeDef,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
         "SegmentName": str,
         "TsUseAudioRenditionGroup": bool,
         "IncludeIframeOnlyStreams": bool,
         "TsIncludeDvbSubtitles": bool,
         "Scte": ScteTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
+    },
+)
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+    {
+        "Segment": SegmentTypeDef,
+        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetOriginEndpointResponseTypeDef = TypedDict(
-    "GetOriginEndpointResponseTypeDef",
+
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+):
+    pass
+
+
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
+        "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+GetOriginEndpointResponseTypeDef = TypedDict(
+    "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
+        "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
     },
 )
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Segment": SegmentTypeDef,
-        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
 
-SegmentUnionTypeDef = Union[SegmentTypeDef, SegmentOutputTypeDef]
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-    },
-)
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
-    {
         "Segment": SegmentTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2/type_defs.pyi` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_mediapackagev2.type_defs import ChannelGroupListConfigurationTypeDef
 
     data: ChannelGroupListConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     CmafEncryptionMethodType,
     ContainerTypeType,
     DrmSystemType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -59,15 +59,14 @@
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
-    "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "CreateChannelGroupResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -81,31 +80,27 @@
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
-    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
-    "SegmentOutputTypeDef",
     "SegmentTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
-    "UpdateOriginEndpointResponseTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
-    "SegmentUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointResponseTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
@@ -444,22 +439,14 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
     },
 )
 
-ScteOutputTypeDef = TypedDict(
-    "ScteOutputTypeDef",
-    {
-        "ScteFilter": List[ScteFilterType],
-    },
-    total=False,
-)
-
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -749,25 +736,14 @@
 
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": List[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
         "ResourceId": str,
         "DrmSystems": Sequence[DrmSystemType],
         "RoleArn": str,
@@ -847,33 +823,14 @@
 )
 
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
-_RequiredEncryptionOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOutputTypeDef",
-    {
-        "EncryptionMethod": EncryptionMethodTypeDef,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalEncryptionOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "KeyRotationIntervalSeconds": int,
-    },
-    total=False,
-)
-
-class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
-    pass
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -894,151 +851,136 @@
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SegmentOutputTypeDef = TypedDict(
-    "SegmentOutputTypeDef",
-    {
-        "SegmentDurationSeconds": int,
-        "SegmentName": str,
-        "TsUseAudioRenditionGroup": bool,
-        "IncludeIframeOnlyStreams": bool,
-        "TsIncludeDvbSubtitles": bool,
-        "Scte": ScteOutputTypeDef,
-        "Encryption": EncryptionOutputTypeDef,
-    },
-    total=False,
-)
-
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
         "SegmentName": str,
         "TsUseAudioRenditionGroup": bool,
         "IncludeIframeOnlyStreams": bool,
         "TsIncludeDvbSubtitles": bool,
         "Scte": ScteTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
+    },
+)
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+    {
+        "Segment": SegmentTypeDef,
+        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
 
-GetOriginEndpointResponseTypeDef = TypedDict(
-    "GetOriginEndpointResponseTypeDef",
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+):
+    pass
+
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
+        "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+GetOriginEndpointResponseTypeDef = TypedDict(
+    "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentOutputTypeDef,
+        "Segment": SegmentTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
     },
 )
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Segment": SegmentTypeDef,
-        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-SegmentUnionTypeDef = Union[SegmentTypeDef, SegmentOutputTypeDef]
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-    },
-)
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
-    {
         "Segment": SegmentTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
-
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-mediapackagev2-2.5.2.post1/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackagev2-2.5.2.post2/types_aiobotocore_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

