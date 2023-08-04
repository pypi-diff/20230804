# Comparing `tmp/types-aiobotocore-synthetics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-synthetics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-synthetics-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-synthetics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-synthetics-2.5.2.post1.tar` & `types-aiobotocore-synthetics-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18881 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:32.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.833439 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:53:06.000000 types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.566643 types-aiobotocore-synthetics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12375 2023-08-04 13:59:28.566643 types-aiobotocore-synthetics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10845 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.566643 types-aiobotocore-synthetics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.566643 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      466 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      465 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17058 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17029 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9064 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9062 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18400 2023-08-04 13:55:00.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18377 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:59.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.566643 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12375 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      785 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:28.000000 types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/LICENSE` & `types-aiobotocore-synthetics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/PKG-INFO` & `types-aiobotocore-synthetics-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-synthetics
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,102 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_synthetics.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Synthetics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/literals/).
+
 ```python
-from types_aiobotocore_synthetics.literals import (
-    CanaryRunStateReasonCodeType,
-    CanaryRunStateType,
-    CanaryStateReasonCodeType,
-    CanaryStateType,
-    EncryptionModeType,
-    SyntheticsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_synthetics.literals import CanaryRunStateReasonCodeType
 
 
 def check_value(value: CanaryRunStateReasonCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Synthetics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/type_defs/).
+
 ```python
-from types_aiobotocore_synthetics.type_defs import (
-    S3EncryptionConfigTypeDef,
-    AssociateResourceRequestRequestTypeDef,
-    BaseScreenshotOutputTypeDef,
-    BaseScreenshotTypeDef,
-    BlobTypeDef,
-    CanaryCodeOutputTypeDef,
-    CanaryRunConfigInputTypeDef,
-    CanaryRunConfigOutputTypeDef,
-    CanaryRunStatusTypeDef,
-    CanaryRunTimelineTypeDef,
-    CanaryScheduleInputTypeDef,
-    CanaryScheduleOutputTypeDef,
-    CanaryStatusTypeDef,
-    CanaryTimelineTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigInputTypeDef,
-    ResponseMetadataTypeDef,
-    CreateGroupRequestRequestTypeDef,
-    GroupTypeDef,
-    DeleteCanaryRequestRequestTypeDef,
-    DeleteGroupRequestRequestTypeDef,
-    DescribeCanariesLastRunRequestRequestTypeDef,
-    DescribeCanariesRequestRequestTypeDef,
-    DescribeRuntimeVersionsRequestRequestTypeDef,
-    RuntimeVersionTypeDef,
-    DisassociateResourceRequestRequestTypeDef,
-    GetCanaryRequestRequestTypeDef,
-    GetCanaryRunsRequestRequestTypeDef,
-    GetGroupRequestRequestTypeDef,
-    GroupSummaryTypeDef,
-    ListAssociatedGroupsRequestRequestTypeDef,
-    ListGroupResourcesRequestRequestTypeDef,
-    ListGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartCanaryRequestRequestTypeDef,
-    StopCanaryRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ArtifactConfigInputTypeDef,
-    ArtifactConfigOutputTypeDef,
-    VisualReferenceOutputTypeDef,
-    VisualReferenceInputTypeDef,
-    CanaryCodeInputTypeDef,
-    CanaryRunTypeDef,
-    ListGroupResourcesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    GetGroupResponseTypeDef,
-    DescribeRuntimeVersionsResponseTypeDef,
-    ListAssociatedGroupsResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    CanaryTypeDef,
-    CreateCanaryRequestRequestTypeDef,
-    UpdateCanaryRequestRequestTypeDef,
-    CanaryLastRunTypeDef,
-    GetCanaryRunsResponseTypeDef,
-    CreateCanaryResponseTypeDef,
-    DescribeCanariesResponseTypeDef,
-    GetCanaryResponseTypeDef,
-    DescribeCanariesLastRunResponseTypeDef,
-)
+from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef
 
 
 def get_value() -> S3EncryptionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/README.md` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-synthetics
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Synthetics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore synthetics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,102 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_synthetics.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Synthetics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/literals/).
+
 ```python
-from types_aiobotocore_synthetics.literals import (
-    CanaryRunStateReasonCodeType,
-    CanaryRunStateType,
-    CanaryStateReasonCodeType,
-    CanaryStateType,
-    EncryptionModeType,
-    SyntheticsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_synthetics.literals import CanaryRunStateReasonCodeType
 
 
 def check_value(value: CanaryRunStateReasonCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Synthetics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/type_defs/).
+
 ```python
-from types_aiobotocore_synthetics.type_defs import (
-    S3EncryptionConfigTypeDef,
-    AssociateResourceRequestRequestTypeDef,
-    BaseScreenshotOutputTypeDef,
-    BaseScreenshotTypeDef,
-    BlobTypeDef,
-    CanaryCodeOutputTypeDef,
-    CanaryRunConfigInputTypeDef,
-    CanaryRunConfigOutputTypeDef,
-    CanaryRunStatusTypeDef,
-    CanaryRunTimelineTypeDef,
-    CanaryScheduleInputTypeDef,
-    CanaryScheduleOutputTypeDef,
-    CanaryStatusTypeDef,
-    CanaryTimelineTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigInputTypeDef,
-    ResponseMetadataTypeDef,
-    CreateGroupRequestRequestTypeDef,
-    GroupTypeDef,
-    DeleteCanaryRequestRequestTypeDef,
-    DeleteGroupRequestRequestTypeDef,
-    DescribeCanariesLastRunRequestRequestTypeDef,
-    DescribeCanariesRequestRequestTypeDef,
-    DescribeRuntimeVersionsRequestRequestTypeDef,
-    RuntimeVersionTypeDef,
-    DisassociateResourceRequestRequestTypeDef,
-    GetCanaryRequestRequestTypeDef,
-    GetCanaryRunsRequestRequestTypeDef,
-    GetGroupRequestRequestTypeDef,
-    GroupSummaryTypeDef,
-    ListAssociatedGroupsRequestRequestTypeDef,
-    ListGroupResourcesRequestRequestTypeDef,
-    ListGroupsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StartCanaryRequestRequestTypeDef,
-    StopCanaryRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ArtifactConfigInputTypeDef,
-    ArtifactConfigOutputTypeDef,
-    VisualReferenceOutputTypeDef,
-    VisualReferenceInputTypeDef,
-    CanaryCodeInputTypeDef,
-    CanaryRunTypeDef,
-    ListGroupResourcesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    GetGroupResponseTypeDef,
-    DescribeRuntimeVersionsResponseTypeDef,
-    ListAssociatedGroupsResponseTypeDef,
-    ListGroupsResponseTypeDef,
-    CanaryTypeDef,
-    CreateCanaryRequestRequestTypeDef,
-    UpdateCanaryRequestRequestTypeDef,
-    CanaryLastRunTypeDef,
-    GetCanaryRunsResponseTypeDef,
-    CreateCanaryResponseTypeDef,
-    DescribeCanariesResponseTypeDef,
-    GetCanaryResponseTypeDef,
-    DescribeCanariesLastRunResponseTypeDef,
-)
+from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef
 
 
 def get_value() -> S3EncryptionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/setup.py` & `types-aiobotocore-synthetics-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-synthetics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_synthetics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Synthetics 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/__main__.py` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Synthetics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Synthetics 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics\nOther"
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

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.py` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/client.pyi` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.py` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -261,26 +263,28 @@
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
@@ -441,14 +445,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/literals.pyi` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -439,14 +443,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.py` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "BlobTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
@@ -68,16 +67,16 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceOutputTypeDef",
     "VisualReferenceInputTypeDef",
+    "VisualReferenceOutputTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryRunTypeDef",
     "ListGroupResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
@@ -107,45 +106,24 @@
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
-_RequiredBaseScreenshotOutputTypeDef = TypedDict(
-    "_RequiredBaseScreenshotOutputTypeDef",
-    {
-        "ScreenshotName": str,
-    },
-)
-_OptionalBaseScreenshotOutputTypeDef = TypedDict(
-    "_OptionalBaseScreenshotOutputTypeDef",
-    {
-        "IgnoreCoordinates": List[str],
-    },
-    total=False,
-)
-
-
-class BaseScreenshotOutputTypeDef(
-    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
-):
-    pass
-
-
 _RequiredBaseScreenshotTypeDef = TypedDict(
     "_RequiredBaseScreenshotTypeDef",
     {
         "ScreenshotName": str,
     },
 )
 _OptionalBaseScreenshotTypeDef = TypedDict(
     "_OptionalBaseScreenshotTypeDef",
     {
-        "IgnoreCoordinates": Sequence[str],
+        "IgnoreCoordinates": List[str],
     },
     total=False,
 )
 
 
 class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
@@ -542,23 +520,14 @@
     "ArtifactConfigOutputTypeDef",
     {
         "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
-    {
-        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
-        "BaseCanaryRunId": str,
-    },
-    total=False,
-)
-
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
         "BaseCanaryRunId": str,
     },
 )
 _OptionalVisualReferenceInputTypeDef = TypedDict(
@@ -572,14 +541,23 @@
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
 
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotTypeDef],
+        "BaseCanaryRunId": str,
+    },
+    total=False,
+)
+
 _RequiredCanaryCodeInputTypeDef = TypedDict(
     "_RequiredCanaryCodeInputTypeDef",
     {
         "Handler": str,
     },
 )
 _OptionalCanaryCodeInputTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics/type_defs.pyi` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "BlobTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
@@ -67,16 +66,16 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceOutputTypeDef",
     "VisualReferenceInputTypeDef",
+    "VisualReferenceOutputTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryRunTypeDef",
     "ListGroupResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
@@ -106,43 +105,24 @@
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
-_RequiredBaseScreenshotOutputTypeDef = TypedDict(
-    "_RequiredBaseScreenshotOutputTypeDef",
-    {
-        "ScreenshotName": str,
-    },
-)
-_OptionalBaseScreenshotOutputTypeDef = TypedDict(
-    "_OptionalBaseScreenshotOutputTypeDef",
-    {
-        "IgnoreCoordinates": List[str],
-    },
-    total=False,
-)
-
-class BaseScreenshotOutputTypeDef(
-    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
-):
-    pass
-
 _RequiredBaseScreenshotTypeDef = TypedDict(
     "_RequiredBaseScreenshotTypeDef",
     {
         "ScreenshotName": str,
     },
 )
 _OptionalBaseScreenshotTypeDef = TypedDict(
     "_OptionalBaseScreenshotTypeDef",
     {
-        "IgnoreCoordinates": Sequence[str],
+        "IgnoreCoordinates": List[str],
     },
     total=False,
 )
 
 class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
 
@@ -525,23 +505,14 @@
     "ArtifactConfigOutputTypeDef",
     {
         "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
-    {
-        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
-        "BaseCanaryRunId": str,
-    },
-    total=False,
-)
-
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
         "BaseCanaryRunId": str,
     },
 )
 _OptionalVisualReferenceInputTypeDef = TypedDict(
@@ -553,14 +524,23 @@
 )
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotTypeDef],
+        "BaseCanaryRunId": str,
+    },
+    total=False,
+)
+
 _RequiredCanaryCodeInputTypeDef = TypedDict(
     "_RequiredCanaryCodeInputTypeDef",
     {
         "Handler": str,
     },
 )
 _OptionalCanaryCodeInputTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-synthetics-2.5.2.post1/types_aiobotocore_synthetics.egg-info/SOURCES.txt` & `types-aiobotocore-synthetics-2.5.2.post2/types_aiobotocore_synthetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

