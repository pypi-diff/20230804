# Comparing `tmp/types-aiobotocore-kinesisvideo-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesisvideo-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1.tar` & `types-aiobotocore-kinesisvideo-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26216 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.406643 types-aiobotocore-kinesisvideo-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13795 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12257 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.406643 types-aiobotocore-kinesisvideo-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1519 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1518 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26786 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26743 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10404 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10402 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6098 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6092 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28618 2023-08-04 13:42:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28579 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13795 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesisvideo-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,154 +273,67 @@
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_kinesisvideo import KinesisVideoClient
 from types_aiobotocore_kinesisvideo.paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 session = get_session()
 async with session.create_client("kinesisvideo") as client:
     client: KinesisVideoClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator(
         "describe_mapped_resource_configuration"
     )
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = (
+        client.get_paginator("list_edge_agent_configurations")
+    )
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
         "list_signaling_channels"
     )
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesisvideo.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideo` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/literals/).
+
 ```python
-from types_aiobotocore_kinesisvideo.literals import (
-    APINameType,
-    ChannelProtocolType,
-    ChannelRoleType,
-    ChannelTypeType,
-    ComparisonOperatorType,
-    ConfigurationStatusType,
-    DescribeMappedResourceConfigurationPaginatorName,
-    FormatConfigKeyType,
-    FormatType,
-    ImageSelectorTypeType,
-    ListSignalingChannelsPaginatorName,
-    ListStreamsPaginatorName,
-    MediaStorageConfigurationStatusType,
-    MediaUriTypeType,
-    StatusType,
-    StrategyOnFullSizeType,
-    SyncStatusType,
-    UpdateDataRetentionOperationType,
-    KinesisVideoServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kinesisvideo.literals import APINameType
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesisvideo.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KinesisVideo` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/type_defs/).
+
 ```python
-from types_aiobotocore_kinesisvideo.type_defs import (
-    SingleMasterConfigurationTypeDef,
-    ChannelNameConditionTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateStreamInputRequestTypeDef,
-    DeleteSignalingChannelInputRequestTypeDef,
-    DeleteStreamInputRequestTypeDef,
-    LocalSizeConfigTypeDef,
-    DescribeEdgeConfigurationInputRequestTypeDef,
-    DescribeImageGenerationConfigurationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeMappedResourceConfigurationInputRequestTypeDef,
-    MappedResourceConfigurationListItemTypeDef,
-    DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationTypeDef,
-    DescribeNotificationConfigurationInputRequestTypeDef,
-    DescribeSignalingChannelInputRequestTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    StreamInfoTypeDef,
-    GetDataEndpointInputRequestTypeDef,
-    SingleMasterChannelEndpointConfigurationTypeDef,
-    ResourceEndpointListItemTypeDef,
-    ImageGenerationDestinationConfigTypeDef,
-    StreamNameConditionTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListTagsForStreamInputRequestTypeDef,
-    MediaSourceConfigTypeDef,
-    NotificationDestinationConfigTypeDef,
-    ScheduleConfigTypeDef,
-    TagStreamInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UntagStreamInputRequestTypeDef,
-    UpdateDataRetentionInputRequestTypeDef,
-    UpdateStreamInputRequestTypeDef,
-    ChannelInfoTypeDef,
-    UpdateSignalingChannelInputRequestTypeDef,
-    ListSignalingChannelsInputRequestTypeDef,
-    CreateSignalingChannelInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateSignalingChannelOutputTypeDef,
-    CreateStreamOutputTypeDef,
-    GetDataEndpointOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    DeletionConfigTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
-    DescribeMappedResourceConfigurationOutputTypeDef,
-    DescribeMediaStorageConfigurationOutputTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
-    DescribeStreamOutputTypeDef,
-    ListStreamsOutputTypeDef,
-    GetSignalingChannelEndpointInputRequestTypeDef,
-    GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
-    ListStreamsInputRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    RecorderConfigTypeDef,
-    UploaderConfigTypeDef,
-    DescribeSignalingChannelOutputTypeDef,
-    ListSignalingChannelsOutputTypeDef,
-    DescribeImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
-    UpdateImageGenerationConfigurationInputRequestTypeDef,
-    DescribeNotificationConfigurationOutputTypeDef,
-    UpdateNotificationConfigurationInputRequestTypeDef,
-    EdgeConfigTypeDef,
-    DescribeEdgeConfigurationOutputTypeDef,
-    StartEdgeConfigurationUpdateInputRequestTypeDef,
-    StartEdgeConfigurationUpdateOutputTypeDef,
-)
+from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
 
 def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/README.md` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-kinesisvideo
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore kinesisvideo type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -241,154 +273,67 @@
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_kinesisvideo import KinesisVideoClient
 from types_aiobotocore_kinesisvideo.paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 session = get_session()
 async with session.create_client("kinesisvideo") as client:
     client: KinesisVideoClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator(
         "describe_mapped_resource_configuration"
     )
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = (
+        client.get_paginator("list_edge_agent_configurations")
+    )
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
         "list_signaling_channels"
     )
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesisvideo.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideo` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/literals/).
+
 ```python
-from types_aiobotocore_kinesisvideo.literals import (
-    APINameType,
-    ChannelProtocolType,
-    ChannelRoleType,
-    ChannelTypeType,
-    ComparisonOperatorType,
-    ConfigurationStatusType,
-    DescribeMappedResourceConfigurationPaginatorName,
-    FormatConfigKeyType,
-    FormatType,
-    ImageSelectorTypeType,
-    ListSignalingChannelsPaginatorName,
-    ListStreamsPaginatorName,
-    MediaStorageConfigurationStatusType,
-    MediaUriTypeType,
-    StatusType,
-    StrategyOnFullSizeType,
-    SyncStatusType,
-    UpdateDataRetentionOperationType,
-    KinesisVideoServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_kinesisvideo.literals import APINameType
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesisvideo.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KinesisVideo` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/type_defs/).
+
 ```python
-from types_aiobotocore_kinesisvideo.type_defs import (
-    SingleMasterConfigurationTypeDef,
-    ChannelNameConditionTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateStreamInputRequestTypeDef,
-    DeleteSignalingChannelInputRequestTypeDef,
-    DeleteStreamInputRequestTypeDef,
-    LocalSizeConfigTypeDef,
-    DescribeEdgeConfigurationInputRequestTypeDef,
-    DescribeImageGenerationConfigurationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeMappedResourceConfigurationInputRequestTypeDef,
-    MappedResourceConfigurationListItemTypeDef,
-    DescribeMediaStorageConfigurationInputRequestTypeDef,
-    MediaStorageConfigurationTypeDef,
-    DescribeNotificationConfigurationInputRequestTypeDef,
-    DescribeSignalingChannelInputRequestTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    StreamInfoTypeDef,
-    GetDataEndpointInputRequestTypeDef,
-    SingleMasterChannelEndpointConfigurationTypeDef,
-    ResourceEndpointListItemTypeDef,
-    ImageGenerationDestinationConfigTypeDef,
-    StreamNameConditionTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListTagsForStreamInputRequestTypeDef,
-    MediaSourceConfigTypeDef,
-    NotificationDestinationConfigTypeDef,
-    ScheduleConfigTypeDef,
-    TagStreamInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UntagStreamInputRequestTypeDef,
-    UpdateDataRetentionInputRequestTypeDef,
-    UpdateStreamInputRequestTypeDef,
-    ChannelInfoTypeDef,
-    UpdateSignalingChannelInputRequestTypeDef,
-    ListSignalingChannelsInputRequestTypeDef,
-    CreateSignalingChannelInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateSignalingChannelOutputTypeDef,
-    CreateStreamOutputTypeDef,
-    GetDataEndpointOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTagsForStreamOutputTypeDef,
-    DeletionConfigTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
-    DescribeMappedResourceConfigurationOutputTypeDef,
-    DescribeMediaStorageConfigurationOutputTypeDef,
-    UpdateMediaStorageConfigurationInputRequestTypeDef,
-    DescribeStreamOutputTypeDef,
-    ListStreamsOutputTypeDef,
-    GetSignalingChannelEndpointInputRequestTypeDef,
-    GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
-    ListStreamsInputListStreamsPaginateTypeDef,
-    ListStreamsInputRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    RecorderConfigTypeDef,
-    UploaderConfigTypeDef,
-    DescribeSignalingChannelOutputTypeDef,
-    ListSignalingChannelsOutputTypeDef,
-    DescribeImageGenerationConfigurationOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
-    UpdateImageGenerationConfigurationInputRequestTypeDef,
-    DescribeNotificationConfigurationOutputTypeDef,
-    UpdateNotificationConfigurationInputRequestTypeDef,
-    EdgeConfigTypeDef,
-    DescribeEdgeConfigurationOutputTypeDef,
-    StartEdgeConfigurationUpdateInputRequestTypeDef,
-    StartEdgeConfigurationUpdateOutputTypeDef,
-)
+from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
 
 def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/setup.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisvideo",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_kinesisvideo import (
         Client,
         DescribeMappedResourceConfigurationPaginator,
         KinesisVideoClient,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = get_session()
     async with session.create_client("kinesisvideo") as client:
         client: KinesisVideoClient
         ...
 
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from .client import KinesisVideoClient
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 Client = KinesisVideoClient
 
 
 __all__ = (
     "Client",
     "DescribeMappedResourceConfigurationPaginator",
     "KinesisVideoClient",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,42 @@
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_kinesisvideo import (
         Client,
         DescribeMappedResourceConfigurationPaginator,
         KinesisVideoClient,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = get_session()
     async with session.create_client("kinesisvideo") as client:
         client: KinesisVideoClient
         ...
 
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from .client import KinesisVideoClient
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 Client = KinesisVideoClient
 
 __all__ = (
     "Client",
     "DescribeMappedResourceConfigurationPaginator",
     "KinesisVideoClient",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__main__.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideo 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideo 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
@@ -36,15 +37,16 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
+    ImageGenerationConfigurationTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -151,14 +153,25 @@
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_stream)
         """
 
+    async def delete_edge_configuration(
+        self, *, StreamName: str = ..., StreamARN: str = ...
+    ) -> Dict[str, Any]:
+        """
+        An asynchronous API that deletes a stream’s existing edge configuration, as well
+        as the corresponding media from the Edge Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_edge_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#delete_edge_configuration)
+        """
+
     async def delete_signaling_channel(
         self, *, ChannelARN: str, CurrentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_signaling_channel)
@@ -174,15 +187,16 @@
         """
 
     async def describe_edge_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeEdgeConfigurationOutputTypeDef:
         """
         Describes a stream’s edge configuration that was set using the
-        `StartEdgeConfigurationUpdate` API.
+        `StartEdgeConfigurationUpdate` API and the latest status of the edge agent's
+        recorder and uploader jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_edge_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#describe_edge_configuration)
         """
 
     async def describe_image_generation_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
@@ -283,14 +297,25 @@
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_signaling_channel_endpoint)
         """
 
+    async def list_edge_agent_configurations(
+        self, *, HubDeviceArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListEdgeAgentConfigurationsOutputTypeDef:
+        """
+        Returns an array of edge configurations associated with the specified Edge
+        Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_edge_agent_configurations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_edge_agent_configurations)
+        """
+
     async def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...
     ) -> ListSignalingChannelsOutputTypeDef:
@@ -401,15 +426,15 @@
         """
 
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
@@ -475,14 +500,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_edge_agent_configurations"]
+    ) -> ListEdgeAgentConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
@@ -36,15 +37,16 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
+    ImageGenerationConfigurationTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -142,14 +144,24 @@
     ) -> CreateStreamOutputTypeDef:
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#create_stream)
         """
+    async def delete_edge_configuration(
+        self, *, StreamName: str = ..., StreamARN: str = ...
+    ) -> Dict[str, Any]:
+        """
+        An asynchronous API that deletes a stream’s existing edge configuration, as well
+        as the corresponding media from the Edge Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_edge_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#delete_edge_configuration)
+        """
     async def delete_signaling_channel(
         self, *, ChannelARN: str, CurrentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_signaling_channel)
@@ -163,15 +175,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#delete_stream)
         """
     async def describe_edge_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeEdgeConfigurationOutputTypeDef:
         """
         Describes a stream’s edge configuration that was set using the
-        `StartEdgeConfigurationUpdate` API.
+        `StartEdgeConfigurationUpdate` API and the latest status of the edge agent's
+        recorder and uploader jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_edge_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#describe_edge_configuration)
         """
     async def describe_image_generation_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeImageGenerationConfigurationOutputTypeDef:
@@ -262,14 +275,24 @@
         """
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_signaling_channel_endpoint)
         """
+    async def list_edge_agent_configurations(
+        self, *, HubDeviceArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListEdgeAgentConfigurationsOutputTypeDef:
+        """
+        Returns an array of edge configurations associated with the specified Edge
+        Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_edge_agent_configurations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#list_edge_agent_configurations)
+        """
     async def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...
     ) -> ListSignalingChannelsOutputTypeDef:
@@ -370,15 +393,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_data_retention)
         """
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
@@ -438,14 +461,22 @@
     ) -> DescribeMappedResourceConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_edge_agent_configurations"]
+    ) -> ListEdgeAgentConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#get_paginator)
         """
     @overload
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,25 @@
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
     "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
+    "ListEdgeAgentConfigurationsPaginatorName",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
     "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
+    "RecorderStatusType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
+    "UploaderStatusType",
     "KinesisVideoServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -61,24 +64,33 @@
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
+ListEdgeAgentConfigurationsPaginatorName = Literal["list_edge_agent_configurations"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
+RecorderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
-    "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
+    "ACKNOWLEDGED",
+    "DELETE_FAILED",
+    "DELETING",
+    "DELETING_ACKNOWLEDGED",
+    "IN_SYNC",
+    "SYNCING",
+    "SYNC_FAILED",
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
+UploaderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 KinesisVideoServiceName = Literal["kinesisvideo"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -87,14 +99,15 @@
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
@@ -190,14 +203,15 @@
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
@@ -276,26 +290,28 @@
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
@@ -436,15 +452,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+    "describe_mapped_resource_configuration",
+    "list_edge_agent_configurations",
+    "list_signaling_channels",
+    "list_streams",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,25 @@
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
     "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
+    "ListEdgeAgentConfigurationsPaginatorName",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
     "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
+    "RecorderStatusType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
+    "UploaderStatusType",
     "KinesisVideoServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -59,24 +62,33 @@
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
+ListEdgeAgentConfigurationsPaginatorName = Literal["list_edge_agent_configurations"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
+RecorderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
-    "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
+    "ACKNOWLEDGED",
+    "DELETE_FAILED",
+    "DELETING",
+    "DELETING_ACKNOWLEDGED",
+    "IN_SYNC",
+    "SYNCING",
+    "SYNC_FAILED",
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
+UploaderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 KinesisVideoServiceName = Literal["kinesisvideo"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -85,14 +97,15 @@
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
@@ -188,14 +201,15 @@
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
@@ -274,26 +288,28 @@
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
@@ -434,15 +450,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+    "describe_mapped_resource_configuration",
+    "list_edge_agent_configurations",
+    "list_signaling_channels",
+    "list_streams",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,43 +7,47 @@
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
     from types_aiobotocore_kinesisvideo.paginator import (
         DescribeMappedResourceConfigurationPaginator,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = get_session()
     with session.create_client("kinesisvideo") as client:
         client: KinesisVideoClient
 
         describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+        list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
         list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
         list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ChannelNameConditionTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
 )
 
 __all__ = (
     "DescribeMappedResourceConfigurationPaginator",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -70,14 +74,29 @@
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 
+class ListEdgeAgentConfigurationsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, HubDeviceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+        """
+
+
 class ListSignalingChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -7,43 +7,47 @@
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
     from types_aiobotocore_kinesisvideo.paginator import (
         DescribeMappedResourceConfigurationPaginator,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = get_session()
     with session.create_client("kinesisvideo") as client:
         client: KinesisVideoClient
 
         describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+        list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
         list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
         list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ChannelNameConditionTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
 )
 
 __all__ = (
     "DescribeMappedResourceConfigurationPaginator",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -66,14 +70,28 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
+class ListEdgeAgentConfigurationsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, HubDeviceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+        """
+
 class ListSignalingChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.py` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,32 @@
     from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
     data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -43,32 +45,36 @@
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
+    "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
+    "LastRecorderStatusTypeDef",
+    "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
+    "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
     "ScheduleConfigTypeDef",
     "TagStreamInputRequestTypeDef",
@@ -84,40 +90,42 @@
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamOutputTypeDef",
     "GetDataEndpointOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
     "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
+    "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
-    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
-    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
 SingleMasterConfigurationTypeDef = TypedDict(
     "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
@@ -173,14 +181,23 @@
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
 
+DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
+    "DeleteEdgeConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -346,14 +363,36 @@
         "Status": StatusType,
         "CreationTime": datetime,
         "DataRetentionInHours": int,
     },
     total=False,
 )
 
+LastRecorderStatusTypeDef = TypedDict(
+    "LastRecorderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RecorderStatus": RecorderStatusType,
+    },
+    total=False,
+)
+
+LastUploaderStatusTypeDef = TypedDict(
+    "LastUploaderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "UploaderStatus": UploaderStatusType,
+    },
+    total=False,
+)
+
 _RequiredGetDataEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetDataEndpointInputRequestTypeDef",
     {
         "APIName": APINameType,
     },
 )
 _OptionalGetDataEndpointInputRequestTypeDef = TypedDict(
@@ -394,14 +433,37 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
+_RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListEdgeAgentConfigurationsInputRequestTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
+):
+    pass
+
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -698,14 +760,36 @@
         "StreamName": str,
         "StreamARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
+
 ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     {
         "ChannelNameCondition": ChannelNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -749,14 +833,23 @@
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EdgeAgentStatusTypeDef = TypedDict(
+    "EdgeAgentStatusTypeDef",
+    {
+        "LastRecorderStatus": LastRecorderStatusTypeDef,
+        "LastUploaderStatus": LastUploaderStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
@@ -779,56 +872,28 @@
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredImageGenerationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalImageGenerationConfigurationOutputTypeDef",
-    {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-    },
-    total=False,
-)
-
-
-class ImageGenerationConfigurationOutputTypeDef(
-    _RequiredImageGenerationConfigurationOutputTypeDef,
-    _OptionalImageGenerationConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
 
@@ -907,22 +972,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageGenerationConfigurationUnionTypeDef = Union[
-    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
@@ -974,18 +1036,33 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeAgentStatus": EdgeAgentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -1014,7 +1091,16 @@
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsOutputTypeDef",
+    {
+        "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -9,30 +9,32 @@
     from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
     data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -42,32 +44,36 @@
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
+    "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
+    "LastRecorderStatusTypeDef",
+    "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
+    "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
     "ScheduleConfigTypeDef",
     "TagStreamInputRequestTypeDef",
@@ -83,40 +89,42 @@
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamOutputTypeDef",
     "GetDataEndpointOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
     "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
+    "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
-    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
-    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
 SingleMasterConfigurationTypeDef = TypedDict(
     "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
@@ -170,14 +178,23 @@
 )
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
+DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
+    "DeleteEdgeConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -337,14 +354,36 @@
         "Status": StatusType,
         "CreationTime": datetime,
         "DataRetentionInHours": int,
     },
     total=False,
 )
 
+LastRecorderStatusTypeDef = TypedDict(
+    "LastRecorderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RecorderStatus": RecorderStatusType,
+    },
+    total=False,
+)
+
+LastUploaderStatusTypeDef = TypedDict(
+    "LastUploaderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "UploaderStatus": UploaderStatusType,
+    },
+    total=False,
+)
+
 _RequiredGetDataEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetDataEndpointInputRequestTypeDef",
     {
         "APIName": APINameType,
     },
 )
 _OptionalGetDataEndpointInputRequestTypeDef = TypedDict(
@@ -383,14 +422,35 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
+_RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListEdgeAgentConfigurationsInputRequestTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
+):
+    pass
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -673,14 +733,34 @@
         "StreamName": str,
         "StreamARN": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
 ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     {
         "ChannelNameCondition": ChannelNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -724,14 +804,23 @@
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EdgeAgentStatusTypeDef = TypedDict(
+    "EdgeAgentStatusTypeDef",
+    {
+        "LastRecorderStatus": LastRecorderStatusTypeDef,
+        "LastUploaderStatus": LastUploaderStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
@@ -752,54 +841,28 @@
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredImageGenerationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalImageGenerationConfigurationOutputTypeDef",
-    {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-    },
-    total=False,
-)
-
-class ImageGenerationConfigurationOutputTypeDef(
-    _RequiredImageGenerationConfigurationOutputTypeDef,
-    _OptionalImageGenerationConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
 class ImageGenerationConfigurationTypeDef(
@@ -874,22 +937,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageGenerationConfigurationUnionTypeDef = Union[
-    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
@@ -939,18 +999,33 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
+        "EdgeAgentStatus": EdgeAgentStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -977,7 +1052,16 @@
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsOutputTypeDef",
+    {
+        "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

