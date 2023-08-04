# Comparing `tmp/types-aiobotocore-dlm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dlm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dlm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-dlm-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:46 2023, max compression
```

## Comparing `types-aiobotocore-dlm-2.5.2.post1.tar` & `types-aiobotocore-dlm-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.697602 types-aiobotocore-dlm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.697602 types-aiobotocore-dlm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-08-02 14:36:29.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-08-02 14:36:29.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:28.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.685602 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:46.443916 types-aiobotocore-dlm-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:00:46.443916 types-aiobotocore-dlm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:46.443916 types-aiobotocore-dlm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:46.439916 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-08-04 11:43:50.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-04 11:43:50.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-08-04 11:43:50.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-08-04 11:43:50.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-08-04 11:43:50.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:49.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:46.443916 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:46.000000 types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dlm-2.5.2.post1/LICENSE` & `types-aiobotocore-dlm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post1/PKG-INFO` & `types-aiobotocore-dlm-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,92 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dlm.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `DLM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/literals/).
+
 ```python
-from types_aiobotocore_dlm.literals import (
-    EventSourceValuesType,
-    EventTypeValuesType,
-    GettablePolicyStateValuesType,
-    IntervalUnitValuesType,
-    LocationValuesType,
-    PolicyTypeValuesType,
-    ResourceLocationValuesType,
-    ResourceTypeValuesType,
-    RetentionIntervalUnitValuesType,
-    SettablePolicyStateValuesType,
-    DLMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_dlm.literals import EventSourceValuesType
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dlm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DLM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/type_defs/).
+
 ```python
-from types_aiobotocore_dlm.type_defs import (
-    RetentionArchiveTierTypeDef,
-    ResponseMetadataTypeDef,
-    CreateRuleOutputTypeDef,
-    CreateRuleTypeDef,
-    CrossRegionCopyRetainRuleTypeDef,
-    EncryptionConfigurationTypeDef,
-    CrossRegionCopyDeprecateRuleTypeDef,
-    DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeprecateRuleTypeDef,
-    EventParametersOutputTypeDef,
-    EventParametersTypeDef,
-    FastRestoreRuleOutputTypeDef,
-    FastRestoreRuleTypeDef,
-    GetLifecyclePoliciesRequestRequestTypeDef,
-    LifecyclePolicySummaryTypeDef,
-    GetLifecyclePolicyRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    RetainRuleTypeDef,
-    ShareRuleOutputTypeDef,
-    ShareRuleTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ArchiveRetainRuleTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CrossRegionCopyActionTypeDef,
-    CrossRegionCopyRuleTypeDef,
-    EventSourceOutputTypeDef,
-    EventSourceTypeDef,
-    GetLifecyclePoliciesResponseTypeDef,
-    ParametersOutputTypeDef,
-    ParametersTypeDef,
-    ArchiveRuleTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ScheduleOutputTypeDef,
-    ScheduleTypeDef,
-    PolicyDetailsOutputTypeDef,
-    PolicyDetailsTypeDef,
-    LifecyclePolicyTypeDef,
-    CreateLifecyclePolicyRequestRequestTypeDef,
-    PolicyDetailsUnionTypeDef,
-    UpdateLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-)
+from types_aiobotocore_dlm.type_defs import RetentionArchiveTierTypeDef
 
 
 def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dlm-2.5.2.post1/README.md` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-dlm
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore dlm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dlm"></a>
 
 # types-aiobotocore-dlm
 
 [![PyPI - types-aiobotocore-dlm](https://img.shields.io/pypi/v/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
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
 [types-aiobotocore-dlm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -232,92 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dlm.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `DLM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/literals/).
+
 ```python
-from types_aiobotocore_dlm.literals import (
-    EventSourceValuesType,
-    EventTypeValuesType,
-    GettablePolicyStateValuesType,
-    IntervalUnitValuesType,
-    LocationValuesType,
-    PolicyTypeValuesType,
-    ResourceLocationValuesType,
-    ResourceTypeValuesType,
-    RetentionIntervalUnitValuesType,
-    SettablePolicyStateValuesType,
-    DLMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_dlm.literals import EventSourceValuesType
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dlm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DLM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/type_defs/).
+
 ```python
-from types_aiobotocore_dlm.type_defs import (
-    RetentionArchiveTierTypeDef,
-    ResponseMetadataTypeDef,
-    CreateRuleOutputTypeDef,
-    CreateRuleTypeDef,
-    CrossRegionCopyRetainRuleTypeDef,
-    EncryptionConfigurationTypeDef,
-    CrossRegionCopyDeprecateRuleTypeDef,
-    DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeprecateRuleTypeDef,
-    EventParametersOutputTypeDef,
-    EventParametersTypeDef,
-    FastRestoreRuleOutputTypeDef,
-    FastRestoreRuleTypeDef,
-    GetLifecyclePoliciesRequestRequestTypeDef,
-    LifecyclePolicySummaryTypeDef,
-    GetLifecyclePolicyRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    RetainRuleTypeDef,
-    ShareRuleOutputTypeDef,
-    ShareRuleTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ArchiveRetainRuleTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CrossRegionCopyActionTypeDef,
-    CrossRegionCopyRuleTypeDef,
-    EventSourceOutputTypeDef,
-    EventSourceTypeDef,
-    GetLifecyclePoliciesResponseTypeDef,
-    ParametersOutputTypeDef,
-    ParametersTypeDef,
-    ArchiveRuleTypeDef,
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ScheduleOutputTypeDef,
-    ScheduleTypeDef,
-    PolicyDetailsOutputTypeDef,
-    PolicyDetailsTypeDef,
-    LifecyclePolicyTypeDef,
-    CreateLifecyclePolicyRequestRequestTypeDef,
-    PolicyDetailsUnionTypeDef,
-    UpdateLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-)
+from types_aiobotocore_dlm.type_defs import RetentionArchiveTierTypeDef
 
 
 def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dlm-2.5.2.post1/setup.py` & `types-aiobotocore-dlm-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dlm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/__main__.py` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DLM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DLM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.py` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsUnionTypeDef,
+    PolicyDetailsTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -86,15 +86,15 @@
 
     async def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsUnionTypeDef,
+        PolicyDetails: PolicyDetailsTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -177,15 +177,15 @@
     async def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsUnionTypeDef = ...
+        PolicyDetails: PolicyDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/client.pyi` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsUnionTypeDef,
+    PolicyDetailsTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -80,15 +80,15 @@
         """
     async def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: PolicyDetailsUnionTypeDef,
+        PolicyDetails: PolicyDetailsTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -163,15 +163,15 @@
     async def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: PolicyDetailsUnionTypeDef = ...
+        PolicyDetails: PolicyDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.py` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm/literals.pyi` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post1/types_aiobotocore_dlm.egg-info/SOURCES.txt` & `types-aiobotocore-dlm-2.5.2.post2/types_aiobotocore_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

