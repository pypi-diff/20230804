# Comparing `tmp/types-aiobotocore-translate-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-translate-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-translate-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-translate-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-translate-2.5.2.post1.tar` & `types-aiobotocore-translate-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-08-02 14:50:46.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-08-02 14:50:46.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:45.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.617432 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:53:08.000000 types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11497 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      681 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      680 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18162 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18133 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9061 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9059 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2041 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2038 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20212 2023-08-04 13:55:22.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20193 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-translate-2.5.2.post1/LICENSE` & `types-aiobotocore-translate-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/PKG-INFO` & `types-aiobotocore-translate-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,109 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_translate.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Translate` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/literals/).
+
 ```python
-from types_aiobotocore_translate.literals import (
-    DirectionalityType,
-    DisplayLanguageCodeType,
-    EncryptionKeyTypeType,
-    FormalityType,
-    JobStatusType,
-    ListTerminologiesPaginatorName,
-    MergeStrategyType,
-    ParallelDataFormatType,
-    ParallelDataStatusType,
-    ProfanityType,
-    TerminologyDataFormatType,
-    TranslateServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_translate.literals import DirectionalityType
 
 
 def check_value(value: DirectionalityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_translate.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Translate` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/type_defs/).
+
 ```python
-from types_aiobotocore_translate.type_defs import (
-    TermTypeDef,
-    BlobTypeDef,
-    EncryptionKeyTypeDef,
-    ParallelDataConfigTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteParallelDataRequestRequestTypeDef,
-    DeleteTerminologyRequestRequestTypeDef,
-    DescribeTextTranslationJobRequestRequestTypeDef,
-    GetParallelDataRequestRequestTypeDef,
-    ParallelDataDataLocationTypeDef,
-    GetTerminologyRequestRequestTypeDef,
-    TerminologyDataLocationTypeDef,
-    InputDataConfigTypeDef,
-    JobDetailsTypeDef,
-    LanguageTypeDef,
-    ListLanguagesRequestRequestTypeDef,
-    ListParallelDataRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTerminologiesRequestRequestTypeDef,
-    TranslationSettingsTypeDef,
-    StopTextTranslationJobRequestRequestTypeDef,
-    TimestampTypeDef,
-    TranslatedDocumentTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AppliedTerminologyTypeDef,
-    DocumentTypeDef,
-    TerminologyDataTypeDef,
-    OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
-    UpdateParallelDataRequestRequestTypeDef,
-    CreateParallelDataRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
-    ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
-    TranslateTextRequestRequestTypeDef,
-    TextTranslationJobFilterTypeDef,
-    TranslateDocumentResponseTypeDef,
-    TranslateTextResponseTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
-    ImportTerminologyRequestRequestTypeDef,
-    StartTextTranslationJobRequestRequestTypeDef,
-    TextTranslationJobPropertiesTypeDef,
-    GetTerminologyResponseTypeDef,
-    ImportTerminologyResponseTypeDef,
-    ListTerminologiesResponseTypeDef,
-    GetParallelDataResponseTypeDef,
-    ListParallelDataResponseTypeDef,
-    ListTextTranslationJobsRequestRequestTypeDef,
-    DescribeTextTranslationJobResponseTypeDef,
-    ListTextTranslationJobsResponseTypeDef,
-)
+from types_aiobotocore_translate.type_defs import TermTypeDef
 
 
 def get_value() -> TermTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-translate-2.5.2.post1/README.md` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-translate
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore translate type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,109 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_translate.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Translate` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/literals/).
+
 ```python
-from types_aiobotocore_translate.literals import (
-    DirectionalityType,
-    DisplayLanguageCodeType,
-    EncryptionKeyTypeType,
-    FormalityType,
-    JobStatusType,
-    ListTerminologiesPaginatorName,
-    MergeStrategyType,
-    ParallelDataFormatType,
-    ParallelDataStatusType,
-    ProfanityType,
-    TerminologyDataFormatType,
-    TranslateServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_translate.literals import DirectionalityType
 
 
 def check_value(value: DirectionalityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_translate.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Translate` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/type_defs/).
+
 ```python
-from types_aiobotocore_translate.type_defs import (
-    TermTypeDef,
-    BlobTypeDef,
-    EncryptionKeyTypeDef,
-    ParallelDataConfigTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteParallelDataRequestRequestTypeDef,
-    DeleteTerminologyRequestRequestTypeDef,
-    DescribeTextTranslationJobRequestRequestTypeDef,
-    GetParallelDataRequestRequestTypeDef,
-    ParallelDataDataLocationTypeDef,
-    GetTerminologyRequestRequestTypeDef,
-    TerminologyDataLocationTypeDef,
-    InputDataConfigTypeDef,
-    JobDetailsTypeDef,
-    LanguageTypeDef,
-    ListLanguagesRequestRequestTypeDef,
-    ListParallelDataRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTerminologiesRequestRequestTypeDef,
-    TranslationSettingsTypeDef,
-    StopTextTranslationJobRequestRequestTypeDef,
-    TimestampTypeDef,
-    TranslatedDocumentTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AppliedTerminologyTypeDef,
-    DocumentTypeDef,
-    TerminologyDataTypeDef,
-    OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
-    UpdateParallelDataRequestRequestTypeDef,
-    CreateParallelDataRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
-    ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
-    TranslateTextRequestRequestTypeDef,
-    TextTranslationJobFilterTypeDef,
-    TranslateDocumentResponseTypeDef,
-    TranslateTextResponseTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
-    ImportTerminologyRequestRequestTypeDef,
-    StartTextTranslationJobRequestRequestTypeDef,
-    TextTranslationJobPropertiesTypeDef,
-    GetTerminologyResponseTypeDef,
-    ImportTerminologyResponseTypeDef,
-    ListTerminologiesResponseTypeDef,
-    GetParallelDataResponseTypeDef,
-    ListParallelDataResponseTypeDef,
-    ListTextTranslationJobsRequestRequestTypeDef,
-    DescribeTextTranslationJobResponseTypeDef,
-    ListTextTranslationJobsResponseTypeDef,
-)
+from types_aiobotocore_translate.type_defs import TermTypeDef
 
 
 def get_value() -> TermTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-translate-2.5.2.post1/setup.py` & `types-aiobotocore-translate-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-translate",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__init__.pyi` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/__main__.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Translate 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Translate 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
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

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/client.pyi` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -173,14 +174,15 @@
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
@@ -259,26 +261,28 @@
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

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/literals.pyi` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -171,14 +172,15 @@
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
@@ -257,26 +259,28 @@
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

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/paginator.pyi` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.py` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate/type_defs.pyi` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post1/types_aiobotocore_translate.egg-info/SOURCES.txt` & `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

