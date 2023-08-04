# Comparing `tmp/types-aiobotocore-iotevents-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotevents-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotevents-data-2.5.2.post1.tar` & `types-aiobotocore-iotevents-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.609562 types-aiobotocore-iotevents-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-08-02 14:52:26.609562 types-aiobotocore-iotevents-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.609562 types-aiobotocore-iotevents-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.605563 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:48.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.609562 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.436643 types-aiobotocore-iotevents-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12582 2023-08-04 13:59:12.426643 types-aiobotocore-iotevents-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11037 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.436643 types-aiobotocore-iotevents-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.426643 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      493 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      492 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11762 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11742 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8398 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8396 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18888 2023-08-04 13:41:03.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18863 2023-08-04 13:41:03.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:02.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.426643 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12582 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/LICENSE` & `types-aiobotocore-iotevents-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iotevents-data-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iotevents-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTEventsData 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotevents-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotevents-data"></a>
 
 # types-aiobotocore-iotevents-data
 
 [![PyPI - types-aiobotocore-iotevents-data](https://img.shields.io/pypi/v/types-aiobotocore-iotevents-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/)
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
 [types-aiobotocore-iotevents-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,103 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotevents_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTEventsData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/literals/).
+
 ```python
-from types_aiobotocore_iotevents_data.literals import (
-    AlarmStateNameType,
-    ComparisonOperatorType,
-    CustomerActionNameType,
-    ErrorCodeType,
-    EventTypeType,
-    TriggerTypeType,
-    IoTEventsDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_iotevents_data.literals import AlarmStateNameType
 
 
 def check_value(value: AlarmStateNameType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotevents_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTEventsData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/type_defs/).
+
 ```python
-from types_aiobotocore_iotevents_data.type_defs import (
-    AcknowledgeActionConfigurationTypeDef,
-    AcknowledgeAlarmActionRequestTypeDef,
-    AlarmSummaryTypeDef,
-    BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteDetectorErrorEntryTypeDef,
-    DeleteDetectorRequestTypeDef,
-    DisableAlarmActionRequestTypeDef,
-    EnableAlarmActionRequestTypeDef,
-    BatchPutMessageErrorEntryTypeDef,
-    ResetAlarmActionRequestTypeDef,
-    SnoozeAlarmActionRequestTypeDef,
-    BatchUpdateDetectorErrorEntryTypeDef,
-    BlobTypeDef,
-    DisableActionConfigurationTypeDef,
-    EnableActionConfigurationTypeDef,
-    ResetActionConfigurationTypeDef,
-    SnoozeActionConfigurationTypeDef,
-    DescribeAlarmRequestRequestTypeDef,
-    DescribeDetectorRequestRequestTypeDef,
-    TimerDefinitionTypeDef,
-    VariableDefinitionTypeDef,
-    DetectorStateSummaryTypeDef,
-    TimerTypeDef,
-    VariableTypeDef,
-    ListAlarmsRequestRequestTypeDef,
-    ListDetectorsRequestRequestTypeDef,
-    TimestampValueTypeDef,
-    SimpleRuleEvaluationTypeDef,
-    StateChangeConfigurationTypeDef,
-    BatchAcknowledgeAlarmRequestRequestTypeDef,
-    BatchAcknowledgeAlarmResponseTypeDef,
-    BatchDisableAlarmResponseTypeDef,
-    BatchEnableAlarmResponseTypeDef,
-    BatchResetAlarmResponseTypeDef,
-    BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
-    BatchDeleteDetectorResponseTypeDef,
-    BatchDeleteDetectorRequestRequestTypeDef,
-    BatchDisableAlarmRequestRequestTypeDef,
-    BatchEnableAlarmRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchResetAlarmRequestRequestTypeDef,
-    BatchSnoozeAlarmRequestRequestTypeDef,
-    BatchUpdateDetectorResponseTypeDef,
-    CustomerActionTypeDef,
-    DetectorStateDefinitionTypeDef,
-    DetectorSummaryTypeDef,
-    DetectorStateTypeDef,
-    MessageTypeDef,
-    RuleEvaluationTypeDef,
-    SystemEventTypeDef,
-    UpdateDetectorRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    DetectorTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    AlarmStateTypeDef,
-    BatchUpdateDetectorRequestRequestTypeDef,
-    DescribeDetectorResponseTypeDef,
-    AlarmTypeDef,
-    DescribeAlarmResponseTypeDef,
-)
+from types_aiobotocore_iotevents_data.type_defs import AcknowledgeActionConfigurationTypeDef
 
 
 def get_value() -> AcknowledgeActionConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/README.md` & `types-aiobotocore-iotevents-data-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-iotevents-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTEventsData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore iotevents-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotevents-data"></a>
 
 # types-aiobotocore-iotevents-data
 
 [![PyPI - types-aiobotocore-iotevents-data](https://img.shields.io/pypi/v/types-aiobotocore-iotevents-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/)
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
 [types-aiobotocore-iotevents-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,103 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotevents_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTEventsData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/literals/).
+
 ```python
-from types_aiobotocore_iotevents_data.literals import (
-    AlarmStateNameType,
-    ComparisonOperatorType,
-    CustomerActionNameType,
-    ErrorCodeType,
-    EventTypeType,
-    TriggerTypeType,
-    IoTEventsDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_iotevents_data.literals import AlarmStateNameType
 
 
 def check_value(value: AlarmStateNameType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotevents_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTEventsData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/type_defs/).
+
 ```python
-from types_aiobotocore_iotevents_data.type_defs import (
-    AcknowledgeActionConfigurationTypeDef,
-    AcknowledgeAlarmActionRequestTypeDef,
-    AlarmSummaryTypeDef,
-    BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteDetectorErrorEntryTypeDef,
-    DeleteDetectorRequestTypeDef,
-    DisableAlarmActionRequestTypeDef,
-    EnableAlarmActionRequestTypeDef,
-    BatchPutMessageErrorEntryTypeDef,
-    ResetAlarmActionRequestTypeDef,
-    SnoozeAlarmActionRequestTypeDef,
-    BatchUpdateDetectorErrorEntryTypeDef,
-    BlobTypeDef,
-    DisableActionConfigurationTypeDef,
-    EnableActionConfigurationTypeDef,
-    ResetActionConfigurationTypeDef,
-    SnoozeActionConfigurationTypeDef,
-    DescribeAlarmRequestRequestTypeDef,
-    DescribeDetectorRequestRequestTypeDef,
-    TimerDefinitionTypeDef,
-    VariableDefinitionTypeDef,
-    DetectorStateSummaryTypeDef,
-    TimerTypeDef,
-    VariableTypeDef,
-    ListAlarmsRequestRequestTypeDef,
-    ListDetectorsRequestRequestTypeDef,
-    TimestampValueTypeDef,
-    SimpleRuleEvaluationTypeDef,
-    StateChangeConfigurationTypeDef,
-    BatchAcknowledgeAlarmRequestRequestTypeDef,
-    BatchAcknowledgeAlarmResponseTypeDef,
-    BatchDisableAlarmResponseTypeDef,
-    BatchEnableAlarmResponseTypeDef,
-    BatchResetAlarmResponseTypeDef,
-    BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
-    BatchDeleteDetectorResponseTypeDef,
-    BatchDeleteDetectorRequestRequestTypeDef,
-    BatchDisableAlarmRequestRequestTypeDef,
-    BatchEnableAlarmRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchResetAlarmRequestRequestTypeDef,
-    BatchSnoozeAlarmRequestRequestTypeDef,
-    BatchUpdateDetectorResponseTypeDef,
-    CustomerActionTypeDef,
-    DetectorStateDefinitionTypeDef,
-    DetectorSummaryTypeDef,
-    DetectorStateTypeDef,
-    MessageTypeDef,
-    RuleEvaluationTypeDef,
-    SystemEventTypeDef,
-    UpdateDetectorRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    DetectorTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    AlarmStateTypeDef,
-    BatchUpdateDetectorRequestRequestTypeDef,
-    DescribeDetectorResponseTypeDef,
-    AlarmTypeDef,
-    DescribeAlarmResponseTypeDef,
-)
+from types_aiobotocore_iotevents_data.type_defs import AcknowledgeActionConfigurationTypeDef
 
 
 def get_value() -> AcknowledgeActionConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/setup.py` & `types-aiobotocore-iotevents-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotevents_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTEventsData 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/client.py` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/client.pyi` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/literals.py` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
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
@@ -163,14 +164,15 @@
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
@@ -249,26 +251,28 @@
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

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/literals.pyi` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
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
@@ -161,14 +162,15 @@
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
@@ -247,26 +249,28 @@
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

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/type_defs.py` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data/type_defs.pyi` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/PKG-INFO` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTEventsData 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTEventsData 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/
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
 [types-aiobotocore-iotevents-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,103 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotevents_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTEventsData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/literals/).
+
 ```python
-from types_aiobotocore_iotevents_data.literals import (
-    AlarmStateNameType,
-    ComparisonOperatorType,
-    CustomerActionNameType,
-    ErrorCodeType,
-    EventTypeType,
-    TriggerTypeType,
-    IoTEventsDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_iotevents_data.literals import AlarmStateNameType
 
 
 def check_value(value: AlarmStateNameType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotevents_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTEventsData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents_data/type_defs/).
+
 ```python
-from types_aiobotocore_iotevents_data.type_defs import (
-    AcknowledgeActionConfigurationTypeDef,
-    AcknowledgeAlarmActionRequestTypeDef,
-    AlarmSummaryTypeDef,
-    BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteDetectorErrorEntryTypeDef,
-    DeleteDetectorRequestTypeDef,
-    DisableAlarmActionRequestTypeDef,
-    EnableAlarmActionRequestTypeDef,
-    BatchPutMessageErrorEntryTypeDef,
-    ResetAlarmActionRequestTypeDef,
-    SnoozeAlarmActionRequestTypeDef,
-    BatchUpdateDetectorErrorEntryTypeDef,
-    BlobTypeDef,
-    DisableActionConfigurationTypeDef,
-    EnableActionConfigurationTypeDef,
-    ResetActionConfigurationTypeDef,
-    SnoozeActionConfigurationTypeDef,
-    DescribeAlarmRequestRequestTypeDef,
-    DescribeDetectorRequestRequestTypeDef,
-    TimerDefinitionTypeDef,
-    VariableDefinitionTypeDef,
-    DetectorStateSummaryTypeDef,
-    TimerTypeDef,
-    VariableTypeDef,
-    ListAlarmsRequestRequestTypeDef,
-    ListDetectorsRequestRequestTypeDef,
-    TimestampValueTypeDef,
-    SimpleRuleEvaluationTypeDef,
-    StateChangeConfigurationTypeDef,
-    BatchAcknowledgeAlarmRequestRequestTypeDef,
-    BatchAcknowledgeAlarmResponseTypeDef,
-    BatchDisableAlarmResponseTypeDef,
-    BatchEnableAlarmResponseTypeDef,
-    BatchResetAlarmResponseTypeDef,
-    BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
-    BatchDeleteDetectorResponseTypeDef,
-    BatchDeleteDetectorRequestRequestTypeDef,
-    BatchDisableAlarmRequestRequestTypeDef,
-    BatchEnableAlarmRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchResetAlarmRequestRequestTypeDef,
-    BatchSnoozeAlarmRequestRequestTypeDef,
-    BatchUpdateDetectorResponseTypeDef,
-    CustomerActionTypeDef,
-    DetectorStateDefinitionTypeDef,
-    DetectorSummaryTypeDef,
-    DetectorStateTypeDef,
-    MessageTypeDef,
-    RuleEvaluationTypeDef,
-    SystemEventTypeDef,
-    UpdateDetectorRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    DetectorTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    AlarmStateTypeDef,
-    BatchUpdateDetectorRequestRequestTypeDef,
-    DescribeDetectorResponseTypeDef,
-    AlarmTypeDef,
-    DescribeAlarmResponseTypeDef,
-)
+from types_aiobotocore_iotevents_data.type_defs import AcknowledgeActionConfigurationTypeDef
 
 
 def get_value() -> AcknowledgeActionConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotevents-data-2.5.2.post1/types_aiobotocore_iotevents_data.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-data-2.5.2.post2/types_aiobotocore_iotevents_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

