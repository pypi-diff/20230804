# Comparing `tmp/types-aiobotocore-simspaceweaver-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-simspaceweaver-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1.tar` & `types-aiobotocore-simspaceweaver-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12569 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11023 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.826643 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      498 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      497 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13279 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8759 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8757 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10576 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10569 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.826643 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12569 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/LICENSE` & `types-aiobotocore-simspaceweaver-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,83 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_simspaceweaver.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SimSpaceWeaver` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/literals/).
+
 ```python
-from types_aiobotocore_simspaceweaver.literals import (
-    ClockStatusType,
-    ClockTargetStatusType,
-    LifecycleManagementStrategyType,
-    SimulationAppStatusType,
-    SimulationAppTargetStatusType,
-    SimulationStatusType,
-    SimulationTargetStatusType,
-    SimSpaceWeaverServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_simspaceweaver.literals import ClockStatusType
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimSpaceWeaver` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/type_defs/).
+
 ```python
-from types_aiobotocore_simspaceweaver.type_defs import (
-    CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
-    DeleteAppInputRequestTypeDef,
-    DeleteSimulationInputRequestTypeDef,
-    DescribeAppInputRequestTypeDef,
-    LaunchOverridesOutputTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
-    DomainTypeDef,
-    LaunchOverridesTypeDef,
-    ListAppsInputRequestTypeDef,
-    SimulationAppMetadataTypeDef,
-    ListSimulationsInputRequestTypeDef,
-    SimulationMetadataTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    SimulationClockTypeDef,
-    SimulationAppPortMappingTypeDef,
-    StartClockInputRequestTypeDef,
-    StopAppInputRequestTypeDef,
-    StopClockInputRequestTypeDef,
-    StopSimulationInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
-    StartSimulationInputRequestTypeDef,
-    LaunchOverridesUnionTypeDef,
-    StartAppInputRequestTypeDef,
-    ListAppsOutputTypeDef,
-    ListSimulationsOutputTypeDef,
-    LiveSimulationStateTypeDef,
-    SimulationAppEndpointInfoTypeDef,
-    LoggingConfigurationTypeDef,
-    DescribeAppOutputTypeDef,
-    DescribeSimulationOutputTypeDef,
-)
+from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
 
 def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/README.md` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-simspaceweaver
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,83 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_simspaceweaver.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SimSpaceWeaver` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/literals/).
+
 ```python
-from types_aiobotocore_simspaceweaver.literals import (
-    ClockStatusType,
-    ClockTargetStatusType,
-    LifecycleManagementStrategyType,
-    SimulationAppStatusType,
-    SimulationAppTargetStatusType,
-    SimulationStatusType,
-    SimulationTargetStatusType,
-    SimSpaceWeaverServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_simspaceweaver.literals import ClockStatusType
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimSpaceWeaver` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/type_defs/).
+
 ```python
-from types_aiobotocore_simspaceweaver.type_defs import (
-    CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
-    DeleteAppInputRequestTypeDef,
-    DeleteSimulationInputRequestTypeDef,
-    DescribeAppInputRequestTypeDef,
-    LaunchOverridesOutputTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
-    DomainTypeDef,
-    LaunchOverridesTypeDef,
-    ListAppsInputRequestTypeDef,
-    SimulationAppMetadataTypeDef,
-    ListSimulationsInputRequestTypeDef,
-    SimulationMetadataTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    SimulationClockTypeDef,
-    SimulationAppPortMappingTypeDef,
-    StartClockInputRequestTypeDef,
-    StopAppInputRequestTypeDef,
-    StopClockInputRequestTypeDef,
-    StopSimulationInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
-    StartSimulationInputRequestTypeDef,
-    LaunchOverridesUnionTypeDef,
-    StartAppInputRequestTypeDef,
-    ListAppsOutputTypeDef,
-    ListSimulationsOutputTypeDef,
-    LiveSimulationStateTypeDef,
-    SimulationAppEndpointInfoTypeDef,
-    LoggingConfigurationTypeDef,
-    DescribeAppOutputTypeDef,
-    DescribeSimulationOutputTypeDef,
-)
+from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
 
 def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/setup.py` & `types-aiobotocore-simspaceweaver-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-simspaceweaver",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__main__.py` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.py` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
-    LaunchOverridesUnionTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
@@ -178,15 +178,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesUnionTypeDef = ...
+        LaunchOverrides: LaunchOverridesTypeDef = ...
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
-    LaunchOverridesUnionTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
@@ -163,15 +163,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesUnionTypeDef = ...
+        LaunchOverrides: LaunchOverridesTypeDef = ...
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.py` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
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
@@ -168,14 +169,15 @@
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
@@ -254,26 +256,28 @@
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,26 +254,28 @@
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.py` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
     data: CloudWatchLogsLogGroupTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ClockStatusType,
     ClockTargetStatusType,
     LifecycleManagementStrategyType,
     SimulationAppStatusType,
     SimulationAppTargetStatusType,
@@ -33,20 +33,19 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesOutputTypeDef",
+    "LaunchOverridesTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
-    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "SimulationClockTypeDef",
     "SimulationAppPortMappingTypeDef",
@@ -54,20 +53,19 @@
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
+    "StartAppInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
-    "LaunchOverridesUnionTypeDef",
-    "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
@@ -111,16 +109,16 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesOutputTypeDef = TypedDict(
-    "LaunchOverridesOutputTypeDef",
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -155,22 +153,14 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
-    {
-        "LaunchCommands": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -306,14 +296,39 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
+_RequiredStartAppInputRequestTypeDef = TypedDict(
+    "_RequiredStartAppInputRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+    },
+)
+_OptionalStartAppInputRequestTypeDef = TypedDict(
+    "_OptionalStartAppInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "LaunchOverrides": LaunchOverridesTypeDef,
+    },
+    total=False,
+)
+
+
+class StartAppInputRequestTypeDef(
+    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
+):
+    pass
+
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -361,40 +376,14 @@
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
 
-LaunchOverridesUnionTypeDef = Union[LaunchOverridesTypeDef, LaunchOverridesOutputTypeDef]
-_RequiredStartAppInputRequestTypeDef = TypedDict(
-    "_RequiredStartAppInputRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-    },
-)
-_OptionalStartAppInputRequestTypeDef = TypedDict(
-    "_OptionalStartAppInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "LaunchOverrides": LaunchOverridesTypeDef,
-    },
-    total=False,
-)
-
-
-class StartAppInputRequestTypeDef(
-    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
-):
-    pass
-
-
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -437,15 +426,15 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesOutputTypeDef,
+        "LaunchOverrides": LaunchOverridesTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
     data: CloudWatchLogsLogGroupTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ClockStatusType,
     ClockTargetStatusType,
     LifecycleManagementStrategyType,
     SimulationAppStatusType,
     SimulationAppTargetStatusType,
@@ -32,20 +32,19 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesOutputTypeDef",
+    "LaunchOverridesTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
-    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "SimulationClockTypeDef",
     "SimulationAppPortMappingTypeDef",
@@ -53,20 +52,19 @@
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
+    "StartAppInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
-    "LaunchOverridesUnionTypeDef",
-    "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
@@ -110,16 +108,16 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesOutputTypeDef = TypedDict(
-    "LaunchOverridesOutputTypeDef",
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -154,22 +152,14 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
-    {
-        "LaunchCommands": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -303,14 +293,37 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
+_RequiredStartAppInputRequestTypeDef = TypedDict(
+    "_RequiredStartAppInputRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+    },
+)
+_OptionalStartAppInputRequestTypeDef = TypedDict(
+    "_OptionalStartAppInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "LaunchOverrides": LaunchOverridesTypeDef,
+    },
+    total=False,
+)
+
+class StartAppInputRequestTypeDef(
+    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
+):
+    pass
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -356,38 +369,14 @@
 )
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
-LaunchOverridesUnionTypeDef = Union[LaunchOverridesTypeDef, LaunchOverridesOutputTypeDef]
-_RequiredStartAppInputRequestTypeDef = TypedDict(
-    "_RequiredStartAppInputRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-    },
-)
-_OptionalStartAppInputRequestTypeDef = TypedDict(
-    "_OptionalStartAppInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "LaunchOverrides": LaunchOverridesTypeDef,
-    },
-    total=False,
-)
-
-class StartAppInputRequestTypeDef(
-    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
-):
-    pass
-
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -430,15 +419,15 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesOutputTypeDef,
+        "LaunchOverrides": LaunchOverridesTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,83 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_simspaceweaver.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SimSpaceWeaver` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/literals/).
+
 ```python
-from types_aiobotocore_simspaceweaver.literals import (
-    ClockStatusType,
-    ClockTargetStatusType,
-    LifecycleManagementStrategyType,
-    SimulationAppStatusType,
-    SimulationAppTargetStatusType,
-    SimulationStatusType,
-    SimulationTargetStatusType,
-    SimSpaceWeaverServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_simspaceweaver.literals import ClockStatusType
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimSpaceWeaver` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/type_defs/).
+
 ```python
-from types_aiobotocore_simspaceweaver.type_defs import (
-    CloudWatchLogsLogGroupTypeDef,
-    S3DestinationTypeDef,
-    DeleteAppInputRequestTypeDef,
-    DeleteSimulationInputRequestTypeDef,
-    DescribeAppInputRequestTypeDef,
-    LaunchOverridesOutputTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeSimulationInputRequestTypeDef,
-    S3LocationTypeDef,
-    DomainTypeDef,
-    LaunchOverridesTypeDef,
-    ListAppsInputRequestTypeDef,
-    SimulationAppMetadataTypeDef,
-    ListSimulationsInputRequestTypeDef,
-    SimulationMetadataTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    SimulationClockTypeDef,
-    SimulationAppPortMappingTypeDef,
-    StartClockInputRequestTypeDef,
-    StopAppInputRequestTypeDef,
-    StopClockInputRequestTypeDef,
-    StopSimulationInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    LogDestinationTypeDef,
-    CreateSnapshotInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
-    StartSimulationInputRequestTypeDef,
-    LaunchOverridesUnionTypeDef,
-    StartAppInputRequestTypeDef,
-    ListAppsOutputTypeDef,
-    ListSimulationsOutputTypeDef,
-    LiveSimulationStateTypeDef,
-    SimulationAppEndpointInfoTypeDef,
-    LoggingConfigurationTypeDef,
-    DescribeAppOutputTypeDef,
-    DescribeSimulationOutputTypeDef,
-)
+from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
 
 def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt` & `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

