# Comparing `tmp/types-aiobotocore-connectcampaigns-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-connectcampaigns-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:41 2023, max compression
```

## Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1.tar` & `types-aiobotocore-connectcampaigns-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.237613 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-02 14:35:53.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:52.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.241613 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:07.000000 types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:43:11.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:12.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.955744 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:41.000000 types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/LICENSE` & `types-aiobotocore-connectcampaigns-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,100 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_connectcampaigns.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ConnectCampaignService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/literals/).
+
 ```python
-from types_aiobotocore_connectcampaigns.literals import (
-    CampaignStateType,
-    EncryptionTypeType,
-    FailureCodeType,
-    GetCampaignStateBatchFailureCodeType,
-    InstanceIdFilterOperatorType,
-    InstanceOnboardingJobFailureCodeType,
-    InstanceOnboardingJobStatusCodeType,
-    ListCampaignsPaginatorName,
-    ConnectCampaignServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_connectcampaigns.literals import CampaignStateType
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ConnectCampaignService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/type_defs/).
+
 ```python
-from types_aiobotocore_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigTypeDef,
-    InstanceIdFilterTypeDef,
-    CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteCampaignRequestRequestTypeDef,
-    DeleteConnectInstanceConfigRequestRequestTypeDef,
-    DeleteInstanceOnboardingJobRequestRequestTypeDef,
-    DescribeCampaignRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredictiveDialerConfigTypeDef,
-    ProgressiveDialerConfigTypeDef,
-    EncryptionConfigTypeDef,
-    FailedCampaignStateResponseTypeDef,
-    FailedRequestTypeDef,
-    GetCampaignStateBatchRequestRequestTypeDef,
-    SuccessfulCampaignStateResponseTypeDef,
-    GetCampaignStateRequestRequestTypeDef,
-    GetConnectInstanceConfigRequestRequestTypeDef,
-    GetInstanceOnboardingJobStatusRequestRequestTypeDef,
-    InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PauseCampaignRequestRequestTypeDef,
-    SuccessfulRequestTypeDef,
-    ResumeCampaignRequestRequestTypeDef,
-    StartCampaignRequestRequestTypeDef,
-    StopCampaignRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigTypeDef,
-    UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
-    CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DialRequestTypeDef,
-    DialerConfigTypeDef,
-    InstanceConfigTypeDef,
-    StartInstanceOnboardingJobRequestRequestTypeDef,
-    GetCampaignStateBatchResponseTypeDef,
-    GetInstanceOnboardingJobStatusResponseTypeDef,
-    StartInstanceOnboardingJobResponseTypeDef,
-    PutDialRequestBatchResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListCampaignsRequestRequestTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
-    CampaignTypeDef,
-    CreateCampaignRequestRequestTypeDef,
-    UpdateCampaignDialerConfigRequestRequestTypeDef,
-    GetConnectInstanceConfigResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-)
+from types_aiobotocore_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
 
 def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/README.md` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-connectcampaigns
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore connectcampaigns type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcampaigns"></a>
 
 # types-aiobotocore-connectcampaigns
 
 [![PyPI - types-aiobotocore-connectcampaigns](https://img.shields.io/pypi/v/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,100 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_connectcampaigns.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ConnectCampaignService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/literals/).
+
 ```python
-from types_aiobotocore_connectcampaigns.literals import (
-    CampaignStateType,
-    EncryptionTypeType,
-    FailureCodeType,
-    GetCampaignStateBatchFailureCodeType,
-    InstanceIdFilterOperatorType,
-    InstanceOnboardingJobFailureCodeType,
-    InstanceOnboardingJobStatusCodeType,
-    ListCampaignsPaginatorName,
-    ConnectCampaignServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_connectcampaigns.literals import CampaignStateType
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ConnectCampaignService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/type_defs/).
+
 ```python
-from types_aiobotocore_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigTypeDef,
-    InstanceIdFilterTypeDef,
-    CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteCampaignRequestRequestTypeDef,
-    DeleteConnectInstanceConfigRequestRequestTypeDef,
-    DeleteInstanceOnboardingJobRequestRequestTypeDef,
-    DescribeCampaignRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredictiveDialerConfigTypeDef,
-    ProgressiveDialerConfigTypeDef,
-    EncryptionConfigTypeDef,
-    FailedCampaignStateResponseTypeDef,
-    FailedRequestTypeDef,
-    GetCampaignStateBatchRequestRequestTypeDef,
-    SuccessfulCampaignStateResponseTypeDef,
-    GetCampaignStateRequestRequestTypeDef,
-    GetConnectInstanceConfigRequestRequestTypeDef,
-    GetInstanceOnboardingJobStatusRequestRequestTypeDef,
-    InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PauseCampaignRequestRequestTypeDef,
-    SuccessfulRequestTypeDef,
-    ResumeCampaignRequestRequestTypeDef,
-    StartCampaignRequestRequestTypeDef,
-    StopCampaignRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigTypeDef,
-    UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
-    CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DialRequestTypeDef,
-    DialerConfigTypeDef,
-    InstanceConfigTypeDef,
-    StartInstanceOnboardingJobRequestRequestTypeDef,
-    GetCampaignStateBatchResponseTypeDef,
-    GetInstanceOnboardingJobStatusResponseTypeDef,
-    StartInstanceOnboardingJobResponseTypeDef,
-    PutDialRequestBatchResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListCampaignsRequestRequestTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
-    CampaignTypeDef,
-    CreateCampaignRequestRequestTypeDef,
-    UpdateCampaignDialerConfigRequestRequestTypeDef,
-    GetConnectInstanceConfigResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-)
+from types_aiobotocore_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
 
 def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/setup.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcampaigns",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__init__.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/__main__.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectCampaignService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/client.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/literals.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/paginator.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.py` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns/type_defs.pyi` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectcampaigns type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcampaigns"></a>
 
 # types-aiobotocore-connectcampaigns
 
 [![PyPI - types-aiobotocore-connectcampaigns](https://img.shields.io/pypi/v/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
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
 [types-aiobotocore-connectcampaigns docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,100 +257,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_connectcampaigns.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ConnectCampaignService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/literals/).
+
 ```python
-from types_aiobotocore_connectcampaigns.literals import (
-    CampaignStateType,
-    EncryptionTypeType,
-    FailureCodeType,
-    GetCampaignStateBatchFailureCodeType,
-    InstanceIdFilterOperatorType,
-    InstanceOnboardingJobFailureCodeType,
-    InstanceOnboardingJobStatusCodeType,
-    ListCampaignsPaginatorName,
-    ConnectCampaignServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_connectcampaigns.literals import CampaignStateType
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_connectcampaigns.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ConnectCampaignService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/type_defs/).
+
 ```python
-from types_aiobotocore_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigTypeDef,
-    InstanceIdFilterTypeDef,
-    CampaignSummaryTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteCampaignRequestRequestTypeDef,
-    DeleteConnectInstanceConfigRequestRequestTypeDef,
-    DeleteInstanceOnboardingJobRequestRequestTypeDef,
-    DescribeCampaignRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredictiveDialerConfigTypeDef,
-    ProgressiveDialerConfigTypeDef,
-    EncryptionConfigTypeDef,
-    FailedCampaignStateResponseTypeDef,
-    FailedRequestTypeDef,
-    GetCampaignStateBatchRequestRequestTypeDef,
-    SuccessfulCampaignStateResponseTypeDef,
-    GetCampaignStateRequestRequestTypeDef,
-    GetConnectInstanceConfigRequestRequestTypeDef,
-    GetInstanceOnboardingJobStatusRequestRequestTypeDef,
-    InstanceOnboardingJobStatusTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PauseCampaignRequestRequestTypeDef,
-    SuccessfulRequestTypeDef,
-    ResumeCampaignRequestRequestTypeDef,
-    StartCampaignRequestRequestTypeDef,
-    StopCampaignRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigTypeDef,
-    UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
-    CampaignFiltersTypeDef,
-    CreateCampaignResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCampaignStateResponseTypeDef,
-    ListCampaignsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DialRequestTypeDef,
-    DialerConfigTypeDef,
-    InstanceConfigTypeDef,
-    StartInstanceOnboardingJobRequestRequestTypeDef,
-    GetCampaignStateBatchResponseTypeDef,
-    GetInstanceOnboardingJobStatusResponseTypeDef,
-    StartInstanceOnboardingJobResponseTypeDef,
-    PutDialRequestBatchResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
-    ListCampaignsRequestRequestTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
-    CampaignTypeDef,
-    CreateCampaignRequestRequestTypeDef,
-    UpdateCampaignDialerConfigRequestRequestTypeDef,
-    GetConnectInstanceConfigResponseTypeDef,
-    DescribeCampaignResponseTypeDef,
-)
+from types_aiobotocore_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
 
 def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post1/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt` & `types-aiobotocore-connectcampaigns-2.5.2.post2/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

