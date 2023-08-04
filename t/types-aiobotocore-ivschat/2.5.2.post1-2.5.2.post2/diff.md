# Comparing `tmp/types-aiobotocore-ivschat-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ivschat-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivschat-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivschat-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-ivschat-2.5.2.post1.tar` & `types-aiobotocore-ivschat-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.009555 types-aiobotocore-ivschat-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-02 14:52:29.005555 types-aiobotocore-ivschat-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:29.009555 types-aiobotocore-ivschat-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.001555 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14863 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-08-02 14:41:12.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:11.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:29.005555 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:28.000000 types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.356643 types-aiobotocore-ivschat-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12246 2023-08-04 13:59:13.356643 types-aiobotocore-ivschat-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10728 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.356643 types-aiobotocore-ivschat-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.356643 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      442 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      441 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14863 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14838 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8375 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8373 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14339 2023-08-04 13:41:36.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14324 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:35.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.356643 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12246 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      734 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:13.000000 types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/LICENSE` & `types-aiobotocore-ivschat-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ivschat-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivschat
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ivschat 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ivschat 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,80 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivschat.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ivschat` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/literals/).
+
 ```python
-from types_aiobotocore_ivschat.literals import (
-    ChatTokenCapabilityType,
-    CreateLoggingConfigurationStateType,
-    FallbackResultType,
-    LoggingConfigurationStateType,
-    UpdateLoggingConfigurationStateType,
-    ivschatServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivschat.literals import ChatTokenCapabilityType
 
 
 def check_value(value: ChatTokenCapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivschat.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivschat` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/type_defs/).
+
 ```python
-from types_aiobotocore_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationTypeDef,
-    CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    MessageReviewHandlerTypeDef,
-    DeleteLoggingConfigurationRequestRequestTypeDef,
-    DeleteMessageRequestRequestTypeDef,
-    DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
-    DisconnectUserRequestRequestTypeDef,
-    GetLoggingConfigurationRequestRequestTypeDef,
-    GetRoomRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRoomsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SendEventRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
-    CreateRoomRequestRequestTypeDef,
-    CreateRoomResponseTypeDef,
-    GetRoomResponseTypeDef,
-    RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
-    UpdateRoomResponseTypeDef,
-    DestinationConfigurationTypeDef,
-    ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
-    CreateLoggingConfigurationResponseTypeDef,
-    GetLoggingConfigurationResponseTypeDef,
-    LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    ListLoggingConfigurationsResponseTypeDef,
-)
+from types_aiobotocore_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
 
 
 def get_value() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/README.md` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ivschat
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ivschat 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ivschat type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ivschat"></a>
 
 # types-aiobotocore-ivschat
 
 [![PyPI - types-aiobotocore-ivschat](https://img.shields.io/pypi/v/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/)
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -233,80 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivschat.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ivschat` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/literals/).
+
 ```python
-from types_aiobotocore_ivschat.literals import (
-    ChatTokenCapabilityType,
-    CreateLoggingConfigurationStateType,
-    FallbackResultType,
-    LoggingConfigurationStateType,
-    UpdateLoggingConfigurationStateType,
-    ivschatServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivschat.literals import ChatTokenCapabilityType
 
 
 def check_value(value: ChatTokenCapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivschat.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivschat` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/type_defs/).
+
 ```python
-from types_aiobotocore_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationTypeDef,
-    CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    MessageReviewHandlerTypeDef,
-    DeleteLoggingConfigurationRequestRequestTypeDef,
-    DeleteMessageRequestRequestTypeDef,
-    DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
-    DisconnectUserRequestRequestTypeDef,
-    GetLoggingConfigurationRequestRequestTypeDef,
-    GetRoomRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRoomsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SendEventRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
-    CreateRoomRequestRequestTypeDef,
-    CreateRoomResponseTypeDef,
-    GetRoomResponseTypeDef,
-    RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
-    UpdateRoomResponseTypeDef,
-    DestinationConfigurationTypeDef,
-    ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
-    CreateLoggingConfigurationResponseTypeDef,
-    GetLoggingConfigurationResponseTypeDef,
-    LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    ListLoggingConfigurationsResponseTypeDef,
-)
+from types_aiobotocore_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
 
 
 def get_value() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/setup.py` & `types-aiobotocore-ivschat-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivschat",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ivschat 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/__main__.py` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ivschat 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ivschat 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
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

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/client.py` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/client.pyi` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/literals.py` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChatTokenCapabilityType",
     "CreateLoggingConfigurationStateType",
     "FallbackResultType",
     "LoggingConfigurationStateType",
     "UpdateLoggingConfigurationStateType",
     "ivschatServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChatTokenCapabilityType = Literal["DELETE_MESSAGE", "DISCONNECT_USER", "SEND_MESSAGE"]
 CreateLoggingConfigurationStateType = Literal["ACTIVE"]
 FallbackResultType = Literal["ALLOW", "DENY"]
 LoggingConfigurationStateType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 UpdateLoggingConfigurationStateType = Literal["ACTIVE"]
@@ -51,14 +49,15 @@
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
@@ -154,14 +153,15 @@
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
@@ -240,26 +240,28 @@
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

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/literals.pyi` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ChatTokenCapabilityType",
     "CreateLoggingConfigurationStateType",
     "FallbackResultType",
     "LoggingConfigurationStateType",
     "UpdateLoggingConfigurationStateType",
     "ivschatServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ChatTokenCapabilityType = Literal["DELETE_MESSAGE", "DISCONNECT_USER", "SEND_MESSAGE"]
 CreateLoggingConfigurationStateType = Literal["ACTIVE"]
 FallbackResultType = Literal["ALLOW", "DENY"]
 LoggingConfigurationStateType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 UpdateLoggingConfigurationStateType = Literal["ACTIVE"]
@@ -49,14 +51,15 @@
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
@@ -152,14 +155,15 @@
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
@@ -238,26 +242,28 @@
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

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/type_defs.py` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat/type_defs.pyi` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/PKG-INFO` & `types-aiobotocore-ivschat-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-ivschat
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ivschat 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ivschat type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ivschat"></a>
 
 # types-aiobotocore-ivschat
 
 [![PyPI - types-aiobotocore-ivschat](https://img.shields.io/pypi/v/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivschat.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivschat)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/)
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
 [types-aiobotocore-ivschat docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,80 +233,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivschat.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ivschat` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/literals/).
+
 ```python
-from types_aiobotocore_ivschat.literals import (
-    ChatTokenCapabilityType,
-    CreateLoggingConfigurationStateType,
-    FallbackResultType,
-    LoggingConfigurationStateType,
-    UpdateLoggingConfigurationStateType,
-    ivschatServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivschat.literals import ChatTokenCapabilityType
 
 
 def check_value(value: ChatTokenCapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivschat.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivschat` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivschat/type_defs/).
+
 ```python
-from types_aiobotocore_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationTypeDef,
-    CreateChatTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    MessageReviewHandlerTypeDef,
-    DeleteLoggingConfigurationRequestRequestTypeDef,
-    DeleteMessageRequestRequestTypeDef,
-    DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
-    DisconnectUserRequestRequestTypeDef,
-    GetLoggingConfigurationRequestRequestTypeDef,
-    GetRoomRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRoomsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    SendEventRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
-    DeleteMessageResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SendEventResponseTypeDef,
-    CreateRoomRequestRequestTypeDef,
-    CreateRoomResponseTypeDef,
-    GetRoomResponseTypeDef,
-    RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
-    UpdateRoomResponseTypeDef,
-    DestinationConfigurationTypeDef,
-    ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
-    CreateLoggingConfigurationResponseTypeDef,
-    GetLoggingConfigurationResponseTypeDef,
-    LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    ListLoggingConfigurationsResponseTypeDef,
-)
+from types_aiobotocore_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
 
 
 def get_value() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivschat-2.5.2.post1/types_aiobotocore_ivschat.egg-info/SOURCES.txt` & `types-aiobotocore-ivschat-2.5.2.post2/types_aiobotocore_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

