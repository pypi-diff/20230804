# Comparing `tmp/types-aiobotocore-mediapackage-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediapackage-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackage-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackage-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-mediapackage-2.5.2.post1.tar` & `types-aiobotocore-mediapackage-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.529526 types-aiobotocore-mediapackage-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-08-02 14:52:38.525526 types-aiobotocore-mediapackage-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.529526 types-aiobotocore-mediapackage-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.525526 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18438 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30490 2023-08-02 14:43:23.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:22.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.525526 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:38.000000 types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13491 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11953 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1102 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1101 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18424 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18393 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10349 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10347 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4385 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4380 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25745 2023-08-04 13:44:32.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25722 2023-08-04 13:44:32.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13491 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/LICENSE` & `types-aiobotocore-mediapackage-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/README.md` & `types-aiobotocore-mediapackage-2.5.2.post2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-mediapackage
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MediaPackage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore mediapackage type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mediapackage"></a>
 
 # types-aiobotocore-mediapackage
 
 [![PyPI - types-aiobotocore-mediapackage](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
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
 [types-aiobotocore-mediapackage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,131 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediapackage.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `MediaPackage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/literals/).
+
 ```python
-from types_aiobotocore_mediapackage.literals import (
-    AdMarkersType,
-    AdTriggersElementType,
-    AdsOnDeliveryRestrictionsType,
-    CmafEncryptionMethodType,
-    EncryptionMethodType,
-    ListChannelsPaginatorName,
-    ListHarvestJobsPaginatorName,
-    ListOriginEndpointsPaginatorName,
-    ManifestLayoutType,
-    OriginationType,
-    PeriodTriggersElementType,
-    PlaylistTypeType,
-    PresetSpeke20AudioType,
-    PresetSpeke20VideoType,
-    ProfileType,
-    SegmentTemplateFormatType,
-    StatusType,
-    StreamOrderType,
-    UtcTimingType,
-    MediaPackageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediapackage.literals import AdMarkersType
 
 
 def check_value(value: AdMarkersType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediapackage.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaPackage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/type_defs/).
+
 ```python
-from types_aiobotocore_mediapackage.type_defs import (
-    AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
-    HlsManifestCreateOrUpdateParametersTypeDef,
-    StreamSelectionTypeDef,
-    HlsManifestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateChannelRequestRequestTypeDef,
-    S3DestinationTypeDef,
-    DeleteChannelRequestRequestTypeDef,
-    DeleteOriginEndpointRequestRequestTypeDef,
-    DescribeChannelRequestRequestTypeDef,
-    DescribeHarvestJobRequestRequestTypeDef,
-    DescribeOriginEndpointRequestRequestTypeDef,
-    EncryptionContractConfigurationTypeDef,
-    IngestEndpointTypeDef,
-    PaginatorConfigTypeDef,
-    ListChannelsRequestRequestTypeDef,
-    ListHarvestJobsRequestRequestTypeDef,
-    ListOriginEndpointsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RotateChannelCredentialsRequestRequestTypeDef,
-    RotateIngestEndpointCredentialsRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateChannelRequestRequestTypeDef,
-    ConfigureLogsRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateHarvestJobRequestRequestTypeDef,
-    CreateHarvestJobResponseTypeDef,
-    DescribeHarvestJobResponseTypeDef,
-    HarvestJobTypeDef,
-    SpekeKeyProviderOutputTypeDef,
-    SpekeKeyProviderTypeDef,
-    HlsIngestTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    ListHarvestJobsResponseTypeDef,
-    CmafEncryptionOutputTypeDef,
-    DashEncryptionOutputTypeDef,
-    HlsEncryptionOutputTypeDef,
-    MssEncryptionOutputTypeDef,
-    CmafEncryptionTypeDef,
-    DashEncryptionTypeDef,
-    HlsEncryptionTypeDef,
-    MssEncryptionTypeDef,
-    ChannelTypeDef,
-    ConfigureLogsResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    DescribeChannelResponseTypeDef,
-    RotateChannelCredentialsResponseTypeDef,
-    RotateIngestEndpointCredentialsResponseTypeDef,
-    UpdateChannelResponseTypeDef,
-    CmafPackageTypeDef,
-    DashPackageOutputTypeDef,
-    HlsPackageOutputTypeDef,
-    MssPackageOutputTypeDef,
-    CmafPackageCreateOrUpdateParametersTypeDef,
-    DashPackageTypeDef,
-    HlsPackageTypeDef,
-    MssPackageTypeDef,
-    ListChannelsResponseTypeDef,
-    CreateOriginEndpointResponseTypeDef,
-    DescribeOriginEndpointResponseTypeDef,
-    OriginEndpointTypeDef,
-    UpdateOriginEndpointResponseTypeDef,
-    DashPackageUnionTypeDef,
-    HlsPackageUnionTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
-    MssPackageUnionTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
-    ListOriginEndpointsResponseTypeDef,
-)
+from types_aiobotocore_mediapackage.type_defs import AuthorizationTypeDef
 
 
 def get_value() -> AuthorizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/setup.py` & `types-aiobotocore-mediapackage-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackage",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaPackage 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__init__.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__init__.pyi` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/__main__.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaPackage 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaPackage 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/client.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
-    DashPackageUnionTypeDef,
+    DashPackageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageUnionTypeDef,
+    HlsPackageTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageUnionTypeDef,
+    MssPackageTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
@@ -154,19 +154,19 @@
     async def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -331,19 +331,19 @@
 
     async def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/client.pyi` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 from .type_defs import (
     AuthorizationTypeDef,
     CmafPackageCreateOrUpdateParametersTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateHarvestJobResponseTypeDef,
     CreateOriginEndpointResponseTypeDef,
-    DashPackageUnionTypeDef,
+    DashPackageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     EgressAccessLogsTypeDef,
     EmptyResponseMetadataTypeDef,
-    HlsPackageUnionTypeDef,
+    HlsPackageTypeDef,
     IngressAccessLogsTypeDef,
     ListChannelsResponseTypeDef,
     ListHarvestJobsResponseTypeDef,
     ListOriginEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MssPackageUnionTypeDef,
+    MssPackageTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     S3DestinationTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateOriginEndpointResponseTypeDef,
 )
 
@@ -144,19 +144,19 @@
     async def create_origin_endpoint(
         self,
         *,
         ChannelId: str,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         Tags: Mapping[str, str] = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> CreateOriginEndpointResponseTypeDef:
         """
@@ -305,19 +305,19 @@
         """
     async def update_origin_endpoint(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         CmafPackage: CmafPackageCreateOrUpdateParametersTypeDef = ...,
-        DashPackage: DashPackageUnionTypeDef = ...,
+        DashPackage: DashPackageTypeDef = ...,
         Description: str = ...,
-        HlsPackage: HlsPackageUnionTypeDef = ...,
+        HlsPackage: HlsPackageTypeDef = ...,
         ManifestName: str = ...,
-        MssPackage: MssPackageUnionTypeDef = ...,
+        MssPackage: MssPackageTypeDef = ...,
         Origination: OriginationType = ...,
         StartoverWindowSeconds: int = ...,
         TimeDelaySeconds: int = ...,
         Whitelist: Sequence[str] = ...
     ) -> UpdateOriginEndpointResponseTypeDef:
         """
         Updates an existing OriginEndpoint.
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/literals.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
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
@@ -205,14 +206,15 @@
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
@@ -291,26 +293,28 @@
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
@@ -457,14 +461,15 @@
 PaginatorName = Literal["list_channels", "list_harvest_jobs", "list_origin_endpoints"]
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

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/literals.pyi` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -203,14 +204,15 @@
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
@@ -289,26 +291,28 @@
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
@@ -455,14 +459,15 @@
 PaginatorName = Literal["list_channels", "list_harvest_jobs", "list_origin_endpoints"]
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

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/paginator.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/paginator.pyi` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/type_defs.py` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mediapackage.type_defs import AuthorizationTypeDef
 
     data: AuthorizationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
     AdsOnDeliveryRestrictionsType,
     AdTriggersElementType,
     CmafEncryptionMethodType,
     EncryptionMethodType,
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
@@ -72,54 +71,43 @@
     "ConfigureLogsRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
-    "CmafEncryptionOutputTypeDef",
-    "DashEncryptionOutputTypeDef",
-    "HlsEncryptionOutputTypeDef",
-    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RotateChannelCredentialsResponseTypeDef",
     "RotateIngestEndpointCredentialsResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CmafPackageTypeDef",
-    "DashPackageOutputTypeDef",
-    "HlsPackageOutputTypeDef",
-    "MssPackageOutputTypeDef",
     "CmafPackageCreateOrUpdateParametersTypeDef",
+    "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
-    "UpdateOriginEndpointResponseTypeDef",
-    "DashPackageUnionTypeDef",
-    "HlsPackageUnionTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
-    "MssPackageUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointResponseTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
@@ -160,22 +148,20 @@
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class HlsManifestCreateOrUpdateParametersTypeDef(
     _RequiredHlsManifestCreateOrUpdateParametersTypeDef,
     _OptionalHlsManifestCreateOrUpdateParametersTypeDef,
 ):
     pass
 
-
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -200,19 +186,17 @@
         "Url": str,
         "AdTriggers": List[AdTriggersElementType],
         "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
     },
     total=False,
 )
 
-
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -231,21 +215,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
@@ -393,21 +375,19 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
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
@@ -415,21 +395,19 @@
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
     },
     total=False,
 )
 
-
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -496,39 +474,14 @@
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
-_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_RequiredSpekeKeyProviderOutputTypeDef",
-    {
-        "ResourceId": str,
-        "RoleArn": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-)
-_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_OptionalSpekeKeyProviderOutputTypeDef",
-    {
-        "CertificateArn": str,
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
         "ResourceId": str,
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -539,19 +492,17 @@
     {
         "CertificateArn": str,
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
-
 HlsIngestTypeDef = TypedDict(
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
@@ -588,89 +539,14 @@
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
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
-        "EncryptionMethod": CmafEncryptionMethodType,
-        "KeyRotationIntervalSeconds": int,
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
-_RequiredDashEncryptionOutputTypeDef = TypedDict(
-    "_RequiredDashEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalDashEncryptionOutputTypeDef = TypedDict(
-    "_OptionalDashEncryptionOutputTypeDef",
-    {
-        "KeyRotationIntervalSeconds": int,
-    },
-    total=False,
-)
-
-
-class DashEncryptionOutputTypeDef(
-    _RequiredDashEncryptionOutputTypeDef, _OptionalDashEncryptionOutputTypeDef
-):
-    pass
-
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
-        "KeyRotationIntervalSeconds": int,
-        "RepeatExtXKey": bool,
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
@@ -679,38 +555,34 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
-
 _RequiredDashEncryptionTypeDef = TypedDict(
     "_RequiredDashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalDashEncryptionTypeDef = TypedDict(
     "_OptionalDashEncryptionTypeDef",
     {
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class DashEncryptionTypeDef(_RequiredDashEncryptionTypeDef, _OptionalDashEncryptionTypeDef):
     pass
 
-
 _RequiredHlsEncryptionTypeDef = TypedDict(
     "_RequiredHlsEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalHlsEncryptionTypeDef = TypedDict(
@@ -720,19 +592,17 @@
         "EncryptionMethod": EncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
         "RepeatExtXKey": bool,
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
 
@@ -837,84 +707,31 @@
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CmafPackageTypeDef = TypedDict(
-    "CmafPackageTypeDef",
+CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     {
-        "Encryption": CmafEncryptionOutputTypeDef,
-        "HlsManifests": List[HlsManifestTypeDef],
+        "Encryption": CmafEncryptionTypeDef,
+        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
-DashPackageOutputTypeDef = TypedDict(
-    "DashPackageOutputTypeDef",
-    {
-        "AdTriggers": List[AdTriggersElementType],
-        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
-        "Encryption": DashEncryptionOutputTypeDef,
-        "IncludeIframeOnlyStream": bool,
-        "ManifestLayout": ManifestLayoutType,
-        "ManifestWindowSeconds": int,
-        "MinBufferTimeSeconds": int,
-        "MinUpdatePeriodSeconds": int,
-        "PeriodTriggers": List[Literal["ADS"]],
-        "Profile": ProfileType,
-        "SegmentDurationSeconds": int,
-        "SegmentTemplateFormat": SegmentTemplateFormatType,
-        "StreamSelection": StreamSelectionTypeDef,
-        "SuggestedPresentationDelaySeconds": int,
-        "UtcTiming": UtcTimingType,
-        "UtcTimingUri": str,
-    },
-    total=False,
-)
-
-HlsPackageOutputTypeDef = TypedDict(
-    "HlsPackageOutputTypeDef",
-    {
-        "AdMarkers": AdMarkersType,
-        "AdTriggers": List[AdTriggersElementType],
-        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
-        "Encryption": HlsEncryptionOutputTypeDef,
-        "IncludeDvbSubtitles": bool,
-        "IncludeIframeOnlyStream": bool,
-        "PlaylistType": PlaylistTypeType,
-        "PlaylistWindowSeconds": int,
-        "ProgramDateTimeIntervalSeconds": int,
-        "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionTypeDef,
-        "UseAudioRenditionGroup": bool,
-    },
-    total=False,
-)
-
-MssPackageOutputTypeDef = TypedDict(
-    "MssPackageOutputTypeDef",
-    {
-        "Encryption": MssEncryptionOutputTypeDef,
-        "ManifestWindowSeconds": int,
-        "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionTypeDef,
-    },
-    total=False,
-)
-
-CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
-    "CmafPackageCreateOrUpdateParametersTypeDef",
+CmafPackageTypeDef = TypedDict(
+    "CmafPackageTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
@@ -976,179 +793,172 @@
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
-        "CmafPackage": CmafPackageTypeDef,
-        "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
+    },
+)
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+    {
+        "Authorization": AuthorizationTypeDef,
+        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "Description": str,
+        "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Dict[str, str],
+        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
-        "Url": str,
-        "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Whitelist": Sequence[str],
     },
+    total=False,
 )
 
-DescribeOriginEndpointResponseTypeDef = TypedDict(
-    "DescribeOriginEndpointResponseTypeDef",
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
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OriginEndpointTypeDef = TypedDict(
-    "OriginEndpointTypeDef",
+DescribeOriginEndpointResponseTypeDef = TypedDict(
+    "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+OriginEndpointTypeDef = TypedDict(
+    "OriginEndpointTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
-HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "ChannelId": str,
         "Id": str,
     },
 )
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
         "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
         "Whitelist": Sequence[str],
     },
     total=False,
 )
 
-
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-
-MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "Authorization": AuthorizationTypeDef,
-        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
+        "ChannelId": str,
+        "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
+        "Id": str,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
+        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Whitelist": Sequence[str],
+        "Url": str,
+        "Whitelist": List[str],
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
-
-
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage/type_defs.pyi` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mediapackage.type_defs import AuthorizationTypeDef
 
     data: AuthorizationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
     AdsOnDeliveryRestrictionsType,
     AdTriggersElementType,
     CmafEncryptionMethodType,
     EncryptionMethodType,
@@ -37,14 +37,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "IngressAccessLogsTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
@@ -71,54 +72,43 @@
     "ConfigureLogsRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListHarvestJobsResponseTypeDef",
-    "CmafEncryptionOutputTypeDef",
-    "DashEncryptionOutputTypeDef",
-    "HlsEncryptionOutputTypeDef",
-    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RotateChannelCredentialsResponseTypeDef",
     "RotateIngestEndpointCredentialsResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CmafPackageTypeDef",
-    "DashPackageOutputTypeDef",
-    "HlsPackageOutputTypeDef",
-    "MssPackageOutputTypeDef",
     "CmafPackageCreateOrUpdateParametersTypeDef",
+    "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
-    "UpdateOriginEndpointResponseTypeDef",
-    "DashPackageUnionTypeDef",
-    "HlsPackageUnionTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
-    "MssPackageUnionTypeDef",
     "UpdateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointResponseTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
@@ -159,20 +149,22 @@
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class HlsManifestCreateOrUpdateParametersTypeDef(
     _RequiredHlsManifestCreateOrUpdateParametersTypeDef,
     _OptionalHlsManifestCreateOrUpdateParametersTypeDef,
 ):
     pass
 
+
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -197,17 +189,19 @@
         "Url": str,
         "AdTriggers": List[AdTriggersElementType],
         "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
     },
     total=False,
 )
 
+
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -226,19 +220,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
@@ -386,19 +382,21 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
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
@@ -406,19 +404,21 @@
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
     },
     total=False,
 )
 
+
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -485,37 +485,14 @@
         "S3Destination": S3DestinationTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
-_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_RequiredSpekeKeyProviderOutputTypeDef",
-    {
-        "ResourceId": str,
-        "RoleArn": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-)
-_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
-    "_OptionalSpekeKeyProviderOutputTypeDef",
-    {
-        "CertificateArn": str,
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
         "ResourceId": str,
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -526,17 +503,19 @@
     {
         "CertificateArn": str,
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
+
 HlsIngestTypeDef = TypedDict(
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
@@ -573,83 +552,14 @@
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
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
-        "EncryptionMethod": CmafEncryptionMethodType,
-        "KeyRotationIntervalSeconds": int,
-    },
-    total=False,
-)
-
-class CmafEncryptionOutputTypeDef(
-    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
-):
-    pass
-
-_RequiredDashEncryptionOutputTypeDef = TypedDict(
-    "_RequiredDashEncryptionOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-)
-_OptionalDashEncryptionOutputTypeDef = TypedDict(
-    "_OptionalDashEncryptionOutputTypeDef",
-    {
-        "KeyRotationIntervalSeconds": int,
-    },
-    total=False,
-)
-
-class DashEncryptionOutputTypeDef(
-    _RequiredDashEncryptionOutputTypeDef, _OptionalDashEncryptionOutputTypeDef
-):
-    pass
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
-        "KeyRotationIntervalSeconds": int,
-        "RepeatExtXKey": bool,
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
@@ -658,34 +568,38 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
+
 _RequiredDashEncryptionTypeDef = TypedDict(
     "_RequiredDashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalDashEncryptionTypeDef = TypedDict(
     "_OptionalDashEncryptionTypeDef",
     {
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class DashEncryptionTypeDef(_RequiredDashEncryptionTypeDef, _OptionalDashEncryptionTypeDef):
     pass
 
+
 _RequiredHlsEncryptionTypeDef = TypedDict(
     "_RequiredHlsEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalHlsEncryptionTypeDef = TypedDict(
@@ -695,17 +609,19 @@
         "EncryptionMethod": EncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
         "RepeatExtXKey": bool,
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
 
@@ -810,84 +726,31 @@
         "Id": str,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CmafPackageTypeDef = TypedDict(
-    "CmafPackageTypeDef",
+CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     {
-        "Encryption": CmafEncryptionOutputTypeDef,
-        "HlsManifests": List[HlsManifestTypeDef],
+        "Encryption": CmafEncryptionTypeDef,
+        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
-DashPackageOutputTypeDef = TypedDict(
-    "DashPackageOutputTypeDef",
-    {
-        "AdTriggers": List[AdTriggersElementType],
-        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
-        "Encryption": DashEncryptionOutputTypeDef,
-        "IncludeIframeOnlyStream": bool,
-        "ManifestLayout": ManifestLayoutType,
-        "ManifestWindowSeconds": int,
-        "MinBufferTimeSeconds": int,
-        "MinUpdatePeriodSeconds": int,
-        "PeriodTriggers": List[Literal["ADS"]],
-        "Profile": ProfileType,
-        "SegmentDurationSeconds": int,
-        "SegmentTemplateFormat": SegmentTemplateFormatType,
-        "StreamSelection": StreamSelectionTypeDef,
-        "SuggestedPresentationDelaySeconds": int,
-        "UtcTiming": UtcTimingType,
-        "UtcTimingUri": str,
-    },
-    total=False,
-)
-
-HlsPackageOutputTypeDef = TypedDict(
-    "HlsPackageOutputTypeDef",
-    {
-        "AdMarkers": AdMarkersType,
-        "AdTriggers": List[AdTriggersElementType],
-        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
-        "Encryption": HlsEncryptionOutputTypeDef,
-        "IncludeDvbSubtitles": bool,
-        "IncludeIframeOnlyStream": bool,
-        "PlaylistType": PlaylistTypeType,
-        "PlaylistWindowSeconds": int,
-        "ProgramDateTimeIntervalSeconds": int,
-        "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionTypeDef,
-        "UseAudioRenditionGroup": bool,
-    },
-    total=False,
-)
-
-MssPackageOutputTypeDef = TypedDict(
-    "MssPackageOutputTypeDef",
-    {
-        "Encryption": MssEncryptionOutputTypeDef,
-        "ManifestWindowSeconds": int,
-        "SegmentDurationSeconds": int,
-        "StreamSelection": StreamSelectionTypeDef,
-    },
-    total=False,
-)
-
-CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
-    "CmafPackageCreateOrUpdateParametersTypeDef",
+CmafPackageTypeDef = TypedDict(
+    "CmafPackageTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
+        "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
@@ -949,175 +812,176 @@
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
-        "CmafPackage": CmafPackageTypeDef,
-        "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
-        "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
+    },
+)
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+    {
+        "Authorization": AuthorizationTypeDef,
+        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "Description": str,
+        "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Dict[str, str],
+        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
-        "Url": str,
-        "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Whitelist": Sequence[str],
     },
+    total=False,
 )
 
-DescribeOriginEndpointResponseTypeDef = TypedDict(
-    "DescribeOriginEndpointResponseTypeDef",
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
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OriginEndpointTypeDef = TypedDict(
-    "OriginEndpointTypeDef",
+DescribeOriginEndpointResponseTypeDef = TypedDict(
+    "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+OriginEndpointTypeDef = TypedDict(
+    "OriginEndpointTypeDef",
     {
         "Arn": str,
         "Authorization": AuthorizationTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageOutputTypeDef,
+        "DashPackage": DashPackageTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageOutputTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageOutputTypeDef,
+        "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DashPackageUnionTypeDef = Union[DashPackageTypeDef, DashPackageOutputTypeDef]
-HlsPackageUnionTypeDef = Union[HlsPackageTypeDef, HlsPackageOutputTypeDef]
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "ChannelId": str,
         "Id": str,
     },
 )
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
         "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
         "Whitelist": Sequence[str],
     },
     total=False,
 )
 
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
+
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-MssPackageUnionTypeDef = Union[MssPackageTypeDef, MssPackageOutputTypeDef]
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "Authorization": AuthorizationTypeDef,
-        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
+        "ChannelId": str,
+        "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
+        "Id": str,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
+        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Whitelist": Sequence[str],
+        "Url": str,
+        "Whitelist": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
-):
-    pass
-
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post1/types_aiobotocore_mediapackage.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

