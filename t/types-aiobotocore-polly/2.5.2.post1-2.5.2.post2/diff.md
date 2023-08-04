# Comparing `tmp/types-aiobotocore-polly-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-polly-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-polly-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-polly-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-polly-2.5.2.post1.tar` & `types-aiobotocore-polly-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:45:02.000000 types-aiobotocore-polly-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.625493 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13130 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11620 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.746643 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1087 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12645 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12624 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10758 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10756 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4382 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4377 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8921 2023-08-04 13:47:06.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8916 2023-08-04 13:47:06.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.746643 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13130 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-polly-2.5.2.post1/LICENSE` & `types-aiobotocore-polly-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/PKG-INFO` & `types-aiobotocore-polly-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,75 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_polly.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Polly` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/literals/).
+
 ```python
-from types_aiobotocore_polly.literals import (
-    DescribeVoicesPaginatorName,
-    EngineType,
-    GenderType,
-    LanguageCodeType,
-    ListLexiconsPaginatorName,
-    ListSpeechSynthesisTasksPaginatorName,
-    OutputFormatType,
-    SpeechMarkTypeType,
-    TaskStatusType,
-    TextTypeType,
-    VoiceIdType,
-    PollyServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_polly.literals import DescribeVoicesPaginatorName
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Polly` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/type_defs/).
+
 ```python
-from types_aiobotocore_polly.type_defs import (
-    DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VoiceTypeDef,
-    GetLexiconInputRequestTypeDef,
-    LexiconAttributesTypeDef,
-    LexiconTypeDef,
-    GetSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesisTaskTypeDef,
-    ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputRequestTypeDef,
-    PutLexiconInputRequestTypeDef,
-    StartSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
-    SynthesizeSpeechOutputTypeDef,
-    DescribeVoicesOutputTypeDef,
-    LexiconDescriptionTypeDef,
-    GetLexiconOutputTypeDef,
-    GetSpeechSynthesisTaskOutputTypeDef,
-    ListSpeechSynthesisTasksOutputTypeDef,
-    StartSpeechSynthesisTaskOutputTypeDef,
-    ListLexiconsOutputTypeDef,
-)
+from types_aiobotocore_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
 
 def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-polly-2.5.2.post1/README.md` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-polly
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore polly type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,75 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_polly.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Polly` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/literals/).
+
 ```python
-from types_aiobotocore_polly.literals import (
-    DescribeVoicesPaginatorName,
-    EngineType,
-    GenderType,
-    LanguageCodeType,
-    ListLexiconsPaginatorName,
-    ListSpeechSynthesisTasksPaginatorName,
-    OutputFormatType,
-    SpeechMarkTypeType,
-    TaskStatusType,
-    TextTypeType,
-    VoiceIdType,
-    PollyServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_polly.literals import DescribeVoicesPaginatorName
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Polly` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/type_defs/).
+
 ```python
-from types_aiobotocore_polly.type_defs import (
-    DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VoiceTypeDef,
-    GetLexiconInputRequestTypeDef,
-    LexiconAttributesTypeDef,
-    LexiconTypeDef,
-    GetSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesisTaskTypeDef,
-    ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputRequestTypeDef,
-    PutLexiconInputRequestTypeDef,
-    StartSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
-    SynthesizeSpeechOutputTypeDef,
-    DescribeVoicesOutputTypeDef,
-    LexiconDescriptionTypeDef,
-    GetLexiconOutputTypeDef,
-    GetSpeechSynthesisTaskOutputTypeDef,
-    ListSpeechSynthesisTasksOutputTypeDef,
-    StartSpeechSynthesisTaskOutputTypeDef,
-    ListLexiconsOutputTypeDef,
-)
+from types_aiobotocore_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
 
 def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-polly-2.5.2.post1/setup.py` & `types-aiobotocore-polly-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-polly",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.pyi` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__main__.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.pyi` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeVoicesPaginatorName",
     "EngineType",
     "GenderType",
     "LanguageCodeType",
     "ListLexiconsPaginatorName",
     "ListSpeechSynthesisTasksPaginatorName",
@@ -34,15 +33,14 @@
     "PollyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeVoicesPaginatorName = Literal["describe_voices"]
 EngineType = Literal["neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
@@ -59,22 +57,24 @@
     "en-NZ",
     "en-US",
     "en-ZA",
     "es-ES",
     "es-MX",
     "es-US",
     "fi-FI",
+    "fr-BE",
     "fr-CA",
     "fr-FR",
     "hi-IN",
     "is-IS",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "nb-NO",
+    "nl-BE",
     "nl-NL",
     "pl-PL",
     "pt-BR",
     "pt-PT",
     "ro-RO",
     "ru-RU",
     "sv-SE",
@@ -119,14 +119,15 @@
     "Gwyneth",
     "Hala",
     "Hannah",
     "Hans",
     "Hiujin",
     "Ida",
     "Ines",
+    "Isabelle",
     "Ivy",
     "Jacek",
     "Jan",
     "Joanna",
     "Joey",
     "Justin",
     "Kajal",
@@ -134,14 +135,15 @@
     "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
+    "Lisa",
     "Liv",
     "Lotte",
     "Lucia",
     "Lupe",
     "Mads",
     "Maja",
     "Marlene",
@@ -191,14 +193,15 @@
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
@@ -294,14 +297,15 @@
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
@@ -380,26 +384,28 @@
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

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.pyi` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeVoicesPaginatorName",
     "EngineType",
     "GenderType",
     "LanguageCodeType",
     "ListLexiconsPaginatorName",
     "ListSpeechSynthesisTasksPaginatorName",
@@ -33,14 +34,15 @@
     "PollyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeVoicesPaginatorName = Literal["describe_voices"]
 EngineType = Literal["neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
@@ -57,22 +59,24 @@
     "en-NZ",
     "en-US",
     "en-ZA",
     "es-ES",
     "es-MX",
     "es-US",
     "fi-FI",
+    "fr-BE",
     "fr-CA",
     "fr-FR",
     "hi-IN",
     "is-IS",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "nb-NO",
+    "nl-BE",
     "nl-NL",
     "pl-PL",
     "pt-BR",
     "pt-PT",
     "ro-RO",
     "ru-RU",
     "sv-SE",
@@ -117,14 +121,15 @@
     "Gwyneth",
     "Hala",
     "Hannah",
     "Hans",
     "Hiujin",
     "Ida",
     "Ines",
+    "Isabelle",
     "Ivy",
     "Jacek",
     "Jan",
     "Joanna",
     "Joey",
     "Justin",
     "Kajal",
@@ -132,14 +137,15 @@
     "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
+    "Lisa",
     "Liv",
     "Lotte",
     "Lucia",
     "Lupe",
     "Mads",
     "Maja",
     "Marlene",
@@ -189,14 +195,15 @@
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
@@ -292,14 +299,15 @@
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
@@ -378,26 +386,28 @@
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

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.pyi` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.py` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.pyi` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/PKG-INFO` & `types-aiobotocore-polly-2.5.2.post2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-polly
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore polly type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,75 +263,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_polly.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Polly` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/literals/).
+
 ```python
-from types_aiobotocore_polly.literals import (
-    DescribeVoicesPaginatorName,
-    EngineType,
-    GenderType,
-    LanguageCodeType,
-    ListLexiconsPaginatorName,
-    ListSpeechSynthesisTasksPaginatorName,
-    OutputFormatType,
-    SpeechMarkTypeType,
-    TaskStatusType,
-    TextTypeType,
-    VoiceIdType,
-    PollyServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_polly.literals import DescribeVoicesPaginatorName
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Polly` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/type_defs/).
+
 ```python
-from types_aiobotocore_polly.type_defs import (
-    DeleteLexiconInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeVoicesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    VoiceTypeDef,
-    GetLexiconInputRequestTypeDef,
-    LexiconAttributesTypeDef,
-    LexiconTypeDef,
-    GetSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesisTaskTypeDef,
-    ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputRequestTypeDef,
-    PutLexiconInputRequestTypeDef,
-    StartSpeechSynthesisTaskInputRequestTypeDef,
-    SynthesizeSpeechInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
-    SynthesizeSpeechOutputTypeDef,
-    DescribeVoicesOutputTypeDef,
-    LexiconDescriptionTypeDef,
-    GetLexiconOutputTypeDef,
-    GetSpeechSynthesisTaskOutputTypeDef,
-    ListSpeechSynthesisTasksOutputTypeDef,
-    StartSpeechSynthesisTaskOutputTypeDef,
-    ListLexiconsOutputTypeDef,
-)
+from types_aiobotocore_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
 
 def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/SOURCES.txt` & `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

