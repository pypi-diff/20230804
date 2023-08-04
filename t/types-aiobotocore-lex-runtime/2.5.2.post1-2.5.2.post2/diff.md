# Comparing `tmp/types-aiobotocore-lex-runtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lex-runtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lex-runtime-2.5.2.post1.tar` & `types-aiobotocore-lex-runtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-08-02 14:41:53.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-08-02 14:41:53.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12480 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10940 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.176643 types-aiobotocore-lex-runtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      504 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      503 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8265 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8252 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8534 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8532 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9729 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9716 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12480 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/LICENSE` & `types-aiobotocore-lex-runtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,71 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lex_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/literals/).
+
 ```python
-from types_aiobotocore_lex_runtime.literals import (
-    ConfirmationStatusType,
-    ContentTypeType,
-    DialogActionTypeType,
-    DialogStateType,
-    FulfillmentStateType,
-    MessageFormatTypeType,
-    LexRuntimeServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionOutputTypeDef,
-    DialogActionTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentSummaryOutputTypeDef,
-    IntentConfidenceTypeDef,
-    IntentSummaryTypeDef,
-    SentimentResponseTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    PostContentRequestRequestTypeDef,
-    GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    DialogActionUnionTypeDef,
-    PredictedIntentTypeDef,
-    IntentSummaryUnionTypeDef,
-    GetSessionResponseTypeDef,
-    ActiveContextUnionTypeDef,
-    ResponseCardTypeDef,
-    PostTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PostTextResponseTypeDef,
-)
+from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/README.md` & `types-aiobotocore-lex-runtime-2.5.2.post2/README.md`

 * *Files 21% similar despite different names*

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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,71 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lex_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/literals/).
+
 ```python
-from types_aiobotocore_lex_runtime.literals import (
-    ConfirmationStatusType,
-    ContentTypeType,
-    DialogActionTypeType,
-    DialogStateType,
-    FulfillmentStateType,
-    MessageFormatTypeType,
-    LexRuntimeServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionOutputTypeDef,
-    DialogActionTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentSummaryOutputTypeDef,
-    IntentConfidenceTypeDef,
-    IntentSummaryTypeDef,
-    SentimentResponseTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    PostContentRequestRequestTypeDef,
-    GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    DialogActionUnionTypeDef,
-    PredictedIntentTypeDef,
-    IntentSummaryUnionTypeDef,
-    GetSessionResponseTypeDef,
-    ActiveContextUnionTypeDef,
-    ResponseCardTypeDef,
-    PostTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PostTextResponseTypeDef,
-)
+from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/setup.py` & `types-aiobotocore-lex-runtime-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-runtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__main__.py` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LexRuntimeService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.py` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
-    ActiveContextUnionTypeDef,
+    ActiveContextTypeDef,
     BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionUnionTypeDef,
+    DialogActionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryUnionTypeDef,
+    IntentSummaryTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -149,15 +149,15 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
@@ -165,18 +165,18 @@
     async def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: DialogActionUnionTypeDef = ...,
-        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
+        dialogAction: DialogActionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
-    ActiveContextUnionTypeDef,
+    ActiveContextTypeDef,
     BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionUnionTypeDef,
+    DialogActionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryUnionTypeDef,
+    IntentSummaryTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -139,33 +139,33 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
     async def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: DialogActionUnionTypeDef = ...,
-        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
+        dialogAction: DialogActionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.py` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -156,14 +157,15 @@
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
@@ -242,26 +244,28 @@
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -154,14 +155,15 @@
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
@@ -240,26 +242,28 @@
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.py` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,36 +36,30 @@
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryOutputTypeDef",
-    "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
+    "IntentConfidenceTypeDef",
     "SentimentResponseTypeDef",
-    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
     "DeleteSessionResponseTypeDef",
     "PostContentResponseTypeDef",
     "PutSessionResponseTypeDef",
-    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
-    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
-    "ActiveContextUnionTypeDef",
-    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
+    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
@@ -99,51 +93,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredDialogActionOutputTypeDef = TypedDict(
-    "_RequiredDialogActionOutputTypeDef",
-    {
-        "type": DialogActionTypeType,
-    },
-)
-_OptionalDialogActionOutputTypeDef = TypedDict(
-    "_OptionalDialogActionOutputTypeDef",
-    {
-        "intentName": str,
-        "slots": Dict[str, str],
-        "slotToElicit": str,
-        "fulfillmentState": FulfillmentStateType,
-        "message": str,
-        "messageFormat": MessageFormatTypeType,
-    },
-    total=False,
-)
-
-
-class DialogActionOutputTypeDef(
-    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
-):
-    pass
-
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Mapping[str, str],
+        "slots": Dict[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
@@ -172,96 +140,61 @@
 
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredIntentSummaryOutputTypeDef = TypedDict(
-    "_RequiredIntentSummaryOutputTypeDef",
+_RequiredIntentSummaryTypeDef = TypedDict(
+    "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
-_OptionalIntentSummaryOutputTypeDef = TypedDict(
-    "_OptionalIntentSummaryOutputTypeDef",
+_OptionalIntentSummaryTypeDef = TypedDict(
+    "_OptionalIntentSummaryTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
         "slots": Dict[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
 
-class IntentSummaryOutputTypeDef(
-    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
-):
+class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
 
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
-_RequiredIntentSummaryTypeDef = TypedDict(
-    "_RequiredIntentSummaryTypeDef",
-    {
-        "dialogActionType": DialogActionTypeType,
-    },
-)
-_OptionalIntentSummaryTypeDef = TypedDict(
-    "_OptionalIntentSummaryTypeDef",
-    {
-        "intentName": str,
-        "checkpointLabel": str,
-        "slots": Mapping[str, str],
-        "confirmationStatus": ConfirmationStatusType,
-        "fulfillmentState": FulfillmentStateType,
-        "slotToElicit": str,
-    },
-    total=False,
-)
-
-
-class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
-    pass
-
-
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentimentLabel": str,
         "sentimentScore": str,
     },
     total=False,
 )
 
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Mapping[str, str],
+        "parameters": Dict[str, str],
     },
 )
 
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
@@ -352,64 +285,51 @@
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
-IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionOutputTypeDef,
-        "activeContexts": List[ActiveContextOutputTypeDef],
+        "dialogAction": DialogActionTypeDef,
+        "activeContexts": List[ActiveContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
-
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "inputText": str,
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[ActiveContextUnionTypeDef],
+        "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
 
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
@@ -426,28 +346,38 @@
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
+        "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
-        "activeContexts": Sequence[ActiveContextUnionTypeDef],
+        "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
 
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
 
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
+    },
+    total=False,
+)
+
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
         "slots": Dict[str, str],
@@ -456,11 +386,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextOutputTypeDef],
+        "activeContexts": List[ActiveContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -35,36 +35,30 @@
 
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
     "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryOutputTypeDef",
-    "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
+    "IntentConfidenceTypeDef",
     "SentimentResponseTypeDef",
-    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
     "DeleteSessionResponseTypeDef",
     "PostContentResponseTypeDef",
     "PutSessionResponseTypeDef",
-    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
-    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
-    "ActiveContextUnionTypeDef",
-    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
+    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
@@ -98,49 +92,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredDialogActionOutputTypeDef = TypedDict(
-    "_RequiredDialogActionOutputTypeDef",
-    {
-        "type": DialogActionTypeType,
-    },
-)
-_OptionalDialogActionOutputTypeDef = TypedDict(
-    "_OptionalDialogActionOutputTypeDef",
-    {
-        "intentName": str,
-        "slots": Dict[str, str],
-        "slotToElicit": str,
-        "fulfillmentState": FulfillmentStateType,
-        "message": str,
-        "messageFormat": MessageFormatTypeType,
-    },
-    total=False,
-)
-
-class DialogActionOutputTypeDef(
-    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
-):
-    pass
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Mapping[str, str],
+        "slots": Dict[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
@@ -165,92 +135,59 @@
 )
 
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-_RequiredIntentSummaryOutputTypeDef = TypedDict(
-    "_RequiredIntentSummaryOutputTypeDef",
+_RequiredIntentSummaryTypeDef = TypedDict(
+    "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
-_OptionalIntentSummaryOutputTypeDef = TypedDict(
-    "_OptionalIntentSummaryOutputTypeDef",
+_OptionalIntentSummaryTypeDef = TypedDict(
+    "_OptionalIntentSummaryTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
         "slots": Dict[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-class IntentSummaryOutputTypeDef(
-    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
-):
+class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
 
-_RequiredIntentSummaryTypeDef = TypedDict(
-    "_RequiredIntentSummaryTypeDef",
-    {
-        "dialogActionType": DialogActionTypeType,
-    },
-)
-_OptionalIntentSummaryTypeDef = TypedDict(
-    "_OptionalIntentSummaryTypeDef",
-    {
-        "intentName": str,
-        "checkpointLabel": str,
-        "slots": Mapping[str, str],
-        "confirmationStatus": ConfirmationStatusType,
-        "fulfillmentState": FulfillmentStateType,
-        "slotToElicit": str,
-    },
-    total=False,
-)
-
-class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
-    pass
-
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentimentLabel": str,
         "sentimentScore": str,
     },
     total=False,
 )
 
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Mapping[str, str],
+        "parameters": Dict[str, str],
     },
 )
 
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
@@ -339,64 +276,51 @@
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
-IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionOutputTypeDef,
-        "activeContexts": List[ActiveContextOutputTypeDef],
+        "dialogAction": DialogActionTypeDef,
+        "activeContexts": List[ActiveContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
-
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "inputText": str,
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[ActiveContextUnionTypeDef],
+        "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
@@ -411,26 +335,36 @@
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
+        "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
-        "activeContexts": Sequence[ActiveContextUnionTypeDef],
+        "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
+    },
+    total=False,
+)
+
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
         "slots": Dict[str, str],
@@ -439,11 +373,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextOutputTypeDef],
+        "activeContexts": List[ActiveContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,71 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_lex_runtime.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `LexRuntimeService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/literals/).
+
 ```python
-from types_aiobotocore_lex_runtime.literals import (
-    ConfirmationStatusType,
-    ContentTypeType,
-    DialogActionTypeType,
-    DialogStateType,
-    FulfillmentStateType,
-    MessageFormatTypeType,
-    LexRuntimeServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `LexRuntimeService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveTypeDef,
-    BlobTypeDef,
-    ButtonTypeDef,
-    DeleteSessionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DialogActionOutputTypeDef,
-    DialogActionTypeDef,
-    GetSessionRequestRequestTypeDef,
-    IntentSummaryOutputTypeDef,
-    IntentConfidenceTypeDef,
-    IntentSummaryTypeDef,
-    SentimentResponseTypeDef,
-    ActiveContextOutputTypeDef,
-    ActiveContextTypeDef,
-    PostContentRequestRequestTypeDef,
-    GenericAttachmentTypeDef,
-    DeleteSessionResponseTypeDef,
-    PostContentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    DialogActionUnionTypeDef,
-    PredictedIntentTypeDef,
-    IntentSummaryUnionTypeDef,
-    GetSessionResponseTypeDef,
-    ActiveContextUnionTypeDef,
-    ResponseCardTypeDef,
-    PostTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PostTextResponseTypeDef,
-)
+from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
 
 def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

