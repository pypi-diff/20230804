# Comparing `tmp/types-aiobotocore-codeguruprofiler-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codeguruprofiler-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:38 2023, max compression
```

## Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1.tar` & `types-aiobotocore-codeguruprofiler-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23256 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.427608 types-aiobotocore-codeguruprofiler-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-08-04 12:00:38.427608 types-aiobotocore-codeguruprofiler-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:38.427608 types-aiobotocore-codeguruprofiler-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.415608 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21314 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22311 2023-08-04 11:42:27.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:26.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.427608 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:38.000000 types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/LICENSE` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/README.md` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-codeguruprofiler
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore codeguruprofiler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,119 +291,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguruprofiler.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruProfiler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/literals/).
+
 ```python
-from types_aiobotocore_codeguruprofiler.literals import (
-    ActionGroupType,
-    AgentParameterFieldType,
-    AggregationPeriodType,
-    ComputePlatformType,
-    EventPublisherType,
-    FeedbackTypeType,
-    ListProfileTimesPaginatorName,
-    MetadataFieldType,
-    MetricTypeType,
-    OrderByType,
-    CodeGuruProfilerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codeguruprofiler.literals import ActionGroupType
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguruprofiler.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruProfiler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/type_defs/).
+
 ```python
-from types_aiobotocore_codeguruprofiler.type_defs import (
-    ResponseMetadataTypeDef,
-    AgentConfigurationTypeDef,
-    AgentOrchestrationConfigTypeDef,
-    AggregatedProfileTimeTypeDef,
-    UserFeedbackTypeDef,
-    MetricTypeDef,
-    TimestampTypeDef,
-    TimestampStructureTypeDef,
-    BlobTypeDef,
-    ChannelOutputTypeDef,
-    ChannelTypeDef,
-    ConfigureAgentRequestRequestTypeDef,
-    DeleteProfilingGroupRequestRequestTypeDef,
-    DescribeProfilingGroupRequestRequestTypeDef,
-    FindingsReportSummaryTypeDef,
-    FrameMetricOutputTypeDef,
-    FrameMetricTypeDef,
-    GetFindingsReportAccountSummaryRequestRequestTypeDef,
-    GetNotificationConfigurationRequestRequestTypeDef,
-    GetPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ProfileTimeTypeDef,
-    ListProfilingGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    MatchTypeDef,
-    PatternTypeDef,
-    PutPermissionRequestRequestTypeDef,
-    RemoveNotificationChannelRequestRequestTypeDef,
-    RemovePermissionRequestRequestTypeDef,
-    SubmitFeedbackRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutPermissionResponseTypeDef,
-    RemovePermissionResponseTypeDef,
-    ConfigureAgentResponseTypeDef,
-    CreateProfilingGroupRequestRequestTypeDef,
-    UpdateProfilingGroupRequestRequestTypeDef,
-    ProfilingStatusTypeDef,
-    AnomalyInstanceTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
-    ChannelUnionTypeDef,
-    GetFindingsReportAccountSummaryResponseTypeDef,
-    ListFindingsReportsResponseTypeDef,
-    FrameMetricDatumTypeDef,
-    FrameMetricUnionTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    ListProfileTimesResponseTypeDef,
-    RecommendationTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
-    AddNotificationChannelsResponseTypeDef,
-    GetNotificationConfigurationResponseTypeDef,
-    RemoveNotificationChannelResponseTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
-    BatchGetFrameMetricDataResponseTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
-    CreateProfilingGroupResponseTypeDef,
-    DescribeProfilingGroupResponseTypeDef,
-    ListProfilingGroupsResponseTypeDef,
-    UpdateProfilingGroupResponseTypeDef,
-    GetRecommendationsResponseTypeDef,
-)
+from types_aiobotocore_codeguruprofiler.type_defs import ChannelTypeDef
 
 
-def get_value() -> ResponseMetadataTypeDef:
+def get_value() -> ChannelTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguruprofiler",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__main__.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeGuruProfiler 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
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

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
     BlobTypeDef,
-    ChannelUnionTypeDef,
+    ChannelTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricUnionTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
@@ -95,29 +95,29 @@
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#exceptions)
         """
 
     async def add_notification_channels(
-        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
+        self, *, channels: Sequence[ChannelTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#add_notification_channels)
         """
 
     async def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
         endTime: TimestampTypeDef = ...,
-        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
+        frameMetrics: Sequence[FrameMetricTypeDef] = ...,
         period: str = ...,
         startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
     BlobTypeDef,
-    ChannelUnionTypeDef,
+    ChannelTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricUnionTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
@@ -90,28 +90,28 @@
         """
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#exceptions)
         """
     async def add_notification_channels(
-        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
+        self, *, channels: Sequence[ChannelTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#add_notification_channels)
         """
     async def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
         endTime: TimestampTypeDef = ...,
-        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
+        frameMetrics: Sequence[FrameMetricTypeDef] = ...,
         period: str = ...,
         startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_codeguruprofiler.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_codeguruprofiler.type_defs import ChannelTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: ChannelTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,33 +31,30 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
+    "FrameMetricTypeDef",
     "TimestampTypeDef",
     "TimestampStructureTypeDef",
     "BlobTypeDef",
-    "ChannelOutputTypeDef",
-    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
-    "FrameMetricOutputTypeDef",
-    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -65,53 +62,69 @@
     "PatternTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutPermissionResponseTypeDef",
     "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
+    "FrameMetricDatumTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
-    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
-    "FrameMetricDatumTypeDef",
-    "FrameMetricUnionTypeDef",
     "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
+    {
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -130,21 +143,19 @@
     "_OptionalAgentConfigurationTypeDef",
     {
         "agentParameters": Dict[AgentParameterFieldType, str],
     },
     total=False,
 )
 
-
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
-
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -169,63 +180,32 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
+    {
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 TimestampTypeDef = Union[datetime, str]
 TimestampStructureTypeDef = TypedDict(
     "TimestampStructureTypeDef",
     {
         "value": datetime,
     },
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "eventPublishers": List[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
-
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
-
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -233,21 +213,19 @@
     {
         "fleetInstanceId": str,
         "metadata": Mapping[MetadataFieldType, str],
     },
     total=False,
 )
 
-
 class ConfigureAgentRequestRequestTypeDef(
     _RequiredConfigureAgentRequestRequestTypeDef, _OptionalConfigureAgentRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProfilingGroupRequestRequestTypeDef = TypedDict(
     "DeleteProfilingGroupRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
@@ -266,32 +244,14 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
-FrameMetricOutputTypeDef = TypedDict(
-    "FrameMetricOutputTypeDef",
-    {
-        "frameName": str,
-        "threadStates": List[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
-    },
-)
-
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
-    {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
-    },
-)
-
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -383,21 +343,19 @@
     "_OptionalPutPermissionRequestRequestTypeDef",
     {
         "revisionId": str,
     },
     total=False,
 )
 
-
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
-
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -423,21 +381,19 @@
     "_OptionalSubmitFeedbackRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
-
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -446,14 +402,30 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
+    {
+        "channels": Sequence[ChannelTypeDef],
+        "profilingGroupName": str,
+    },
+)
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelTypeDef],
+    },
+    total=False,
+)
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "policy": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -516,22 +488,20 @@
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "computePlatform": ComputePlatformType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProfilingGroupRequestRequestTypeDef(
     _RequiredCreateProfilingGroupRequestRequestTypeDef,
     _OptionalCreateProfilingGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateProfilingGroupRequestRequestTypeDef = TypedDict(
     "UpdateProfilingGroupRequestRequestTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "profilingGroupName": str,
     },
 )
@@ -558,18 +528,48 @@
     {
         "endTime": datetime,
         "userFeedback": UserFeedbackTypeDef,
     },
     total=False,
 )
 
-
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricTypeDef,
+        "values": List[float],
+    },
+)
+
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
 
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
@@ -581,21 +581,19 @@
         "maxDepth": int,
         "period": str,
         "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
     },
@@ -604,22 +602,20 @@
     "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class GetRecommendationsRequestRequestTypeDef(
     _RequiredGetRecommendationsRequestRequestTypeDef,
     _OptionalGetRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsReportsRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
     },
@@ -630,22 +626,20 @@
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
@@ -657,21 +651,19 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-
 class ListProfileTimesRequestRequestTypeDef(
     _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPostAgentProfileRequestRequestTypeDef",
     {
         "agentProfile": BlobTypeDef,
         "contentType": str,
         "profilingGroupName": str,
     },
@@ -680,30 +672,19 @@
     "_OptionalPostAgentProfileRequestRequestTypeDef",
     {
         "profileToken": str,
     },
     total=False,
 )
 
-
 class PostAgentProfileRequestRequestTypeDef(
     _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
 ):
     pass
 
-
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelOutputTypeDef],
-    },
-    total=False,
-)
-
-ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -714,23 +695,14 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
-    {
-        "frameMetric": FrameMetricOutputTypeDef,
-        "values": List[float],
-    },
-)
-
-FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
 _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
         "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
@@ -741,22 +713,20 @@
     {
         "orderBy": OrderByType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
     _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
     _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
 ):
     pass
 
-
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -770,38 +740,14 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
-    },
-)
-
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -818,19 +764,35 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
     {
-        "channels": Sequence[ChannelUnionTypeDef],
-        "profilingGroupName": str,
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
@@ -839,40 +801,14 @@
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
-    {
-        "endTime": TimestampTypeDef,
-        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
-        "period": str,
-        "startTime": TimestampTypeDef,
-        "targetResolution": AggregationPeriodType,
-    },
-    total=False,
-)
-
-
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
-):
-    pass
-
-
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_codeguruprofiler.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_codeguruprofiler.type_defs import ChannelTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: ChannelTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,32 +31,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
+    "FrameMetricTypeDef",
     "TimestampTypeDef",
     "TimestampStructureTypeDef",
     "BlobTypeDef",
-    "ChannelOutputTypeDef",
-    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
-    "FrameMetricOutputTypeDef",
-    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -64,53 +63,71 @@
     "PatternTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
     "GetPolicyResponseTypeDef",
     "GetProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutPermissionResponseTypeDef",
     "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
+    "FrameMetricDatumTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "ListFindingsReportsRequestRequestTypeDef",
     "ListProfileTimesRequestRequestTypeDef",
     "PostAgentProfileRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
-    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
-    "FrameMetricDatumTypeDef",
-    "FrameMetricUnionTypeDef",
     "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
+    {
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -129,19 +146,21 @@
     "_OptionalAgentConfigurationTypeDef",
     {
         "agentParameters": Dict[AgentParameterFieldType, str],
     },
     total=False,
 )
 
+
 class AgentConfigurationTypeDef(
     _RequiredAgentConfigurationTypeDef, _OptionalAgentConfigurationTypeDef
 ):
     pass
 
+
 AgentOrchestrationConfigTypeDef = TypedDict(
     "AgentOrchestrationConfigTypeDef",
     {
         "profilingEnabled": bool,
     },
 )
 
@@ -166,59 +185,32 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
+    {
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
+    },
+)
+
 TimestampTypeDef = Union[datetime, str]
 TimestampStructureTypeDef = TypedDict(
     "TimestampStructureTypeDef",
     {
         "value": datetime,
     },
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "eventPublishers": List[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
-    {
-        "id": str,
-    },
-    total=False,
-)
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -226,19 +218,21 @@
     {
         "fleetInstanceId": str,
         "metadata": Mapping[MetadataFieldType, str],
     },
     total=False,
 )
 
+
 class ConfigureAgentRequestRequestTypeDef(
     _RequiredConfigureAgentRequestRequestTypeDef, _OptionalConfigureAgentRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProfilingGroupRequestRequestTypeDef = TypedDict(
     "DeleteProfilingGroupRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 
@@ -257,32 +251,14 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
-FrameMetricOutputTypeDef = TypedDict(
-    "FrameMetricOutputTypeDef",
-    {
-        "frameName": str,
-        "threadStates": List[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
-    },
-)
-
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
-    {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
-    },
-)
-
 GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
@@ -374,19 +350,21 @@
     "_OptionalPutPermissionRequestRequestTypeDef",
     {
         "revisionId": str,
     },
     total=False,
 )
 
+
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
+
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -412,19 +390,21 @@
     "_OptionalSubmitFeedbackRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
+
 class SubmitFeedbackRequestRequestTypeDef(
     _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -433,14 +413,30 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
+    {
+        "channels": Sequence[ChannelTypeDef],
+        "profilingGroupName": str,
+    },
+)
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelTypeDef],
+    },
+    total=False,
+)
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "policy": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -503,20 +499,22 @@
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "computePlatform": ComputePlatformType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProfilingGroupRequestRequestTypeDef(
     _RequiredCreateProfilingGroupRequestRequestTypeDef,
     _OptionalCreateProfilingGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateProfilingGroupRequestRequestTypeDef = TypedDict(
     "UpdateProfilingGroupRequestRequestTypeDef",
     {
         "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
         "profilingGroupName": str,
     },
 )
@@ -543,17 +541,53 @@
     {
         "endTime": datetime,
         "userFeedback": UserFeedbackTypeDef,
     },
     total=False,
 )
 
+
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
+
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricTypeDef,
+        "values": List[float],
+    },
+)
+
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetProfileRequestRequestTypeDef = TypedDict(
     "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalGetProfileRequestRequestTypeDef = TypedDict(
@@ -564,19 +598,21 @@
         "maxDepth": int,
         "period": str,
         "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class GetProfileRequestRequestTypeDef(
     _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
     },
@@ -585,20 +621,22 @@
     "_OptionalGetRecommendationsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class GetRecommendationsRequestRequestTypeDef(
     _RequiredGetRecommendationsRequestRequestTypeDef,
     _OptionalGetRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsReportsRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
     },
@@ -609,20 +647,22 @@
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListFindingsReportsRequestRequestTypeDef(
     _RequiredListFindingsReportsRequestRequestTypeDef,
     _OptionalListFindingsReportsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestRequestTypeDef",
     {
         "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
@@ -634,19 +674,21 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
+
 class ListProfileTimesRequestRequestTypeDef(
     _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPostAgentProfileRequestRequestTypeDef",
     {
         "agentProfile": BlobTypeDef,
         "contentType": str,
         "profilingGroupName": str,
     },
@@ -655,28 +697,21 @@
     "_OptionalPostAgentProfileRequestRequestTypeDef",
     {
         "profileToken": str,
     },
     total=False,
 )
 
+
 class PostAgentProfileRequestRequestTypeDef(
     _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
 ):
     pass
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
-    {
-        "channels": List[ChannelOutputTypeDef],
-    },
-    total=False,
-)
 
-ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -687,23 +722,14 @@
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
-    {
-        "frameMetric": FrameMetricOutputTypeDef,
-        "values": List[float],
-    },
-)
-
-FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
 _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
     "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
     {
         "endTime": TimestampTypeDef,
         "period": AggregationPeriodType,
         "profilingGroupName": str,
         "startTime": TimestampTypeDef,
@@ -714,20 +740,22 @@
     {
         "orderBy": OrderByType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
     _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
     _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
 ):
     pass
 
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -741,38 +769,14 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
-    {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
-    },
-)
-
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -789,19 +793,35 @@
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
     {
-        "channels": Sequence[ChannelUnionTypeDef],
-        "profilingGroupName": str,
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
@@ -810,38 +830,14 @@
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
-    {
-        "endTime": TimestampTypeDef,
-        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
-        "period": str,
-        "startTime": TimestampTypeDef,
-        "targetResolution": AggregationPeriodType,
-    },
-    total=False,
-)
-
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
-):
-    pass
-
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-codeguruprofiler-2.5.2.post2/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

