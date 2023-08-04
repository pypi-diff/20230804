# Comparing `tmp/types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.057469 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-08-02 14:52:57.057469 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.057469 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.057469 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-08-02 14:48:59.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.057469 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.056643 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13401 2023-08-04 13:59:25.056643 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11793 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.056643 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2234 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.056643 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      616 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      615 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1031 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7905 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7893 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8106 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8104 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5944 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5931 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:26.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.056643 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13401 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1125 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       49 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-featurestore-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/
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
 [types-aiobotocore-sagemaker-featurestore-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,53 +270,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_featurestore_runtime.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    TargetStoreType,
-    SageMakerFeatureStoreRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.literals import DeletionModeType
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import (
-    BatchGetRecordErrorTypeDef,
-    BatchGetRecordIdentifierOutputTypeDef,
-    BatchGetRecordIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
-    DeleteRecordRequestRequestTypeDef,
-    GetRecordRequestRequestTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    BatchGetRecordResultDetailTypeDef,
-    GetRecordResponseTypeDef,
-    PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
-    BatchGetRecordResponseTypeDef,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
 
 def get_value() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/README.md` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-sagemaker-featurestore-runtime
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore sagemaker-featurestore-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-featurestore-runtime"></a>
 
 # types-aiobotocore-sagemaker-featurestore-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/)
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
 [types-aiobotocore-sagemaker-featurestore-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -238,53 +270,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_featurestore_runtime.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    TargetStoreType,
-    SageMakerFeatureStoreRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.literals import DeletionModeType
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import (
-    BatchGetRecordErrorTypeDef,
-    BatchGetRecordIdentifierOutputTypeDef,
-    BatchGetRecordIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
-    DeleteRecordRequestRequestTypeDef,
-    GetRecordRequestRequestTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    BatchGetRecordResultDetailTypeDef,
-    GetRecordResponseTypeDef,
-    PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
-    BatchGetRecordResponseTypeDef,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
 
 def get_value() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-featurestore-runtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker_featurestore_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__init__.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__init__.pyi` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/__main__.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime\nOther"
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

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/client.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,22 @@
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import DeletionModeType, TargetStoreType
+from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
 from .type_defs import (
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
+    TtlDurationTypeDef,
 )
 
 __all__ = ("SageMakerFeatureStoreRuntimeClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -62,15 +63,18 @@
         SageMakerFeatureStoreRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#exceptions)
         """
 
     async def batch_get_record(
-        self, *, Identifiers: Sequence[BatchGetRecordIdentifierUnionTypeDef]
+        self,
+        *,
+        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
+        ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> BatchGetRecordResponseTypeDef:
         """
         Retrieves a batch of `Records` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#batch_get_record)
         """
@@ -122,32 +126,35 @@
         """
 
     async def get_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
-        FeatureNames: Sequence[str] = ...
+        FeatureNames: Sequence[str] = ...,
+        ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> GetRecordResponseTypeDef:
         """
         Use for `OnlineStore` serving from a `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.get_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#get_record)
         """
 
     async def put_record(
         self,
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
-        TargetStores: Sequence[TargetStoreType] = ...
+        TargetStores: Sequence[TargetStoreType] = ...,
+        TtlDuration: TtlDurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Used for data ingestion into the `FeatureStore`.
+        The `PutRecord` API is used to ingest a list of `Records` into your feature
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#put_record)
         """
 
     async def __aenter__(self) -> "SageMakerFeatureStoreRuntimeClient":
         """
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/client.pyi` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,22 @@
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import DeletionModeType, TargetStoreType
+from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
 from .type_defs import (
-    BatchGetRecordIdentifierUnionTypeDef,
+    BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
+    TtlDurationTypeDef,
 )
 
 __all__ = ("SageMakerFeatureStoreRuntimeClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -58,15 +59,18 @@
         """
         SageMakerFeatureStoreRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#exceptions)
         """
     async def batch_get_record(
-        self, *, Identifiers: Sequence[BatchGetRecordIdentifierUnionTypeDef]
+        self,
+        *,
+        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
+        ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> BatchGetRecordResponseTypeDef:
         """
         Retrieves a batch of `Records` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#batch_get_record)
         """
@@ -113,31 +117,34 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#generate_presigned_url)
         """
     async def get_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
-        FeatureNames: Sequence[str] = ...
+        FeatureNames: Sequence[str] = ...,
+        ExpirationTimeResponse: ExpirationTimeResponseType = ...
     ) -> GetRecordResponseTypeDef:
         """
         Use for `OnlineStore` serving from a `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.get_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#get_record)
         """
     async def put_record(
         self,
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
-        TargetStores: Sequence[TargetStoreType] = ...
+        TargetStores: Sequence[TargetStoreType] = ...,
+        TtlDuration: TtlDurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Used for data ingestion into the `FeatureStore`.
+        The `PutRecord` API is used to ingest a list of `Records` into your feature
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/client/#put_record)
         """
     async def __aenter__(self) -> "SageMakerFeatureStoreRuntimeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client)
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/literals.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,27 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "DeletionModeType",
+    "ExpirationTimeResponseType",
     "TargetStoreType",
+    "TtlDurationUnitType",
     "SageMakerFeatureStoreRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
 
 DeletionModeType = Literal["HardDelete", "SoftDelete"]
+ExpirationTimeResponseType = Literal["Disabled", "Enabled"]
 TargetStoreType = Literal["OfflineStore", "OnlineStore"]
+TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 SageMakerFeatureStoreRuntimeServiceName = Literal["sagemaker-featurestore-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -42,14 +46,15 @@
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
@@ -145,14 +150,15 @@
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
@@ -231,26 +237,28 @@
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

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/literals.pyi` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,26 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "DeletionModeType",
+    "ExpirationTimeResponseType",
     "TargetStoreType",
+    "TtlDurationUnitType",
     "SageMakerFeatureStoreRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
 DeletionModeType = Literal["HardDelete", "SoftDelete"]
+ExpirationTimeResponseType = Literal["Disabled", "Enabled"]
 TargetStoreType = Literal["OfflineStore", "OnlineStore"]
+TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 SageMakerFeatureStoreRuntimeServiceName = Literal["sagemaker-featurestore-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -40,14 +44,15 @@
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
@@ -143,14 +148,15 @@
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
@@ -229,26 +235,28 @@
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

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.py` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,73 +8,54 @@
     ```python
     from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
     data: BatchGetRecordErrorTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
-from .literals import DeletionModeType, TargetStoreType
+from .literals import (
+    DeletionModeType,
+    ExpirationTimeResponseType,
+    TargetStoreType,
+    TtlDurationUnitType,
+)
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchGetRecordErrorTypeDef",
-    "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "FeatureValueTypeDef",
     "DeleteRecordRequestRequestTypeDef",
     "GetRecordRequestRequestTypeDef",
-    "BatchGetRecordIdentifierUnionTypeDef",
+    "TtlDurationTypeDef",
+    "BatchGetRecordRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
-    "BatchGetRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
     "BatchGetRecordErrorTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
-    {
-        "FeatureGroupName": str,
-        "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
-        "FeatureNames": List[str],
-    },
-    total=False,
-)
-
-
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -82,21 +63,19 @@
     "_OptionalBatchGetRecordIdentifierTypeDef",
     {
         "FeatureNames": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchGetRecordIdentifierTypeDef(
     _RequiredBatchGetRecordIdentifierTypeDef, _OptionalBatchGetRecordIdentifierTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -125,66 +104,100 @@
     {
         "TargetStores": Sequence[TargetStoreType],
         "DeletionMode": DeletionModeType,
     },
     total=False,
 )
 
-
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
     },
 )
 _OptionalGetRecordRequestRequestTypeDef = TypedDict(
     "_OptionalGetRecordRequestRequestTypeDef",
     {
         "FeatureNames": Sequence[str],
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
     },
     total=False,
 )
 
-
 class GetRecordRequestRequestTypeDef(
     _RequiredGetRecordRequestRequestTypeDef, _OptionalGetRecordRequestRequestTypeDef
 ):
     pass
 
+TtlDurationTypeDef = TypedDict(
+    "TtlDurationTypeDef",
+    {
+        "Unit": TtlDurationUnitType,
+        "Value": int,
+    },
+)
+
+_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetRecordRequestRequestTypeDef",
+    {
+        "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
+    },
+)
+_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetRecordRequestRequestTypeDef",
+    {
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
+    },
+    total=False,
+)
+
+class BatchGetRecordRequestRequestTypeDef(
+    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
+):
+    pass
 
-BatchGetRecordIdentifierUnionTypeDef = Union[
-    BatchGetRecordIdentifierTypeDef, BatchGetRecordIdentifierOutputTypeDef
-]
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetRecordResultDetailTypeDef = TypedDict(
-    "BatchGetRecordResultDetailTypeDef",
+_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
+    "_RequiredBatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "Record": List[FeatureValueTypeDef],
     },
 )
+_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
+    "_OptionalBatchGetRecordResultDetailTypeDef",
+    {
+        "ExpiresAt": str,
+    },
+    total=False,
+)
+
+class BatchGetRecordResultDetailTypeDef(
+    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
+):
+    pass
 
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
         "Record": List[FeatureValueTypeDef],
+        "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
     {
@@ -192,34 +205,26 @@
         "Record": Sequence[FeatureValueTypeDef],
     },
 )
 _OptionalPutRecordRequestRequestTypeDef = TypedDict(
     "_OptionalPutRecordRequestRequestTypeDef",
     {
         "TargetStores": Sequence[TargetStoreType],
+        "TtlDuration": TtlDurationTypeDef,
     },
     total=False,
 )
 
-
 class PutRecordRequestRequestTypeDef(
     _RequiredPutRecordRequestRequestTypeDef, _OptionalPutRecordRequestRequestTypeDef
 ):
     pass
 
-
-BatchGetRecordRequestRequestTypeDef = TypedDict(
-    "BatchGetRecordRequestRequestTypeDef",
-    {
-        "Identifiers": Sequence[BatchGetRecordIdentifierUnionTypeDef],
-    },
-)
-
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
-        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
+        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.pyi` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,70 +8,55 @@
     ```python
     from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
     data: BatchGetRecordErrorTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
-from .literals import DeletionModeType, TargetStoreType
+from .literals import (
+    DeletionModeType,
+    ExpirationTimeResponseType,
+    TargetStoreType,
+    TtlDurationUnitType,
+)
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchGetRecordErrorTypeDef",
-    "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "FeatureValueTypeDef",
     "DeleteRecordRequestRequestTypeDef",
     "GetRecordRequestRequestTypeDef",
-    "BatchGetRecordIdentifierUnionTypeDef",
+    "TtlDurationTypeDef",
+    "BatchGetRecordRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
-    "BatchGetRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
     "BatchGetRecordErrorTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
-_RequiredBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_RequiredBatchGetRecordIdentifierOutputTypeDef",
-    {
-        "FeatureGroupName": str,
-        "RecordIdentifiersValueAsString": List[str],
-    },
-)
-_OptionalBatchGetRecordIdentifierOutputTypeDef = TypedDict(
-    "_OptionalBatchGetRecordIdentifierOutputTypeDef",
-    {
-        "FeatureNames": List[str],
-    },
-    total=False,
-)
-
-class BatchGetRecordIdentifierOutputTypeDef(
-    _RequiredBatchGetRecordIdentifierOutputTypeDef, _OptionalBatchGetRecordIdentifierOutputTypeDef
-):
-    pass
-
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -79,19 +64,21 @@
     "_OptionalBatchGetRecordIdentifierTypeDef",
     {
         "FeatureNames": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchGetRecordIdentifierTypeDef(
     _RequiredBatchGetRecordIdentifierTypeDef, _OptionalBatchGetRecordIdentifierTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -120,62 +107,108 @@
     {
         "TargetStores": Sequence[TargetStoreType],
         "DeletionMode": DeletionModeType,
     },
     total=False,
 )
 
+
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
     },
 )
 _OptionalGetRecordRequestRequestTypeDef = TypedDict(
     "_OptionalGetRecordRequestRequestTypeDef",
     {
         "FeatureNames": Sequence[str],
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
     },
     total=False,
 )
 
+
 class GetRecordRequestRequestTypeDef(
     _RequiredGetRecordRequestRequestTypeDef, _OptionalGetRecordRequestRequestTypeDef
 ):
     pass
 
-BatchGetRecordIdentifierUnionTypeDef = Union[
-    BatchGetRecordIdentifierTypeDef, BatchGetRecordIdentifierOutputTypeDef
-]
+
+TtlDurationTypeDef = TypedDict(
+    "TtlDurationTypeDef",
+    {
+        "Unit": TtlDurationUnitType,
+        "Value": int,
+    },
+)
+
+_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetRecordRequestRequestTypeDef",
+    {
+        "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
+    },
+)
+_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetRecordRequestRequestTypeDef",
+    {
+        "ExpirationTimeResponse": ExpirationTimeResponseType,
+    },
+    total=False,
+)
+
+
+class BatchGetRecordRequestRequestTypeDef(
+    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
+):
+    pass
+
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetRecordResultDetailTypeDef = TypedDict(
-    "BatchGetRecordResultDetailTypeDef",
+_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
+    "_RequiredBatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "Record": List[FeatureValueTypeDef],
     },
 )
+_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
+    "_OptionalBatchGetRecordResultDetailTypeDef",
+    {
+        "ExpiresAt": str,
+    },
+    total=False,
+)
+
+
+class BatchGetRecordResultDetailTypeDef(
+    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
+):
+    pass
+
 
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
         "Record": List[FeatureValueTypeDef],
+        "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
     {
@@ -183,32 +216,28 @@
         "Record": Sequence[FeatureValueTypeDef],
     },
 )
 _OptionalPutRecordRequestRequestTypeDef = TypedDict(
     "_OptionalPutRecordRequestRequestTypeDef",
     {
         "TargetStores": Sequence[TargetStoreType],
+        "TtlDuration": TtlDurationTypeDef,
     },
     total=False,
 )
 
+
 class PutRecordRequestRequestTypeDef(
     _RequiredPutRecordRequestRequestTypeDef, _OptionalPutRecordRequestRequestTypeDef
 ):
     pass
 
-BatchGetRecordRequestRequestTypeDef = TypedDict(
-    "BatchGetRecordRequestRequestTypeDef",
-    {
-        "Identifiers": Sequence[BatchGetRecordIdentifierUnionTypeDef],
-    },
-)
 
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
-        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
+        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-sagemaker-featurestore-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SageMakerFeatureStoreRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sagemaker-featurestore-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-featurestore-runtime"></a>
 
 # types-aiobotocore-sagemaker-featurestore-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/)
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
 [types-aiobotocore-sagemaker-featurestore-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,53 +238,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_featurestore_runtime.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    TargetStoreType,
-    SageMakerFeatureStoreRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.literals import DeletionModeType
 
 
 def check_value(value: DeletionModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `SageMakerFeatureStoreRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_featurestore_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import (
-    BatchGetRecordErrorTypeDef,
-    BatchGetRecordIdentifierOutputTypeDef,
-    BatchGetRecordIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    FeatureValueTypeDef,
-    DeleteRecordRequestRequestTypeDef,
-    GetRecordRequestRequestTypeDef,
-    BatchGetRecordIdentifierUnionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    BatchGetRecordResultDetailTypeDef,
-    GetRecordResponseTypeDef,
-    PutRecordRequestRequestTypeDef,
-    BatchGetRecordRequestRequestTypeDef,
-    BatchGetRecordResponseTypeDef,
-)
+from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef
 
 
 def get_value() -> BatchGetRecordErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post1/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-featurestore-runtime-2.5.2.post2/types_aiobotocore_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

