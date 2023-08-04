# Comparing `tmp/types-aiobotocore-scheduler-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-scheduler-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-scheduler-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-scheduler-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-scheduler-2.5.2.post1.tar` & `types-aiobotocore-scheduler-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.421465 types-aiobotocore-scheduler-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-08-02 14:52:58.417465 types-aiobotocore-scheduler-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:58.421465 types-aiobotocore-scheduler-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.409465 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-08-02 14:49:03.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-08-02 14:49:03.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-02 14:49:03.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18511 2023-08-02 14:49:03.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:02.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.417465 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:58.000000 types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.686643 types-aiobotocore-scheduler-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11788 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.686643 types-aiobotocore-scheduler-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2097 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      939 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13232 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9268 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9266 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3359 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3355 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15803 2023-08-04 13:52:38.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15781 2023-08-04 13:52:38.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/LICENSE` & `types-aiobotocore-scheduler-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/PKG-INFO` & `types-aiobotocore-scheduler-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,101 +295,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_scheduler.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `EventBridgeScheduler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/literals/).
+
 ```python
-from types_aiobotocore_scheduler.literals import (
-    AssignPublicIpType,
-    FlexibleTimeWindowModeType,
-    LaunchTypeType,
-    ListScheduleGroupsPaginatorName,
-    ListSchedulesPaginatorName,
-    PlacementConstraintTypeType,
-    PlacementStrategyTypeType,
-    PropagateTagsType,
-    ScheduleGroupStateType,
-    ScheduleStateType,
-    EventBridgeSchedulerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_scheduler.literals import ActionAfterCompletionType
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EventBridgeScheduler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/type_defs/).
+
 ```python
-from types_aiobotocore_scheduler.type_defs import (
-    AwsVpcConfigurationOutputTypeDef,
-    AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    FlexibleTimeWindowTypeDef,
-    TimestampTypeDef,
-    DeadLetterConfigTypeDef,
-    DeleteScheduleGroupInputRequestTypeDef,
-    DeleteScheduleInputRequestTypeDef,
-    PlacementConstraintTypeDef,
-    PlacementStrategyTypeDef,
-    EventBridgeParametersTypeDef,
-    GetScheduleGroupInputRequestTypeDef,
-    GetScheduleInputRequestTypeDef,
-    KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
-    ListScheduleGroupsInputRequestTypeDef,
-    ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RetryPolicyTypeDef,
-    SageMakerPipelineParameterTypeDef,
-    TargetSummaryTypeDef,
-    SqsParametersTypeDef,
-    UntagResourceInputRequestTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
-    ListScheduleGroupsOutputTypeDef,
-    SageMakerPipelineParametersOutputTypeDef,
-    SageMakerPipelineParametersTypeDef,
-    ScheduleSummaryTypeDef,
-    EcsParametersOutputTypeDef,
-    EcsParametersTypeDef,
-    ListSchedulesOutputTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
-    GetScheduleOutputTypeDef,
-    CreateScheduleInputRequestTypeDef,
-    TargetUnionTypeDef,
-    UpdateScheduleInputRequestTypeDef,
-)
+from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationTypeDef
 
 
-def get_value() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/README.md` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-scheduler
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore scheduler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-scheduler"></a>
 
 # types-aiobotocore-scheduler
 
 [![PyPI - types-aiobotocore-scheduler](https://img.shields.io/pypi/v/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,101 +295,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_scheduler.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `EventBridgeScheduler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/literals/).
+
 ```python
-from types_aiobotocore_scheduler.literals import (
-    AssignPublicIpType,
-    FlexibleTimeWindowModeType,
-    LaunchTypeType,
-    ListScheduleGroupsPaginatorName,
-    ListSchedulesPaginatorName,
-    PlacementConstraintTypeType,
-    PlacementStrategyTypeType,
-    PropagateTagsType,
-    ScheduleGroupStateType,
-    ScheduleStateType,
-    EventBridgeSchedulerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_scheduler.literals import ActionAfterCompletionType
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EventBridgeScheduler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/type_defs/).
+
 ```python
-from types_aiobotocore_scheduler.type_defs import (
-    AwsVpcConfigurationOutputTypeDef,
-    AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    FlexibleTimeWindowTypeDef,
-    TimestampTypeDef,
-    DeadLetterConfigTypeDef,
-    DeleteScheduleGroupInputRequestTypeDef,
-    DeleteScheduleInputRequestTypeDef,
-    PlacementConstraintTypeDef,
-    PlacementStrategyTypeDef,
-    EventBridgeParametersTypeDef,
-    GetScheduleGroupInputRequestTypeDef,
-    GetScheduleInputRequestTypeDef,
-    KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
-    ListScheduleGroupsInputRequestTypeDef,
-    ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RetryPolicyTypeDef,
-    SageMakerPipelineParameterTypeDef,
-    TargetSummaryTypeDef,
-    SqsParametersTypeDef,
-    UntagResourceInputRequestTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
-    ListScheduleGroupsOutputTypeDef,
-    SageMakerPipelineParametersOutputTypeDef,
-    SageMakerPipelineParametersTypeDef,
-    ScheduleSummaryTypeDef,
-    EcsParametersOutputTypeDef,
-    EcsParametersTypeDef,
-    ListSchedulesOutputTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
-    GetScheduleOutputTypeDef,
-    CreateScheduleInputRequestTypeDef,
-    TargetUnionTypeDef,
-    UpdateScheduleInputRequestTypeDef,
-)
+from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationTypeDef
 
 
-def get_value() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/setup.py` & `types-aiobotocore-scheduler-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-scheduler",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__init__.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__init__.pyi` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/__main__.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/client.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import ScheduleStateType
+from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
     CreateScheduleOutputTypeDef,
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TimestampTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -99,15 +99,16 @@
 
     async def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetUnionTypeDef,
+        Target: TargetTypeDef,
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
@@ -232,15 +233,16 @@
 
     async def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetUnionTypeDef,
+        Target: TargetTypeDef,
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/client.pyi` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import ScheduleStateType
+from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
     CreateScheduleOutputTypeDef,
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TimestampTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -92,15 +92,16 @@
         """
     async def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetUnionTypeDef,
+        Target: TargetTypeDef,
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
@@ -213,15 +214,16 @@
         """
     async def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: TargetUnionTypeDef,
+        Target: TargetTypeDef,
+        ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/literals.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for scheduler service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_scheduler.literals import AssignPublicIpType
+    from types_aiobotocore_scheduler.literals import ActionAfterCompletionType
 
-    data: AssignPublicIpType = "DISABLED"
+    data: ActionAfterCompletionType = "DELETE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ActionAfterCompletionType",
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
     "PlacementStrategyTypeType",
@@ -34,14 +35,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+ActionAfterCompletionType = Literal["DELETE", "NONE"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
@@ -60,14 +62,15 @@
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
@@ -163,14 +166,15 @@
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
@@ -249,26 +253,28 @@
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

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/literals.pyi` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 Type annotations for scheduler service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_scheduler.literals import AssignPublicIpType
+    from types_aiobotocore_scheduler.literals import ActionAfterCompletionType
 
-    data: AssignPublicIpType = "DISABLED"
+    data: ActionAfterCompletionType = "DELETE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ActionAfterCompletionType",
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
     "PlacementConstraintTypeType",
     "PlacementStrategyTypeType",
@@ -32,14 +33,15 @@
     "EventBridgeSchedulerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+ActionAfterCompletionType = Literal["DELETE", "NONE"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
 PlacementStrategyTypeType = Literal["binpack", "random", "spread"]
@@ -58,14 +60,15 @@
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
@@ -161,14 +164,15 @@
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
@@ -247,26 +251,28 @@
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

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/paginator.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/paginator.pyi` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/type_defs.py` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 Type annotations for scheduler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
+    from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = ...
+    data: AwsVpcConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
     ScheduleGroupStateType,
     ScheduleStateType,
@@ -30,17 +31,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
     "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
@@ -58,62 +57,35 @@
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "RetryPolicyTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateScheduleGroupOutputTypeDef",
     "CreateScheduleOutputTypeDef",
     "GetScheduleGroupOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateScheduleOutputTypeDef",
     "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListScheduleGroupsOutputTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "GetScheduleOutputTypeDef",
     "CreateScheduleInputRequestTypeDef",
-    "TargetUnionTypeDef",
+    "GetScheduleOutputTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "AssignPublicIp": AssignPublicIpType,
-        "SecurityGroups": List[str],
-    },
-    total=False,
-)
-
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -121,21 +93,19 @@
     {
         "AssignPublicIp": AssignPublicIpType,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -143,21 +113,19 @@
     {
         "base": int,
         "weight": int,
     },
     total=False,
 )
 
-
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -183,21 +151,19 @@
     "_OptionalFlexibleTimeWindowTypeDef",
     {
         "MaximumWindowInMinutes": int,
     },
     total=False,
 )
 
-
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
-
 TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
@@ -213,21 +179,19 @@
     "_OptionalDeleteScheduleGroupInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteScheduleGroupInputRequestTypeDef(
     _RequiredDeleteScheduleGroupInputRequestTypeDef, _OptionalDeleteScheduleGroupInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteScheduleInputRequestTypeDef = TypedDict(
     "_RequiredDeleteScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteScheduleInputRequestTypeDef = TypedDict(
@@ -235,21 +199,19 @@
     {
         "ClientToken": str,
         "GroupName": str,
     },
     total=False,
 )
 
-
 class DeleteScheduleInputRequestTypeDef(
     _RequiredDeleteScheduleInputRequestTypeDef, _OptionalDeleteScheduleInputRequestTypeDef
 ):
     pass
 
-
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
     total=False,
@@ -289,21 +251,19 @@
     "_OptionalGetScheduleInputRequestTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
-
 class GetScheduleInputRequestTypeDef(
     _RequiredGetScheduleInputRequestTypeDef, _OptionalGetScheduleInputRequestTypeDef
 ):
     pass
 
-
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
@@ -394,22 +354,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -425,21 +377,19 @@
     {
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -513,22 +463,14 @@
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
-    {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
-    },
-    total=False,
-)
-
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
@@ -543,47 +485,14 @@
         "Name": str,
         "State": ScheduleStateType,
         "Target": TargetSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredEcsParametersOutputTypeDef = TypedDict(
-    "_RequiredEcsParametersOutputTypeDef",
-    {
-        "TaskDefinitionArn": str,
-    },
-)
-_OptionalEcsParametersOutputTypeDef = TypedDict(
-    "_OptionalEcsParametersOutputTypeDef",
-    {
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "EnableECSManagedTags": bool,
-        "EnableExecuteCommand": bool,
-        "Group": str,
-        "LaunchType": LaunchTypeType,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
-        "PlatformVersion": str,
-        "PropagateTags": Literal["TASK_DEFINITION"],
-        "ReferenceId": str,
-        "Tags": List[Dict[str, str]],
-        "TaskCount": int,
-    },
-    total=False,
-)
-
-
-class EcsParametersOutputTypeDef(
-    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
-):
-    pass
-
-
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
@@ -602,55 +511,26 @@
         "ReferenceId": str,
         "Tags": Sequence[Mapping[str, str]],
         "TaskCount": int,
     },
     total=False,
 )
 
-
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
-
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Arn": str,
-        "RoleArn": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "EcsParameters": EcsParametersOutputTypeDef,
-        "EventBridgeParameters": EventBridgeParametersTypeDef,
-        "Input": str,
-        "KinesisParameters": KinesisParametersTypeDef,
-        "RetryPolicy": RetryPolicyTypeDef,
-        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "SqsParameters": SqsParametersTypeDef,
-    },
-    total=False,
-)
-
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
         "RoleArn": str,
     },
 )
@@ -665,94 +545,91 @@
         "RetryPolicy": RetryPolicyTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersTypeDef,
         "SqsParameters": SqsParametersTypeDef,
     },
     total=False,
 )
 
-
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
-
-GetScheduleOutputTypeDef = TypedDict(
-    "GetScheduleOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "Description": str,
-        "EndDate": datetime,
-        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
-        "GroupName": str,
-        "KmsKeyArn": str,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "ScheduleExpression": str,
-        "ScheduleExpressionTimezone": str,
-        "StartDate": datetime,
-        "State": ScheduleStateType,
-        "Target": TargetOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
-
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
+GetScheduleOutputTypeDef = TypedDict(
+    "GetScheduleOutputTypeDef",
+    {
+        "ActionAfterCompletion": ActionAfterCompletionType,
+        "Arn": str,
+        "CreationDate": datetime,
+        "Description": str,
+        "EndDate": datetime,
+        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
+        "GroupName": str,
+        "KmsKeyArn": str,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "ScheduleExpression": str,
+        "ScheduleExpressionTimezone": str,
+        "StartDate": datetime,
+        "State": ScheduleStateType,
+        "Target": TargetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
-
 class UpdateScheduleInputRequestTypeDef(
     _RequiredUpdateScheduleInputRequestTypeDef, _OptionalUpdateScheduleInputRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler/type_defs.pyi` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 Type annotations for scheduler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
+    from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = ...
+    data: AwsVpcConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionAfterCompletionType,
     AssignPublicIpType,
     FlexibleTimeWindowModeType,
     LaunchTypeType,
     PlacementConstraintTypeType,
     PlacementStrategyTypeType,
     ScheduleGroupStateType,
     ScheduleStateType,
@@ -30,16 +31,16 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
     "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
@@ -57,60 +58,35 @@
     "ListSchedulesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "RetryPolicyTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "TargetSummaryTypeDef",
     "SqsParametersTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateScheduleGroupInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateScheduleGroupOutputTypeDef",
     "CreateScheduleOutputTypeDef",
     "GetScheduleGroupOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateScheduleOutputTypeDef",
     "ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef",
     "ListSchedulesInputListSchedulesPaginateTypeDef",
     "ListScheduleGroupsOutputTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "ScheduleSummaryTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "GetScheduleOutputTypeDef",
     "CreateScheduleInputRequestTypeDef",
-    "TargetUnionTypeDef",
+    "GetScheduleOutputTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "AssignPublicIp": AssignPublicIpType,
-        "SecurityGroups": List[str],
-    },
-    total=False,
-)
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -118,19 +94,21 @@
     {
         "AssignPublicIp": AssignPublicIpType,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -138,19 +116,21 @@
     {
         "base": int,
         "weight": int,
     },
     total=False,
 )
 
+
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -176,19 +156,21 @@
     "_OptionalFlexibleTimeWindowTypeDef",
     {
         "MaximumWindowInMinutes": int,
     },
     total=False,
 )
 
+
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
+
 TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
@@ -204,19 +186,21 @@
     "_OptionalDeleteScheduleGroupInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteScheduleGroupInputRequestTypeDef(
     _RequiredDeleteScheduleGroupInputRequestTypeDef, _OptionalDeleteScheduleGroupInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteScheduleInputRequestTypeDef = TypedDict(
     "_RequiredDeleteScheduleInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteScheduleInputRequestTypeDef = TypedDict(
@@ -224,19 +208,21 @@
     {
         "ClientToken": str,
         "GroupName": str,
     },
     total=False,
 )
 
+
 class DeleteScheduleInputRequestTypeDef(
     _RequiredDeleteScheduleInputRequestTypeDef, _OptionalDeleteScheduleInputRequestTypeDef
 ):
     pass
 
+
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
     total=False,
@@ -276,19 +262,21 @@
     "_OptionalGetScheduleInputRequestTypeDef",
     {
         "GroupName": str,
     },
     total=False,
 )
 
+
 class GetScheduleInputRequestTypeDef(
     _RequiredGetScheduleInputRequestTypeDef, _OptionalGetScheduleInputRequestTypeDef
 ):
     pass
 
+
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
@@ -379,22 +367,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -410,19 +390,21 @@
     {
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateScheduleGroupInputRequestTypeDef(
     _RequiredCreateScheduleGroupInputRequestTypeDef, _OptionalCreateScheduleGroupInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -496,22 +478,14 @@
     {
         "NextToken": str,
         "ScheduleGroups": List[ScheduleGroupSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
-    {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
-    },
-    total=False,
-)
-
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
         "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
@@ -526,45 +500,14 @@
         "Name": str,
         "State": ScheduleStateType,
         "Target": TargetSummaryTypeDef,
     },
     total=False,
 )
 
-_RequiredEcsParametersOutputTypeDef = TypedDict(
-    "_RequiredEcsParametersOutputTypeDef",
-    {
-        "TaskDefinitionArn": str,
-    },
-)
-_OptionalEcsParametersOutputTypeDef = TypedDict(
-    "_OptionalEcsParametersOutputTypeDef",
-    {
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "EnableECSManagedTags": bool,
-        "EnableExecuteCommand": bool,
-        "Group": str,
-        "LaunchType": LaunchTypeType,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
-        "PlatformVersion": str,
-        "PropagateTags": Literal["TASK_DEFINITION"],
-        "ReferenceId": str,
-        "Tags": List[Dict[str, str]],
-        "TaskCount": int,
-    },
-    total=False,
-)
-
-class EcsParametersOutputTypeDef(
-    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
-):
-    pass
-
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
@@ -583,51 +526,28 @@
         "ReferenceId": str,
         "Tags": Sequence[Mapping[str, str]],
         "TaskCount": int,
     },
     total=False,
 )
 
+
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
+
 ListSchedulesOutputTypeDef = TypedDict(
     "ListSchedulesOutputTypeDef",
     {
         "NextToken": str,
         "Schedules": List[ScheduleSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Arn": str,
-        "RoleArn": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "EcsParameters": EcsParametersOutputTypeDef,
-        "EventBridgeParameters": EventBridgeParametersTypeDef,
-        "Input": str,
-        "KinesisParameters": KinesisParametersTypeDef,
-        "RetryPolicy": RetryPolicyTypeDef,
-        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "SqsParameters": SqsParametersTypeDef,
-    },
-    total=False,
-)
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Arn": str,
         "RoleArn": str,
     },
 )
@@ -642,89 +562,96 @@
         "RetryPolicy": RetryPolicyTypeDef,
         "SageMakerPipelineParameters": SageMakerPipelineParametersTypeDef,
         "SqsParameters": SqsParametersTypeDef,
     },
     total=False,
 )
 
+
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
-GetScheduleOutputTypeDef = TypedDict(
-    "GetScheduleOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationDate": datetime,
-        "Description": str,
-        "EndDate": datetime,
-        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
-        "GroupName": str,
-        "KmsKeyArn": str,
-        "LastModificationDate": datetime,
-        "Name": str,
-        "ScheduleExpression": str,
-        "ScheduleExpressionTimezone": str,
-        "StartDate": datetime,
-        "State": ScheduleStateType,
-        "Target": TargetOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
+
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
+
+GetScheduleOutputTypeDef = TypedDict(
+    "GetScheduleOutputTypeDef",
+    {
+        "ActionAfterCompletion": ActionAfterCompletionType,
+        "Arn": str,
+        "CreationDate": datetime,
+        "Description": str,
+        "EndDate": datetime,
+        "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
+        "GroupName": str,
+        "KmsKeyArn": str,
+        "LastModificationDate": datetime,
+        "Name": str,
+        "ScheduleExpression": str,
+        "ScheduleExpressionTimezone": str,
+        "StartDate": datetime,
+        "State": ScheduleStateType,
+        "Target": TargetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
     },
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
+        "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
         "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
         "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
+
 class UpdateScheduleInputRequestTypeDef(
     _RequiredUpdateScheduleInputRequestTypeDef, _OptionalUpdateScheduleInputRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/PKG-INFO` & `types-aiobotocore-scheduler-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-scheduler
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore scheduler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-scheduler"></a>
 
 # types-aiobotocore-scheduler
 
 [![PyPI - types-aiobotocore-scheduler](https://img.shields.io/pypi/v/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,101 +263,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_scheduler.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `EventBridgeScheduler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/literals/).
+
 ```python
-from types_aiobotocore_scheduler.literals import (
-    AssignPublicIpType,
-    FlexibleTimeWindowModeType,
-    LaunchTypeType,
-    ListScheduleGroupsPaginatorName,
-    ListSchedulesPaginatorName,
-    PlacementConstraintTypeType,
-    PlacementStrategyTypeType,
-    PropagateTagsType,
-    ScheduleGroupStateType,
-    ScheduleStateType,
-    EventBridgeSchedulerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_scheduler.literals import ActionAfterCompletionType
 
 
-def check_value(value: AssignPublicIpType) -> bool:
+def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_scheduler.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EventBridgeScheduler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/type_defs/).
+
 ```python
-from types_aiobotocore_scheduler.type_defs import (
-    AwsVpcConfigurationOutputTypeDef,
-    AwsVpcConfigurationTypeDef,
-    CapacityProviderStrategyItemTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    FlexibleTimeWindowTypeDef,
-    TimestampTypeDef,
-    DeadLetterConfigTypeDef,
-    DeleteScheduleGroupInputRequestTypeDef,
-    DeleteScheduleInputRequestTypeDef,
-    PlacementConstraintTypeDef,
-    PlacementStrategyTypeDef,
-    EventBridgeParametersTypeDef,
-    GetScheduleGroupInputRequestTypeDef,
-    GetScheduleInputRequestTypeDef,
-    KinesisParametersTypeDef,
-    PaginatorConfigTypeDef,
-    ListScheduleGroupsInputRequestTypeDef,
-    ScheduleGroupSummaryTypeDef,
-    ListSchedulesInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RetryPolicyTypeDef,
-    SageMakerPipelineParameterTypeDef,
-    TargetSummaryTypeDef,
-    SqsParametersTypeDef,
-    UntagResourceInputRequestTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateScheduleGroupInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateScheduleGroupOutputTypeDef,
-    CreateScheduleOutputTypeDef,
-    GetScheduleGroupOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateScheduleOutputTypeDef,
-    ListScheduleGroupsInputListScheduleGroupsPaginateTypeDef,
-    ListSchedulesInputListSchedulesPaginateTypeDef,
-    ListScheduleGroupsOutputTypeDef,
-    SageMakerPipelineParametersOutputTypeDef,
-    SageMakerPipelineParametersTypeDef,
-    ScheduleSummaryTypeDef,
-    EcsParametersOutputTypeDef,
-    EcsParametersTypeDef,
-    ListSchedulesOutputTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
-    GetScheduleOutputTypeDef,
-    CreateScheduleInputRequestTypeDef,
-    TargetUnionTypeDef,
-    UpdateScheduleInputRequestTypeDef,
-)
+from types_aiobotocore_scheduler.type_defs import AwsVpcConfigurationTypeDef
 
 
-def get_value() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post1/types_aiobotocore_scheduler.egg-info/SOURCES.txt` & `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

