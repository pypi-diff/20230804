# Comparing `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.916643 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13730 2023-08-04 13:59:24.916643 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12159 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.916643 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2159 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.906643 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      746 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      745 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      993 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8408 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8393 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8183 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8181 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2396 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2393 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5652 2023-08-04 13:52:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5646 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:23.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.906643 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13730 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1079 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       40 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,58 +289,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_a2i_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AugmentedAIRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.literals import (
-    ContentClassifierType,
-    HumanLoopStatusType,
-    ListHumanLoopsPaginatorName,
-    SortOrderType,
-    AugmentedAIRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.literals import ContentClassifierType
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `AugmentedAIRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
-    DeleteHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopRequestRequestTypeDef,
-    HumanLoopOutputTypeDef,
-    ResponseMetadataTypeDef,
-    HumanLoopDataAttributesTypeDef,
-    HumanLoopInputTypeDef,
-    HumanLoopSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    StopHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopResponseTypeDef,
-    StartHumanLoopResponseTypeDef,
-    StartHumanLoopRequestRequestTypeDef,
-    ListHumanLoopsResponseTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
 
 def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/README.md` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/README.md`

 * *Files 9% similar despite different names*

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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,58 +257,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_a2i_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AugmentedAIRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.literals import (
-    ContentClassifierType,
-    HumanLoopStatusType,
-    ListHumanLoopsPaginatorName,
-    SortOrderType,
-    AugmentedAIRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.literals import ContentClassifierType
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `AugmentedAIRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
-    DeleteHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopRequestRequestTypeDef,
-    HumanLoopOutputTypeDef,
-    ResponseMetadataTypeDef,
-    HumanLoopDataAttributesTypeDef,
-    HumanLoopInputTypeDef,
-    HumanLoopSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    StopHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopResponseTypeDef,
-    StartHumanLoopResponseTypeDef,
-    StartHumanLoopRequestRequestTypeDef,
-    ListHumanLoopsResponseTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
 
 def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-a2i-runtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker_a2i_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime\nOther"
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
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
@@ -150,14 +151,15 @@
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
@@ -236,26 +238,28 @@
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
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
@@ -148,14 +149,15 @@
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
@@ -234,26 +236,28 @@
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,58 +289,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_a2i_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AugmentedAIRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.literals import (
-    ContentClassifierType,
-    HumanLoopStatusType,
-    ListHumanLoopsPaginatorName,
-    SortOrderType,
-    AugmentedAIRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.literals import ContentClassifierType
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `AugmentedAIRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
-    DeleteHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopRequestRequestTypeDef,
-    HumanLoopOutputTypeDef,
-    ResponseMetadataTypeDef,
-    HumanLoopDataAttributesTypeDef,
-    HumanLoopInputTypeDef,
-    HumanLoopSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    StopHumanLoopRequestRequestTypeDef,
-    DescribeHumanLoopResponseTypeDef,
-    StartHumanLoopResponseTypeDef,
-    StartHumanLoopRequestRequestTypeDef,
-    ListHumanLoopsResponseTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
 
 def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

