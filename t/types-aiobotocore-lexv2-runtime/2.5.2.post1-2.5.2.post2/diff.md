# Comparing `tmp/types-aiobotocore-lexv2-runtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lexv2-runtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lexv2-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lexv2-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1.tar` & `types-aiobotocore-lexv2-runtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.669542 types-aiobotocore-lexv2-runtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.669542 types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-08-02 14:42:11.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-08-02 14:42:11.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.216643 types-aiobotocore-lexv2-runtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12521 2023-08-04 13:59:15.216643 types-aiobotocore-lexv2-runtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10980 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.216643 types-aiobotocore-lexv2-runtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2113 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.206643 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      485 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      484 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8002 2023-08-04 13:42:55.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7989 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8672 2023-08-04 13:42:55.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8670 2023-08-04 13:42:55.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11377 2023-08-04 13:42:55.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11356 2023-08-04 13:42:55.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:54.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.216643 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12521 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      836 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:15.000000 types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/LICENSE` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,86 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lexv2_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeV2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/literals/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.literals import (
-    ConfirmationStateType,
-    DialogActionTypeType,
-    IntentStateType,
-    MessageContentTypeType,
-    SentimentTypeType,
-    ShapeType,
-    StyleTypeType,
-    LexRuntimeV2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lexv2_runtime.literals import ConfirmationStateType
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeV2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    ConfidenceScoreTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionTypeDef,
-    ElicitSubSlotTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentOutputTypeDef,
-    IntentTypeDef,
-    RecognizedBotMemberTypeDef,
-    RuntimeHintValueTypeDef,
-    RuntimeHintsOutputTypeDef,
-    RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueOutputTypeDef,
-    ValueTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    SentimentResponseTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    SessionStateUnionTypeDef,
-    MessageUnionTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
-    PutSessionRequestRequestTypeDef,
-)
+from types_aiobotocore_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/README.md` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-lexv2-runtime
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore lexv2-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-runtime"></a>
 
 # types-aiobotocore-lexv2-runtime
 
 [![PyPI - types-aiobotocore-lexv2-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/)
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,86 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lexv2_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeV2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/literals/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.literals import (
-    ConfirmationStateType,
-    DialogActionTypeType,
-    IntentStateType,
-    MessageContentTypeType,
-    SentimentTypeType,
-    ShapeType,
-    StyleTypeType,
-    LexRuntimeV2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lexv2_runtime.literals import ConfirmationStateType
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeV2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    ConfidenceScoreTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionTypeDef,
-    ElicitSubSlotTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentOutputTypeDef,
-    IntentTypeDef,
-    RecognizedBotMemberTypeDef,
-    RuntimeHintValueTypeDef,
-    RuntimeHintsOutputTypeDef,
-    RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueOutputTypeDef,
-    ValueTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    SentimentResponseTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    SessionStateUnionTypeDef,
-    MessageUnionTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
-    PutSessionRequestRequestTypeDef,
-)
+from types_aiobotocore_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lexv2-runtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__main__.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.LexRuntimeV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2\nOther"
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

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageUnionTypeDef,
+    MessageTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateUnionTypeDef,
+    SessionStateTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -123,16 +123,16 @@
     async def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateUnionTypeDef,
-        messages: Sequence[MessageUnionTypeDef] = ...,
+        sessionState: SessionStateTypeDef,
+        messages: Sequence[MessageTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -143,15 +143,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateUnionTypeDef = ...,
+        sessionState: SessionStateTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_text)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageUnionTypeDef,
+    MessageTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateUnionTypeDef,
+    SessionStateTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -114,16 +114,16 @@
     async def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateUnionTypeDef,
-        messages: Sequence[MessageUnionTypeDef] = ...,
+        sessionState: SessionStateTypeDef,
+        messages: Sequence[MessageTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -133,15 +133,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateUnionTypeDef = ...,
+        sessionState: SessionStateTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_text)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -160,14 +161,15 @@
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
@@ -246,26 +248,28 @@
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

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -158,14 +159,15 @@
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
@@ -244,26 +246,28 @@
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

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,47 +38,36 @@
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentOutputTypeDef",
     "IntentTypeDef",
     "RecognizedBotMemberTypeDef",
     "RuntimeHintValueTypeDef",
-    "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
-    "ValueOutputTypeDef",
     "ValueTypeDef",
-    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "RecognizeUtteranceRequestRequestTypeDef",
-    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "DeleteSessionResponseTypeDef",
     "PutSessionResponseTypeDef",
     "RecognizeUtteranceResponseTypeDef",
-    "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
-    "SlotOutputTypeDef",
     "SlotTypeDef",
-    "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "SessionStateUnionTypeDef",
-    "MessageUnionTypeDef",
+    "PutSessionRequestRequestTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
-    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
@@ -169,45 +158,24 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-_RequiredIntentOutputTypeDef = TypedDict(
-    "_RequiredIntentOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalIntentOutputTypeDef = TypedDict(
-    "_OptionalIntentOutputTypeDef",
-    {
-        "slots": Dict[str, "SlotOutputTypeDef"],
-        "state": IntentStateType,
-        "confirmationState": ConfirmationStateType,
-    },
-    total=False,
-)
-
-
-class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
-    pass
-
-
 _RequiredIntentTypeDef = TypedDict(
     "_RequiredIntentTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentTypeDef = TypedDict(
     "_OptionalIntentTypeDef",
     {
-        "slots": Mapping[str, "SlotTypeDef"],
+        "slots": Dict[str, "SlotTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
 
@@ -239,26 +207,18 @@
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
-RuntimeHintsOutputTypeDef = TypedDict(
-    "RuntimeHintsOutputTypeDef",
-    {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
-    },
-    total=False,
-)
-
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
-        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
     },
     total=False,
 )
 
 SentimentScoreTypeDef = TypedDict(
     "SentimentScoreTypeDef",
     {
@@ -266,69 +226,40 @@
         "negative": float,
         "neutral": float,
         "mixed": float,
     },
     total=False,
 )
 
-_RequiredValueOutputTypeDef = TypedDict(
-    "_RequiredValueOutputTypeDef",
-    {
-        "interpretedValue": str,
-    },
-)
-_OptionalValueOutputTypeDef = TypedDict(
-    "_OptionalValueOutputTypeDef",
-    {
-        "originalValue": str,
-        "resolvedValues": List[str],
-    },
-    total=False,
-)
-
-
-class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
-    pass
-
-
 _RequiredValueTypeDef = TypedDict(
     "_RequiredValueTypeDef",
     {
         "interpretedValue": str,
     },
 )
 _OptionalValueTypeDef = TypedDict(
     "_OptionalValueTypeDef",
     {
         "originalValue": str,
-        "resolvedValues": Sequence[str],
+        "resolvedValues": List[str],
     },
     total=False,
 )
 
 
 class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
 
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Dict[str, str],
-    },
-)
-
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Mapping[str, str],
+        "contextAttributes": Dict[str, str],
     },
 )
 
 _RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeUtteranceRequestRequestTypeDef",
     {
         "botId": str,
@@ -353,49 +284,26 @@
 class RecognizeUtteranceRequestRequestTypeDef(
     _RequiredRecognizeUtteranceRequestRequestTypeDef,
     _OptionalRecognizeUtteranceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
-    pass
-
-
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
     "_OptionalImageResponseCardTypeDef",
     {
         "subtitle": str,
         "imageUrl": str,
-        "buttons": Sequence[ButtonTypeDef],
+        "buttons": List[ButtonTypeDef],
     },
     total=False,
 )
 
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
@@ -440,109 +348,56 @@
         "inputTranscript": str,
         "audioStream": StreamingBody,
         "recognizedBotMember": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuntimeHintDetailsOutputTypeDef = TypedDict(
-    "RuntimeHintDetailsOutputTypeDef",
-    {
-        "runtimeHintValues": List[RuntimeHintValueTypeDef],
-        "subSlotHints": Dict[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
-        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
-        "subSlotHints": Mapping[str, Dict[str, Any]],
+        "runtimeHintValues": List[RuntimeHintValueTypeDef],
+        "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentiment": SentimentTypeType,
         "sentimentScore": SentimentScoreTypeDef,
     },
     total=False,
 )
 
-SlotOutputTypeDef = TypedDict(
-    "SlotOutputTypeDef",
-    {
-        "value": ValueOutputTypeDef,
-        "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
 SlotTypeDef = TypedDict(
     "SlotTypeDef",
     {
         "value": ValueTypeDef,
         "shape": ShapeType,
-        "values": Sequence[Dict[str, Any]],
-        "subSlots": Mapping[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
-SessionStateOutputTypeDef = TypedDict(
-    "SessionStateOutputTypeDef",
-    {
-        "dialogAction": DialogActionTypeDef,
-        "intent": IntentOutputTypeDef,
-        "activeContexts": List[ActiveContextOutputTypeDef],
-        "sessionAttributes": Dict[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": RuntimeHintsOutputTypeDef,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 SessionStateTypeDef = TypedDict(
     "SessionStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentTypeDef,
-        "activeContexts": Sequence[ActiveContextTypeDef],
-        "sessionAttributes": Mapping[str, str],
+        "activeContexts": List[ActiveContextTypeDef],
+        "sessionAttributes": Dict[str, str],
         "originatingRequestId": str,
         "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
-    {
-        "contentType": MessageContentTypeType,
-    },
-)
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
-    {
-        "content": str,
-        "imageResponseCard": ImageResponseCardOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
-    pass
-
-
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": MessageContentTypeType,
     },
 )
 _OptionalMessageTypeDef = TypedDict(
@@ -560,15 +415,15 @@
 
 
 InterpretationTypeDef = TypedDict(
     "InterpretationTypeDef",
     {
         "nluConfidence": ConfidenceScoreTypeDef,
         "sentimentResponse": SentimentResponseTypeDef,
-        "intent": IntentOutputTypeDef,
+        "intent": IntentTypeDef,
     },
     total=False,
 )
 
 _RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeTextRequestRequestTypeDef",
     {
@@ -591,58 +446,57 @@
 
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
 
-SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
-MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List[MessageOutputTypeDef],
-        "interpretations": List[InterpretationTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List[MessageOutputTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "interpretations": List[InterpretationTypeDef],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
         "sessionState": SessionStateTypeDef,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "messages": Sequence[MessageUnionTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "requestAttributes": Mapping[str, str],
         "responseContentType": str,
     },
     total=False,
 )
 
 
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
+
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "sessionState": SessionStateTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -37,47 +37,36 @@
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentOutputTypeDef",
     "IntentTypeDef",
     "RecognizedBotMemberTypeDef",
     "RuntimeHintValueTypeDef",
-    "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
-    "ValueOutputTypeDef",
     "ValueTypeDef",
-    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "RecognizeUtteranceRequestRequestTypeDef",
-    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
     "DeleteSessionResponseTypeDef",
     "PutSessionResponseTypeDef",
     "RecognizeUtteranceResponseTypeDef",
-    "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
-    "SlotOutputTypeDef",
     "SlotTypeDef",
-    "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
-    "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "SessionStateUnionTypeDef",
-    "MessageUnionTypeDef",
+    "PutSessionRequestRequestTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
-    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
@@ -164,43 +153,24 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-_RequiredIntentOutputTypeDef = TypedDict(
-    "_RequiredIntentOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalIntentOutputTypeDef = TypedDict(
-    "_OptionalIntentOutputTypeDef",
-    {
-        "slots": Dict[str, "SlotOutputTypeDef"],
-        "state": IntentStateType,
-        "confirmationState": ConfirmationStateType,
-    },
-    total=False,
-)
-
-class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
-    pass
-
 _RequiredIntentTypeDef = TypedDict(
     "_RequiredIntentTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentTypeDef = TypedDict(
     "_OptionalIntentTypeDef",
     {
-        "slots": Mapping[str, "SlotTypeDef"],
+        "slots": Dict[str, "SlotTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
@@ -228,26 +198,18 @@
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
-RuntimeHintsOutputTypeDef = TypedDict(
-    "RuntimeHintsOutputTypeDef",
-    {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
-    },
-    total=False,
-)
-
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
-        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
     },
     total=False,
 )
 
 SentimentScoreTypeDef = TypedDict(
     "SentimentScoreTypeDef",
     {
@@ -255,65 +217,38 @@
         "negative": float,
         "neutral": float,
         "mixed": float,
     },
     total=False,
 )
 
-_RequiredValueOutputTypeDef = TypedDict(
-    "_RequiredValueOutputTypeDef",
-    {
-        "interpretedValue": str,
-    },
-)
-_OptionalValueOutputTypeDef = TypedDict(
-    "_OptionalValueOutputTypeDef",
-    {
-        "originalValue": str,
-        "resolvedValues": List[str],
-    },
-    total=False,
-)
-
-class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
-    pass
-
 _RequiredValueTypeDef = TypedDict(
     "_RequiredValueTypeDef",
     {
         "interpretedValue": str,
     },
 )
 _OptionalValueTypeDef = TypedDict(
     "_OptionalValueTypeDef",
     {
         "originalValue": str,
-        "resolvedValues": Sequence[str],
+        "resolvedValues": List[str],
     },
     total=False,
 )
 
 class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Dict[str, str],
-    },
-)
-
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Mapping[str, str],
+        "contextAttributes": Dict[str, str],
     },
 )
 
 _RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeUtteranceRequestRequestTypeDef",
     {
         "botId": str,
@@ -336,47 +271,26 @@
 
 class RecognizeUtteranceRequestRequestTypeDef(
     _RequiredRecognizeUtteranceRequestRequestTypeDef,
     _OptionalRecognizeUtteranceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
-    pass
-
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
     "_OptionalImageResponseCardTypeDef",
     {
         "subtitle": str,
         "imageUrl": str,
-        "buttons": Sequence[ButtonTypeDef],
+        "buttons": List[ButtonTypeDef],
     },
     total=False,
 )
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
@@ -419,107 +333,56 @@
         "inputTranscript": str,
         "audioStream": StreamingBody,
         "recognizedBotMember": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuntimeHintDetailsOutputTypeDef = TypedDict(
-    "RuntimeHintDetailsOutputTypeDef",
-    {
-        "runtimeHintValues": List[RuntimeHintValueTypeDef],
-        "subSlotHints": Dict[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
-        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
-        "subSlotHints": Mapping[str, Dict[str, Any]],
+        "runtimeHintValues": List[RuntimeHintValueTypeDef],
+        "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentiment": SentimentTypeType,
         "sentimentScore": SentimentScoreTypeDef,
     },
     total=False,
 )
 
-SlotOutputTypeDef = TypedDict(
-    "SlotOutputTypeDef",
-    {
-        "value": ValueOutputTypeDef,
-        "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
 SlotTypeDef = TypedDict(
     "SlotTypeDef",
     {
         "value": ValueTypeDef,
         "shape": ShapeType,
-        "values": Sequence[Dict[str, Any]],
-        "subSlots": Mapping[str, Dict[str, Any]],
-    },
-    total=False,
-)
-
-SessionStateOutputTypeDef = TypedDict(
-    "SessionStateOutputTypeDef",
-    {
-        "dialogAction": DialogActionTypeDef,
-        "intent": IntentOutputTypeDef,
-        "activeContexts": List[ActiveContextOutputTypeDef],
-        "sessionAttributes": Dict[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": RuntimeHintsOutputTypeDef,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 SessionStateTypeDef = TypedDict(
     "SessionStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentTypeDef,
-        "activeContexts": Sequence[ActiveContextTypeDef],
-        "sessionAttributes": Mapping[str, str],
+        "activeContexts": List[ActiveContextTypeDef],
+        "sessionAttributes": Dict[str, str],
         "originatingRequestId": str,
         "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
-    {
-        "contentType": MessageContentTypeType,
-    },
-)
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
-    {
-        "content": str,
-        "imageResponseCard": ImageResponseCardOutputTypeDef,
-    },
-    total=False,
-)
-
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
-    pass
-
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": MessageContentTypeType,
     },
 )
 _OptionalMessageTypeDef = TypedDict(
@@ -535,15 +398,15 @@
     pass
 
 InterpretationTypeDef = TypedDict(
     "InterpretationTypeDef",
     {
         "nluConfidence": ConfidenceScoreTypeDef,
         "sentimentResponse": SentimentResponseTypeDef,
-        "intent": IntentOutputTypeDef,
+        "intent": IntentTypeDef,
     },
     total=False,
 )
 
 _RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeTextRequestRequestTypeDef",
     {
@@ -564,57 +427,55 @@
 )
 
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
-SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
-MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List[MessageOutputTypeDef],
-        "interpretations": List[InterpretationTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List[MessageOutputTypeDef],
-        "sessionState": SessionStateOutputTypeDef,
-        "interpretations": List[InterpretationTypeDef],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
         "sessionState": SessionStateTypeDef,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "messages": Sequence[MessageUnionTypeDef],
+        "messages": Sequence[MessageTypeDef],
         "requestAttributes": Mapping[str, str],
         "responseContentType": str,
     },
     total=False,
 )
 
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageTypeDef],
+        "sessionState": SessionStateTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-lexv2-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lexv2-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-runtime"></a>
 
 # types-aiobotocore-lexv2-runtime
 
 [![PyPI - types-aiobotocore-lexv2-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/)
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,86 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lexv2_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeV2` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/literals/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.literals import (
-    ConfirmationStateType,
-    DialogActionTypeType,
-    IntentStateType,
-    MessageContentTypeType,
-    SentimentTypeType,
-    ShapeType,
-    StyleTypeType,
-    LexRuntimeV2ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lexv2_runtime.literals import ConfirmationStateType
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeV2` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lexv2_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    ConfidenceScoreTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionTypeDef,
-    ElicitSubSlotTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentOutputTypeDef,
-    IntentTypeDef,
-    RecognizedBotMemberTypeDef,
-    RuntimeHintValueTypeDef,
-    RuntimeHintsOutputTypeDef,
-    RuntimeHintsTypeDef,
-    SentimentScoreTypeDef,
-    ValueOutputTypeDef,
-    ValueTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
-    DeleteSessionResponseTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    SentimentResponseTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    InterpretationTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    SessionStateUnionTypeDef,
-    MessageUnionTypeDef,
-    GetSessionResponseTypeDef,
-    RecognizeTextResponseTypeDef,
-    PutSessionRequestRequestTypeDef,
-)
+from types_aiobotocore_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lexv2-runtime-2.5.2.post2/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

