# Comparing `tmp/types-aiobotocore-mediapackage-vod-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediapackage-vod-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackage-vod-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackage-vod-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1.tar` & `types-aiobotocore-mediapackage-vod-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.801525 types-aiobotocore-mediapackage-vod-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-08-02 14:52:38.793526 types-aiobotocore-mediapackage-vod-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.801525 types-aiobotocore-mediapackage-vod-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.785525 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25006 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-08-02 14:43:24.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.793526 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.576643 types-aiobotocore-mediapackage-vod-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13756 2023-08-04 13:59:17.576643 types-aiobotocore-mediapackage-vod-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12203 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.576643 types-aiobotocore-mediapackage-vod-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2134 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.576643 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1206 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1205 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      977 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16842 2023-08-04 13:44:34.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16813 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9586 2023-08-04 13:44:34.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9584 2023-08-04 13:44:34.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4561 2023-08-04 13:44:34.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4556 2023-08-04 13:44:34.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20133 2023-08-04 13:44:36.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20108 2023-08-04 13:44:35.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:33.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.576643 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13756 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/LICENSE` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/PKG-INFO` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage-vod
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MediaPackageVod 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MediaPackageVod 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/
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
 [types-aiobotocore-mediapackage-vod docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,119 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediapackage_vod.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MediaPackageVod` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/literals/).
+
 ```python
-from types_aiobotocore_mediapackage_vod.literals import (
-    AdMarkersType,
-    EncryptionMethodType,
-    ListAssetsPaginatorName,
-    ListPackagingConfigurationsPaginatorName,
-    ListPackagingGroupsPaginatorName,
-    ManifestLayoutType,
-    PeriodTriggersElementType,
-    PresetSpeke20AudioType,
-    PresetSpeke20VideoType,
-    ProfileType,
-    ScteMarkersSourceType,
-    SegmentTemplateFormatType,
-    StreamOrderType,
-    MediaPackageVodServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediapackage_vod.literals import AdMarkersType
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediapackage_vod.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaPackageVod` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/type_defs/).
+
 ```python
-from types_aiobotocore_mediapackage_vod.type_defs import (
-    AssetShallowTypeDef,
-    AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    ResponseMetadataTypeDef,
-    CreateAssetRequestRequestTypeDef,
-    EgressEndpointTypeDef,
-    StreamSelectionTypeDef,
-    DeleteAssetRequestRequestTypeDef,
-    DeletePackagingConfigurationRequestRequestTypeDef,
-    DeletePackagingGroupRequestRequestTypeDef,
-    DescribeAssetRequestRequestTypeDef,
-    DescribePackagingConfigurationRequestRequestTypeDef,
-    DescribePackagingGroupRequestRequestTypeDef,
-    EncryptionContractConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ListAssetsRequestRequestTypeDef,
-    ListPackagingConfigurationsRequestRequestTypeDef,
-    ListPackagingGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdatePackagingGroupRequestRequestTypeDef,
-    ConfigureLogsRequestRequestTypeDef,
-    CreatePackagingGroupRequestRequestTypeDef,
-    PackagingGroupTypeDef,
-    ConfigureLogsResponseTypeDef,
-    CreatePackagingGroupResponseTypeDef,
-    DescribePackagingGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAssetsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdatePackagingGroupResponseTypeDef,
-    CreateAssetResponseTypeDef,
-    DescribeAssetResponseTypeDef,
-    DashManifestTypeDef,
-    HlsManifestTypeDef,
-    MssManifestTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
-    ListPackagingGroupsResponseTypeDef,
-    CmafEncryptionOutputTypeDef,
-    DashEncryptionOutputTypeDef,
-    HlsEncryptionOutputTypeDef,
-    MssEncryptionOutputTypeDef,
-    CmafEncryptionTypeDef,
-    DashEncryptionTypeDef,
-    HlsEncryptionTypeDef,
-    MssEncryptionTypeDef,
-    CmafPackageOutputTypeDef,
-    DashPackageOutputTypeDef,
-    HlsPackageOutputTypeDef,
-    MssPackageOutputTypeDef,
-    CmafPackageTypeDef,
-    DashPackageTypeDef,
-    HlsPackageTypeDef,
-    MssPackageTypeDef,
-    CreatePackagingConfigurationResponseTypeDef,
-    DescribePackagingConfigurationResponseTypeDef,
-    PackagingConfigurationTypeDef,
-    CmafPackageUnionTypeDef,
-    DashPackageUnionTypeDef,
-    HlsPackageUnionTypeDef,
-    CreatePackagingConfigurationRequestRequestTypeDef,
-    MssPackageUnionTypeDef,
-    ListPackagingConfigurationsResponseTypeDef,
-)
+from types_aiobotocore_mediapackage_vod.type_defs import AssetShallowTypeDef
 
 
 def get_value() -> AssetShallowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/README.md` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mediapackage-vod
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MediaPackageVod 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mediapackage-vod type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediapackage-vod"></a>
 
 # types-aiobotocore-mediapackage-vod
 
 [![PyPI - types-aiobotocore-mediapackage-vod](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/)
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
 [types-aiobotocore-mediapackage-vod docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,119 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediapackage_vod.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MediaPackageVod` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/literals/).
+
 ```python
-from types_aiobotocore_mediapackage_vod.literals import (
-    AdMarkersType,
-    EncryptionMethodType,
-    ListAssetsPaginatorName,
-    ListPackagingConfigurationsPaginatorName,
-    ListPackagingGroupsPaginatorName,
-    ManifestLayoutType,
-    PeriodTriggersElementType,
-    PresetSpeke20AudioType,
-    PresetSpeke20VideoType,
-    ProfileType,
-    ScteMarkersSourceType,
-    SegmentTemplateFormatType,
-    StreamOrderType,
-    MediaPackageVodServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediapackage_vod.literals import AdMarkersType
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediapackage_vod.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaPackageVod` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/type_defs/).
+
 ```python
-from types_aiobotocore_mediapackage_vod.type_defs import (
-    AssetShallowTypeDef,
-    AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    ResponseMetadataTypeDef,
-    CreateAssetRequestRequestTypeDef,
-    EgressEndpointTypeDef,
-    StreamSelectionTypeDef,
-    DeleteAssetRequestRequestTypeDef,
-    DeletePackagingConfigurationRequestRequestTypeDef,
-    DeletePackagingGroupRequestRequestTypeDef,
-    DescribeAssetRequestRequestTypeDef,
-    DescribePackagingConfigurationRequestRequestTypeDef,
-    DescribePackagingGroupRequestRequestTypeDef,
-    EncryptionContractConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ListAssetsRequestRequestTypeDef,
-    ListPackagingConfigurationsRequestRequestTypeDef,
-    ListPackagingGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdatePackagingGroupRequestRequestTypeDef,
-    ConfigureLogsRequestRequestTypeDef,
-    CreatePackagingGroupRequestRequestTypeDef,
-    PackagingGroupTypeDef,
-    ConfigureLogsResponseTypeDef,
-    CreatePackagingGroupResponseTypeDef,
-    DescribePackagingGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAssetsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdatePackagingGroupResponseTypeDef,
-    CreateAssetResponseTypeDef,
-    DescribeAssetResponseTypeDef,
-    DashManifestTypeDef,
-    HlsManifestTypeDef,
-    MssManifestTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
-    ListAssetsRequestListAssetsPaginateTypeDef,
-    ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
-    ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
-    ListPackagingGroupsResponseTypeDef,
-    CmafEncryptionOutputTypeDef,
-    DashEncryptionOutputTypeDef,
-    HlsEncryptionOutputTypeDef,
-    MssEncryptionOutputTypeDef,
-    CmafEncryptionTypeDef,
-    DashEncryptionTypeDef,
-    HlsEncryptionTypeDef,
-    MssEncryptionTypeDef,
-    CmafPackageOutputTypeDef,
-    DashPackageOutputTypeDef,
-    HlsPackageOutputTypeDef,
-    MssPackageOutputTypeDef,
-    CmafPackageTypeDef,
-    DashPackageTypeDef,
-    HlsPackageTypeDef,
-    MssPackageTypeDef,
-    CreatePackagingConfigurationResponseTypeDef,
-    DescribePackagingConfigurationResponseTypeDef,
-    PackagingConfigurationTypeDef,
-    CmafPackageUnionTypeDef,
-    DashPackageUnionTypeDef,
-    HlsPackageUnionTypeDef,
-    CreatePackagingConfigurationRequestRequestTypeDef,
-    MssPackageUnionTypeDef,
-    ListPackagingConfigurationsResponseTypeDef,
-)
+from types_aiobotocore_mediapackage_vod.type_defs import AssetShallowTypeDef
 
 
 def get_value() -> AssetShallowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/setup.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackage-vod",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaPackageVod 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__init__.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__init__.pyi` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/__main__.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MediaPackageVod 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/client.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
-    CmafPackageUnionTypeDef,
+    CmafPackageTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
-    DashPackageUnionTypeDef,
+    DashPackageTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageUnionTypeDef,
+    HlsPackageTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageUnionTypeDef,
+    MssPackageTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -138,18 +138,18 @@
         """
 
     async def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: CmafPackageUnionTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        CmafPackage: CmafPackageTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/client.pyi` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 from .paginator import (
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 from .type_defs import (
     AuthorizationTypeDef,
-    CmafPackageUnionTypeDef,
+    CmafPackageTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateAssetResponseTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
-    DashPackageUnionTypeDef,
+    DashPackageTypeDef,
     DescribeAssetResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageUnionTypeDef,
+    HlsPackageTypeDef,
     ListAssetsResponseTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
     ListPackagingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageUnionTypeDef,
+    MssPackageTypeDef,
     UpdatePackagingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -129,18 +129,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_asset)
         """
     async def create_packaging_configuration(
         self,
         *,
         Id: str,
         PackagingGroupId: str,
-        CmafPackage: CmafPackageUnionTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        CmafPackage: CmafPackageTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_configuration)
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/literals.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
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
@@ -184,14 +185,15 @@
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
@@ -270,26 +272,28 @@
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
@@ -436,14 +440,15 @@
 PaginatorName = Literal["list_assets", "list_packaging_configurations", "list_packaging_groups"]
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

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/literals.pyi` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
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
@@ -182,14 +183,15 @@
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
@@ -268,26 +270,28 @@
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
@@ -434,14 +438,15 @@
 PaginatorName = Literal["list_assets", "list_packaging_configurations", "list_packaging_groups"]
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

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/paginator.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/paginator.pyi` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/type_defs.py` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/type_defs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mediapackage_vod.type_defs import AssetShallowTypeDef
 
     data: AssetShallowTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
     EncryptionMethodType,
     ManifestLayoutType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetShallowTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
@@ -70,44 +69,31 @@
     "ListTagsForResourceResponseTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
-    "CmafEncryptionOutputTypeDef",
-    "DashEncryptionOutputTypeDef",
-    "HlsEncryptionOutputTypeDef",
-    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
-    "CmafPackageOutputTypeDef",
-    "DashPackageOutputTypeDef",
-    "HlsPackageOutputTypeDef",
-    "MssPackageOutputTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
+    "CreatePackagingConfigurationRequestRequestTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
-    "CmafPackageUnionTypeDef",
-    "DashPackageUnionTypeDef",
-    "HlsPackageUnionTypeDef",
-    "CreatePackagingConfigurationRequestRequestTypeDef",
-    "MssPackageUnionTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -163,21 +149,19 @@
     {
         "ResourceId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
-
 EgressEndpointTypeDef = TypedDict(
     "EgressEndpointTypeDef",
     {
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
@@ -316,43 +300,39 @@
     "_OptionalUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePackagingGroupRequestRequestTypeDef(
     _RequiredUpdatePackagingGroupRequestRequestTypeDef,
     _OptionalUpdatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
     "_OptionalConfigureLogsRequestRequestTypeDef",
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
     },
     total=False,
 )
 
-
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -361,22 +341,20 @@
         "Authorization": AuthorizationTypeDef,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
-
 PackagingGroupTypeDef = TypedDict(
     "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
@@ -533,37 +511,14 @@
     {
         "ManifestName": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
-_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_RequiredSpekeKeyProviderOutputTypeDef",
-    {
-        "RoleArn": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-)
-_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_OptionalSpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SpekeKeyProviderOutputTypeDef(
-    _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
-):
-    pass
-
-
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -572,19 +527,17 @@
     "_OptionalSpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
-
 ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsRequestListAssetsPaginateTypeDef",
     {
         "PackagingGroupId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -612,90 +565,31 @@
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCmafEncryptionOutputTypeDef = TypedDict(
-    "_RequiredCmafEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalCmafEncryptionOutputTypeDef = TypedDict(
-    "_OptionalCmafEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-    },
-    total=False,
-)
-
-
-class CmafEncryptionOutputTypeDef(
-    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
-):
-    pass
-
-
-DashEncryptionOutputTypeDef = TypedDict(
-    "DashEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-
-_RequiredHlsEncryptionOutputTypeDef = TypedDict(
-    "_RequiredHlsEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalHlsEncryptionOutputTypeDef = TypedDict(
-    "_OptionalHlsEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": EncryptionMethodType,
-    },
-    total=False,
-)
-
-
-class HlsEncryptionOutputTypeDef(
-    _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
-):
-    pass
-
-
-MssEncryptionOutputTypeDef = TypedDict(
-    "MssEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalCmafEncryptionTypeDef = TypedDict(
     "_OptionalCmafEncryptionTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
-
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
-
 DashEncryptionTypeDef = TypedDict(
     "DashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
@@ -710,117 +604,24 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
-
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
-
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
-_RequiredCmafPackageOutputTypeDef = TypedDict(
-    "_RequiredCmafPackageOutputTypeDef",
-    {
-        "HlsManifests": List[HlsManifestTypeDef],
-    },
-)
-_OptionalCmafPackageOutputTypeDef = TypedDict(
-    "_OptionalCmafPackageOutputTypeDef",
-    {
-        "Encryption": CmafEncryptionOutputTypeDef,
-        "IncludeEncoderConfigurationInSegments": bool,
-        "SegmentDurationSeconds": int,
-    },
-    total=False,
-)
-
-
-class CmafPackageOutputTypeDef(
-    _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
-):
-    pass
-
-
-_RequiredDashPackageOutputTypeDef = TypedDict(
-    "_RequiredDashPackageOutputTypeDef",
-    {
-        "DashManifests": List[DashManifestTypeDef],
-    },
-)
-_OptionalDashPackageOutputTypeDef = TypedDict(
-    "_OptionalDashPackageOutputTypeDef",
-    {
-        "Encryption": DashEncryptionOutputTypeDef,
-        "IncludeEncoderConfigurationInSegments": bool,
-        "IncludeIframeOnlyStream": bool,
-        "PeriodTriggers": List[Literal["ADS"]],
-        "SegmentDurationSeconds": int,
-        "SegmentTemplateFormat": SegmentTemplateFormatType,
-    },
-    total=False,
-)
-
-
-class DashPackageOutputTypeDef(
-    _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
-):
-    pass
-
-
-_RequiredHlsPackageOutputTypeDef = TypedDict(
-    "_RequiredHlsPackageOutputTypeDef",
-    {
-        "HlsManifests": List[HlsManifestTypeDef],
-    },
-)
-_OptionalHlsPackageOutputTypeDef = TypedDict(
-    "_OptionalHlsPackageOutputTypeDef",
-    {
-        "Encryption": HlsEncryptionOutputTypeDef,
-        "IncludeDvbSubtitles": bool,
-        "SegmentDurationSeconds": int,
-        "UseAudioRenditionGroup": bool,
-    },
-    total=False,
-)
-
-
-class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
-    pass
-
-
-_RequiredMssPackageOutputTypeDef = TypedDict(
-    "_RequiredMssPackageOutputTypeDef",
-    {
-        "MssManifests": List[MssManifestTypeDef],
-    },
-)
-_OptionalMssPackageOutputTypeDef = TypedDict(
-    "_OptionalMssPackageOutputTypeDef",
-    {
-        "Encryption": MssEncryptionOutputTypeDef,
-        "SegmentDurationSeconds": int,
-    },
-    total=False,
-)
-
-
-class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
-    pass
-
-
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -829,19 +630,17 @@
         "Encryption": CmafEncryptionTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class CmafPackageTypeDef(_RequiredCmafPackageTypeDef, _OptionalCmafPackageTypeDef):
     pass
 
-
 _RequiredDashPackageTypeDef = TypedDict(
     "_RequiredDashPackageTypeDef",
     {
         "DashManifests": Sequence[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageTypeDef = TypedDict(
@@ -853,19 +652,17 @@
         "PeriodTriggers": Sequence[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
-
 class DashPackageTypeDef(_RequiredDashPackageTypeDef, _OptionalDashPackageTypeDef):
     pass
 
-
 _RequiredHlsPackageTypeDef = TypedDict(
     "_RequiredHlsPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageTypeDef = TypedDict(
@@ -875,19 +672,17 @@
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
-
 class HlsPackageTypeDef(_RequiredHlsPackageTypeDef, _OptionalHlsPackageTypeDef):
     pass
 
-
 _RequiredMssPackageTypeDef = TypedDict(
     "_RequiredMssPackageTypeDef",
     {
         "MssManifests": Sequence[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageTypeDef = TypedDict(
@@ -895,98 +690,90 @@
     {
         "Encryption": MssEncryptionTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
-
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
+_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "Id": str,
+        "PackagingGroupId": str,
+    },
+)
+_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "CmafPackage": CmafPackageTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
+        "MssPackage": MssPackageTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreatePackagingConfigurationRequestRequestTypeDef(
+    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
+    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
+):
+    pass
 
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
-        "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
-        "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
-        "PackagingGroupId": str,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-CmafPackageUnionTypeDef = Union[CmafPackageTypeDef, CmafPackageOutputTypeDef]
-DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
-HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
-_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "Id": str,
-        "PackagingGroupId": str,
-    },
-)
-_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
-    {
         "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
+        "Id": str,
         "MssPackage": MssPackageTypeDef,
-        "Tags": Mapping[str, str],
+        "PackagingGroupId": str,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
-class CreatePackagingConfigurationRequestRequestTypeDef(
-    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
-    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod/type_defs.pyi` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mediapackage_vod.type_defs import AssetShallowTypeDef
 
     data: AssetShallowTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
     EncryptionMethodType,
     ManifestLayoutType,
     PresetSpeke20AudioType,
     PresetSpeke20VideoType,
@@ -31,14 +31,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssetShallowTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
@@ -69,44 +70,31 @@
     "ListTagsForResourceResponseTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsResponseTypeDef",
-    "CmafEncryptionOutputTypeDef",
-    "DashEncryptionOutputTypeDef",
-    "HlsEncryptionOutputTypeDef",
-    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
-    "CmafPackageOutputTypeDef",
-    "DashPackageOutputTypeDef",
-    "HlsPackageOutputTypeDef",
-    "MssPackageOutputTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
+    "CreatePackagingConfigurationRequestRequestTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
-    "CmafPackageUnionTypeDef",
-    "DashPackageUnionTypeDef",
-    "HlsPackageUnionTypeDef",
-    "CreatePackagingConfigurationRequestRequestTypeDef",
-    "MssPackageUnionTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -162,19 +150,21 @@
     {
         "ResourceId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAssetRequestRequestTypeDef(
     _RequiredCreateAssetRequestRequestTypeDef, _OptionalCreateAssetRequestRequestTypeDef
 ):
     pass
 
+
 EgressEndpointTypeDef = TypedDict(
     "EgressEndpointTypeDef",
     {
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
@@ -313,39 +303,43 @@
     "_OptionalUpdatePackagingGroupRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePackagingGroupRequestRequestTypeDef(
     _RequiredUpdatePackagingGroupRequestRequestTypeDef,
     _OptionalUpdatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
     "_OptionalConfigureLogsRequestRequestTypeDef",
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
     },
     total=False,
 )
 
+
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -354,20 +348,22 @@
         "Authorization": AuthorizationTypeDef,
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+
 PackagingGroupTypeDef = TypedDict(
     "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "CreatedAt": str,
@@ -524,35 +520,14 @@
     {
         "ManifestName": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
-_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_RequiredSpekeKeyProviderOutputTypeDef",
-    {
-        "RoleArn": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-)
-_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_OptionalSpekeKeyProviderOutputTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SpekeKeyProviderOutputTypeDef(
-    _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
-):
-    pass
-
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -561,17 +536,19 @@
     "_OptionalSpekeKeyProviderTypeDef",
     {
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
+
 ListAssetsRequestListAssetsPaginateTypeDef = TypedDict(
     "ListAssetsRequestListAssetsPaginateTypeDef",
     {
         "PackagingGroupId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -599,84 +576,33 @@
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCmafEncryptionOutputTypeDef = TypedDict(
-    "_RequiredCmafEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalCmafEncryptionOutputTypeDef = TypedDict(
-    "_OptionalCmafEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-    },
-    total=False,
-)
-
-class CmafEncryptionOutputTypeDef(
-    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
-):
-    pass
-
-DashEncryptionOutputTypeDef = TypedDict(
-    "DashEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-
-_RequiredHlsEncryptionOutputTypeDef = TypedDict(
-    "_RequiredHlsEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalHlsEncryptionOutputTypeDef = TypedDict(
-    "_OptionalHlsEncryptionOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": EncryptionMethodType,
-    },
-    total=False,
-)
-
-class HlsEncryptionOutputTypeDef(
-    _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
-):
-    pass
-
-MssEncryptionOutputTypeDef = TypedDict(
-    "MssEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalCmafEncryptionTypeDef = TypedDict(
     "_OptionalCmafEncryptionTypeDef",
     {
         "ConstantInitializationVector": str,
     },
     total=False,
 )
 
+
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
+
 DashEncryptionTypeDef = TypedDict(
     "DashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
@@ -691,107 +617,26 @@
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": EncryptionMethodType,
     },
     total=False,
 )
 
+
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
+
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
-_RequiredCmafPackageOutputTypeDef = TypedDict(
-    "_RequiredCmafPackageOutputTypeDef",
-    {
-        "HlsManifests": List[HlsManifestTypeDef],
-    },
-)
-_OptionalCmafPackageOutputTypeDef = TypedDict(
-    "_OptionalCmafPackageOutputTypeDef",
-    {
-        "Encryption": CmafEncryptionOutputTypeDef,
-        "IncludeEncoderConfigurationInSegments": bool,
-        "SegmentDurationSeconds": int,
-    },
-    total=False,
-)
-
-class CmafPackageOutputTypeDef(
-    _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
-):
-    pass
-
-_RequiredDashPackageOutputTypeDef = TypedDict(
-    "_RequiredDashPackageOutputTypeDef",
-    {
-        "DashManifests": List[DashManifestTypeDef],
-    },
-)
-_OptionalDashPackageOutputTypeDef = TypedDict(
-    "_OptionalDashPackageOutputTypeDef",
-    {
-        "Encryption": DashEncryptionOutputTypeDef,
-        "IncludeEncoderConfigurationInSegments": bool,
-        "IncludeIframeOnlyStream": bool,
-        "PeriodTriggers": List[Literal["ADS"]],
-        "SegmentDurationSeconds": int,
-        "SegmentTemplateFormat": SegmentTemplateFormatType,
-    },
-    total=False,
-)
-
-class DashPackageOutputTypeDef(
-    _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
-):
-    pass
-
-_RequiredHlsPackageOutputTypeDef = TypedDict(
-    "_RequiredHlsPackageOutputTypeDef",
-    {
-        "HlsManifests": List[HlsManifestTypeDef],
-    },
-)
-_OptionalHlsPackageOutputTypeDef = TypedDict(
-    "_OptionalHlsPackageOutputTypeDef",
-    {
-        "Encryption": HlsEncryptionOutputTypeDef,
-        "IncludeDvbSubtitles": bool,
-        "SegmentDurationSeconds": int,
-        "UseAudioRenditionGroup": bool,
-    },
-    total=False,
-)
-
-class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
-    pass
-
-_RequiredMssPackageOutputTypeDef = TypedDict(
-    "_RequiredMssPackageOutputTypeDef",
-    {
-        "MssManifests": List[MssManifestTypeDef],
-    },
-)
-_OptionalMssPackageOutputTypeDef = TypedDict(
-    "_OptionalMssPackageOutputTypeDef",
-    {
-        "Encryption": MssEncryptionOutputTypeDef,
-        "SegmentDurationSeconds": int,
-    },
-    total=False,
-)
-
-class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
-    pass
-
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -800,17 +645,19 @@
         "Encryption": CmafEncryptionTypeDef,
         "IncludeEncoderConfigurationInSegments": bool,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class CmafPackageTypeDef(_RequiredCmafPackageTypeDef, _OptionalCmafPackageTypeDef):
     pass
 
+
 _RequiredDashPackageTypeDef = TypedDict(
     "_RequiredDashPackageTypeDef",
     {
         "DashManifests": Sequence[DashManifestTypeDef],
     },
 )
 _OptionalDashPackageTypeDef = TypedDict(
@@ -822,17 +669,19 @@
         "PeriodTriggers": Sequence[Literal["ADS"]],
         "SegmentDurationSeconds": int,
         "SegmentTemplateFormat": SegmentTemplateFormatType,
     },
     total=False,
 )
 
+
 class DashPackageTypeDef(_RequiredDashPackageTypeDef, _OptionalDashPackageTypeDef):
     pass
 
+
 _RequiredHlsPackageTypeDef = TypedDict(
     "_RequiredHlsPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalHlsPackageTypeDef = TypedDict(
@@ -842,17 +691,19 @@
         "IncludeDvbSubtitles": bool,
         "SegmentDurationSeconds": int,
         "UseAudioRenditionGroup": bool,
     },
     total=False,
 )
 
+
 class HlsPackageTypeDef(_RequiredHlsPackageTypeDef, _OptionalHlsPackageTypeDef):
     pass
 
+
 _RequiredMssPackageTypeDef = TypedDict(
     "_RequiredMssPackageTypeDef",
     {
         "MssManifests": Sequence[MssManifestTypeDef],
     },
 )
 _OptionalMssPackageTypeDef = TypedDict(
@@ -860,94 +711,94 @@
     {
         "Encryption": MssEncryptionTypeDef,
         "SegmentDurationSeconds": int,
     },
     total=False,
 )
 
+
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
+
+_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "Id": str,
+        "PackagingGroupId": str,
+    },
+)
+_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "CmafPackage": CmafPackageTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
+        "MssPackage": MssPackageTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreatePackagingConfigurationRequestRequestTypeDef(
+    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
+    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageOutputTypeDef,
-        "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "HlsPackage": HlsPackageOutputTypeDef,
-        "Id": str,
-        "MssPackage": MssPackageOutputTypeDef,
-        "PackagingGroupId": str,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-CmafPackageUnionTypeDef = Union[CmafPackageTypeDef, CmafPackageOutputTypeDef]
-DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
-HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
-_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "Id": str,
-        "PackagingGroupId": str,
-    },
-)
-_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
-    {
         "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "HlsPackage": HlsPackageTypeDef,
+        "Id": str,
         "MssPackage": MssPackageTypeDef,
-        "Tags": Mapping[str, str],
+        "PackagingGroupId": str,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreatePackagingConfigurationRequestRequestTypeDef(
-    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
-    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-mediapackage-vod-2.5.2.post1/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackage-vod-2.5.2.post2/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

