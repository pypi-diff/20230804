# Comparing `tmp/types-aiobotocore-ivs-realtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ivs-realtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivs-realtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivs-realtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1.tar` & `types-aiobotocore-ivs-realtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.985555 types-aiobotocore-ivs-realtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-02 14:52:28.985555 types-aiobotocore-ivs-realtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.985555 types-aiobotocore-ivs-realtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.985555 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-08-02 14:41:11.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-08-02 14:41:11.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:10.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.985555 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:28.000000 types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12488 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10951 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      476 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13425 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13402 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8343 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8341 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12189 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12172 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12488 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/LICENSE` & `types-aiobotocore-ivs-realtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,77 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivs_realtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ivsrealtime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/literals/).
+
 ```python
-from types_aiobotocore_ivs_realtime.literals import (
-    EventErrorCodeType,
-    EventNameType,
-    ParticipantStateType,
-    ParticipantTokenCapabilityType,
-    ivsrealtimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivs_realtime.literals import EventErrorCodeType
 
 
 def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivs_realtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivsrealtime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/type_defs/).
+
 ```python
-from types_aiobotocore_ivs_realtime.type_defs import (
-    CreateParticipantTokenRequestRequestTypeDef,
-    ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
-    ParticipantTokenConfigurationTypeDef,
-    StageTypeDef,
-    DeleteStageRequestRequestTypeDef,
-    DisconnectParticipantRequestRequestTypeDef,
-    EventTypeDef,
-    GetParticipantRequestRequestTypeDef,
-    ParticipantTypeDef,
-    GetStageRequestRequestTypeDef,
-    GetStageSessionRequestRequestTypeDef,
-    StageSessionTypeDef,
-    ListParticipantEventsRequestRequestTypeDef,
-    ListParticipantsRequestRequestTypeDef,
-    ParticipantSummaryTypeDef,
-    ListStageSessionsRequestRequestTypeDef,
-    StageSessionSummaryTypeDef,
-    ListStagesRequestRequestTypeDef,
-    StageSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
-    CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateStageRequestRequestTypeDef,
-    CreateStageResponseTypeDef,
-    GetStageResponseTypeDef,
-    UpdateStageResponseTypeDef,
-    ListParticipantEventsResponseTypeDef,
-    GetParticipantResponseTypeDef,
-    GetStageSessionResponseTypeDef,
-    ListParticipantsResponseTypeDef,
-    ListStageSessionsResponseTypeDef,
-    ListStagesResponseTypeDef,
-)
+from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/README.md` & `types-aiobotocore-ivs-realtime-2.5.2.post2/README.md`

 * *Files 22% similar despite different names*

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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,77 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivs_realtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ivsrealtime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/literals/).
+
 ```python
-from types_aiobotocore_ivs_realtime.literals import (
-    EventErrorCodeType,
-    EventNameType,
-    ParticipantStateType,
-    ParticipantTokenCapabilityType,
-    ivsrealtimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivs_realtime.literals import EventErrorCodeType
 
 
 def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivs_realtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivsrealtime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/type_defs/).
+
 ```python
-from types_aiobotocore_ivs_realtime.type_defs import (
-    CreateParticipantTokenRequestRequestTypeDef,
-    ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
-    ParticipantTokenConfigurationTypeDef,
-    StageTypeDef,
-    DeleteStageRequestRequestTypeDef,
-    DisconnectParticipantRequestRequestTypeDef,
-    EventTypeDef,
-    GetParticipantRequestRequestTypeDef,
-    ParticipantTypeDef,
-    GetStageRequestRequestTypeDef,
-    GetStageSessionRequestRequestTypeDef,
-    StageSessionTypeDef,
-    ListParticipantEventsRequestRequestTypeDef,
-    ListParticipantsRequestRequestTypeDef,
-    ParticipantSummaryTypeDef,
-    ListStageSessionsRequestRequestTypeDef,
-    StageSessionSummaryTypeDef,
-    ListStagesRequestRequestTypeDef,
-    StageSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
-    CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateStageRequestRequestTypeDef,
-    CreateStageResponseTypeDef,
-    GetStageResponseTypeDef,
-    UpdateStageResponseTypeDef,
-    ListParticipantEventsResponseTypeDef,
-    GetParticipantResponseTypeDef,
-    GetStageSessionResponseTypeDef,
-    ListParticipantsResponseTypeDef,
-    ListStageSessionsResponseTypeDef,
-    ListStagesResponseTypeDef,
-)
+from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/setup.py` & `types-aiobotocore-ivs-realtime-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivs-realtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/__main__.py` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ivsrealtime 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ivsrealtime 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\nOther"
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

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/client.py` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/client.pyi` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/literals.py` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "EventErrorCodeType",
     "EventNameType",
     "ParticipantStateType",
     "ParticipantTokenCapabilityType",
     "ivsrealtimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 EventErrorCodeType = Literal["INSUFFICIENT_CAPABILITIES"]
 EventNameType = Literal[
     "JOINED",
     "JOIN_ERROR",
     "LEFT",
     "PUBLISH_ERROR",
     "PUBLISH_STARTED",
@@ -57,14 +55,15 @@
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
@@ -160,14 +159,15 @@
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
@@ -246,26 +246,28 @@
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

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/literals.pyi` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "EventErrorCodeType",
     "EventNameType",
     "ParticipantStateType",
     "ParticipantTokenCapabilityType",
     "ivsrealtimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 EventErrorCodeType = Literal["INSUFFICIENT_CAPABILITIES"]
 EventNameType = Literal[
     "JOINED",
     "JOIN_ERROR",
     "LEFT",
     "PUBLISH_ERROR",
     "PUBLISH_STARTED",
@@ -55,14 +57,15 @@
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
@@ -158,14 +161,15 @@
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
@@ -244,26 +248,28 @@
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

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/type_defs.py` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime/type_defs.pyi` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
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
 [types-aiobotocore-ivs-realtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,77 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ivs_realtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ivsrealtime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/literals/).
+
 ```python
-from types_aiobotocore_ivs_realtime.literals import (
-    EventErrorCodeType,
-    EventNameType,
-    ParticipantStateType,
-    ParticipantTokenCapabilityType,
-    ivsrealtimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ivs_realtime.literals import EventErrorCodeType
 
 
 def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ivs_realtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ivsrealtime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/type_defs/).
+
 ```python
-from types_aiobotocore_ivs_realtime.type_defs import (
-    CreateParticipantTokenRequestRequestTypeDef,
-    ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
-    ParticipantTokenConfigurationTypeDef,
-    StageTypeDef,
-    DeleteStageRequestRequestTypeDef,
-    DisconnectParticipantRequestRequestTypeDef,
-    EventTypeDef,
-    GetParticipantRequestRequestTypeDef,
-    ParticipantTypeDef,
-    GetStageRequestRequestTypeDef,
-    GetStageSessionRequestRequestTypeDef,
-    StageSessionTypeDef,
-    ListParticipantEventsRequestRequestTypeDef,
-    ListParticipantsRequestRequestTypeDef,
-    ParticipantSummaryTypeDef,
-    ListStageSessionsRequestRequestTypeDef,
-    StageSessionSummaryTypeDef,
-    ListStagesRequestRequestTypeDef,
-    StageSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
-    CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateStageRequestRequestTypeDef,
-    CreateStageResponseTypeDef,
-    GetStageResponseTypeDef,
-    UpdateStageResponseTypeDef,
-    ListParticipantEventsResponseTypeDef,
-    GetParticipantResponseTypeDef,
-    GetStageSessionResponseTypeDef,
-    ListParticipantsResponseTypeDef,
-    ListStageSessionsResponseTypeDef,
-    ListStagesResponseTypeDef,
-)
+from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post1/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt` & `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

