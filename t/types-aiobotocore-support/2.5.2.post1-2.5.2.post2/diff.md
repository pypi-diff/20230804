# Comparing `tmp/types-aiobotocore-support-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-support-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-support-2.5.2.post1.tar` & `types-aiobotocore-support-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-08-02 14:50:25.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:24.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.485440 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:53:06.000000 types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13096 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11578 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.396643 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      871 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16246 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16219 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7933 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7931 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3499 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3495 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18653 2023-08-04 13:54:49.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18636 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13096 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      813 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-2.5.2.post1/LICENSE` & `types-aiobotocore-support-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post1/PKG-INFO` & `types-aiobotocore-support-2.5.2.post2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,98 +294,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Support` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/literals/).
+
 ```python
-from types_aiobotocore_support.literals import (
-    DescribeCasesPaginatorName,
-    DescribeCommunicationsPaginatorName,
-    SupportServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_support.literals import DescribeCasesPaginatorName
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Support` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/type_defs/).
+
 ```python
-from types_aiobotocore_support.type_defs import (
-    ResponseMetadataTypeDef,
-    AddCommunicationToCaseRequestRequestTypeDef,
-    AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
-    BlobTypeDef,
-    CategoryTypeDef,
-    DateIntervalTypeDef,
-    SupportedHourTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestRequestTypeDef,
-    DescribeCreateCaseOptionsRequestRequestTypeDef,
-    DescribeServicesRequestRequestTypeDef,
-    DescribeSeverityLevelsRequestRequestTypeDef,
-    SeverityLevelTypeDef,
-    DescribeSupportedLanguagesRequestRequestTypeDef,
-    SupportedLanguageTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
-    TrustedAdvisorCheckRefreshStatusTypeDef,
-    DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
-    DescribeTrustedAdvisorChecksRequestRequestTypeDef,
-    TrustedAdvisorCheckDescriptionTypeDef,
-    RefreshTrustedAdvisorCheckRequestRequestTypeDef,
-    ResolveCaseRequestRequestTypeDef,
-    TrustedAdvisorCostOptimizingSummaryTypeDef,
-    TrustedAdvisorResourceDetailTypeDef,
-    TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    ResolveCaseResponseTypeDef,
-    CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
-    AttachmentTypeDef,
-    ServiceTypeDef,
-    CommunicationTypeOptionsTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    DescribeSeverityLevelsResponseTypeDef,
-    DescribeSupportedLanguagesResponseTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
-    RefreshTrustedAdvisorCheckResponseTypeDef,
-    DescribeTrustedAdvisorChecksResponseTypeDef,
-    TrustedAdvisorCategorySpecificSummaryTypeDef,
-    DescribeCommunicationsResponseTypeDef,
-    RecentCaseCommunicationsTypeDef,
-    AttachmentUnionTypeDef,
-    DescribeServicesResponseTypeDef,
-    DescribeCreateCaseOptionsResponseTypeDef,
-    TrustedAdvisorCheckResultTypeDef,
-    TrustedAdvisorCheckSummaryTypeDef,
-    CaseDetailsTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckResultResponseTypeDef,
-    DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
-    DescribeCasesResponseTypeDef,
-)
+from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-support-2.5.2.post1/README.md` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-support
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore support type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -262,98 +294,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Support` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/literals/).
+
 ```python
-from types_aiobotocore_support.literals import (
-    DescribeCasesPaginatorName,
-    DescribeCommunicationsPaginatorName,
-    SupportServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_support.literals import DescribeCasesPaginatorName
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Support` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/type_defs/).
+
 ```python
-from types_aiobotocore_support.type_defs import (
-    ResponseMetadataTypeDef,
-    AddCommunicationToCaseRequestRequestTypeDef,
-    AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
-    BlobTypeDef,
-    CategoryTypeDef,
-    DateIntervalTypeDef,
-    SupportedHourTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestRequestTypeDef,
-    DescribeCreateCaseOptionsRequestRequestTypeDef,
-    DescribeServicesRequestRequestTypeDef,
-    DescribeSeverityLevelsRequestRequestTypeDef,
-    SeverityLevelTypeDef,
-    DescribeSupportedLanguagesRequestRequestTypeDef,
-    SupportedLanguageTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
-    TrustedAdvisorCheckRefreshStatusTypeDef,
-    DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
-    DescribeTrustedAdvisorChecksRequestRequestTypeDef,
-    TrustedAdvisorCheckDescriptionTypeDef,
-    RefreshTrustedAdvisorCheckRequestRequestTypeDef,
-    ResolveCaseRequestRequestTypeDef,
-    TrustedAdvisorCostOptimizingSummaryTypeDef,
-    TrustedAdvisorResourceDetailTypeDef,
-    TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    ResolveCaseResponseTypeDef,
-    CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
-    AttachmentTypeDef,
-    ServiceTypeDef,
-    CommunicationTypeOptionsTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    DescribeSeverityLevelsResponseTypeDef,
-    DescribeSupportedLanguagesResponseTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
-    RefreshTrustedAdvisorCheckResponseTypeDef,
-    DescribeTrustedAdvisorChecksResponseTypeDef,
-    TrustedAdvisorCategorySpecificSummaryTypeDef,
-    DescribeCommunicationsResponseTypeDef,
-    RecentCaseCommunicationsTypeDef,
-    AttachmentUnionTypeDef,
-    DescribeServicesResponseTypeDef,
-    DescribeCreateCaseOptionsResponseTypeDef,
-    TrustedAdvisorCheckResultTypeDef,
-    TrustedAdvisorCheckSummaryTypeDef,
-    CaseDetailsTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckResultResponseTypeDef,
-    DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
-    DescribeCasesResponseTypeDef,
-)
+from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-support-2.5.2.post1/setup.py` & `types-aiobotocore-support-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__init__.pyi` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/__main__.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Support 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Support 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentUnionTypeDef,
+    AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -86,15 +86,15 @@
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#exceptions)
         """
 
     async def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_attachments_to_set)
         """
```

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/client.pyi` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 from .type_defs import (
     AddAttachmentsToSetResponseTypeDef,
     AddCommunicationToCaseResponseTypeDef,
-    AttachmentUnionTypeDef,
+    AttachmentTypeDef,
     CreateCaseResponseTypeDef,
     DescribeAttachmentResponseTypeDef,
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     DescribeCreateCaseOptionsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
@@ -81,15 +81,15 @@
         """
         SupportClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#exceptions)
         """
     async def add_attachments_to_set(
-        self, *, attachments: Sequence[AttachmentUnionTypeDef], attachmentSetId: str = ...
+        self, *, attachments: Sequence[AttachmentTypeDef], attachmentSetId: str = ...
     ) -> AddAttachmentsToSetResponseTypeDef:
         """
         Adds one or more attachments to an attachment set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_attachments_to_set)
         """
```

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/literals.pyi` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
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
@@ -144,14 +145,15 @@
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
@@ -230,26 +232,28 @@
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

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/paginator.pyi` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.py` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
-    "AttachmentOutputTypeDef",
     "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -54,35 +53,34 @@
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
-    "AttachmentUnionTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -124,23 +122,14 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
@@ -468,22 +457,14 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": str,
         "data": BlobTypeDef,
     },
     total=False,
@@ -610,15 +591,44 @@
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -684,36 +694,14 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[AttachmentUnionTypeDef],
-    },
-)
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachmentSetId": str,
-    },
-    total=False,
-)
-
-
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support/type_defs.pyi` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
-    "AttachmentOutputTypeDef",
     "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -53,35 +52,34 @@
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetResponseTypeDef",
     "AddCommunicationToCaseResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
-    "DescribeAttachmentResponseTypeDef",
     "AttachmentTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
     "DescribeCasesRequestDescribeCasesPaginateTypeDef",
     "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
     "RecentCaseCommunicationsTypeDef",
-    "AttachmentUnionTypeDef",
+    "AddAttachmentsToSetRequestRequestTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "DescribeCreateCaseOptionsResponseTypeDef",
     "TrustedAdvisorCheckResultTypeDef",
     "TrustedAdvisorCheckSummaryTypeDef",
     "CaseDetailsTypeDef",
-    "AddAttachmentsToSetRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     "DescribeCasesResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -121,23 +119,14 @@
     {
         "attachmentId": str,
         "fileName": str,
     },
     total=False,
 )
 
-AttachmentOutputTypeDef = TypedDict(
-    "AttachmentOutputTypeDef",
-    {
-        "fileName": str,
-        "data": bytes,
-    },
-    total=False,
-)
-
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
         "code": str,
         "name": str,
     },
@@ -457,22 +446,14 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
-    {
-        "attachment": AttachmentOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "fileName": str,
         "data": BlobTypeDef,
     },
     total=False,
@@ -597,15 +578,42 @@
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-AttachmentUnionTypeDef = Union[AttachmentTypeDef, AttachmentOutputTypeDef]
+_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachments": Sequence[AttachmentTypeDef],
+    },
+)
+_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
+    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
+    {
+        "attachmentSetId": str,
+    },
+    total=False,
+)
+
+class AddAttachmentsToSetRequestRequestTypeDef(
+    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
+    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
+):
+    pass
+
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -669,34 +677,14 @@
         "recentCommunications": RecentCaseCommunicationsTypeDef,
         "ccEmailAddresses": List[str],
         "language": str,
     },
     total=False,
 )
 
-_RequiredAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_RequiredAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachments": Sequence[AttachmentUnionTypeDef],
-    },
-)
-_OptionalAddAttachmentsToSetRequestRequestTypeDef = TypedDict(
-    "_OptionalAddAttachmentsToSetRequestRequestTypeDef",
-    {
-        "attachmentSetId": str,
-    },
-    total=False,
-)
-
-class AddAttachmentsToSetRequestRequestTypeDef(
-    _RequiredAddAttachmentsToSetRequestRequestTypeDef,
-    _OptionalAddAttachmentsToSetRequestRequestTypeDef,
-):
-    pass
-
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/PKG-INFO` & `types-aiobotocore-support-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-support
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,98 +262,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Support` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/literals/).
+
 ```python
-from types_aiobotocore_support.literals import (
-    DescribeCasesPaginatorName,
-    DescribeCommunicationsPaginatorName,
-    SupportServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_support.literals import DescribeCasesPaginatorName
 
 
 def check_value(value: DescribeCasesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Support` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/type_defs/).
+
 ```python
-from types_aiobotocore_support.type_defs import (
-    ResponseMetadataTypeDef,
-    AddCommunicationToCaseRequestRequestTypeDef,
-    AttachmentDetailsTypeDef,
-    AttachmentOutputTypeDef,
-    BlobTypeDef,
-    CategoryTypeDef,
-    DateIntervalTypeDef,
-    SupportedHourTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    DescribeAttachmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestRequestTypeDef,
-    DescribeCreateCaseOptionsRequestRequestTypeDef,
-    DescribeServicesRequestRequestTypeDef,
-    DescribeSeverityLevelsRequestRequestTypeDef,
-    SeverityLevelTypeDef,
-    DescribeSupportedLanguagesRequestRequestTypeDef,
-    SupportedLanguageTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
-    TrustedAdvisorCheckRefreshStatusTypeDef,
-    DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
-    DescribeTrustedAdvisorChecksRequestRequestTypeDef,
-    TrustedAdvisorCheckDescriptionTypeDef,
-    RefreshTrustedAdvisorCheckRequestRequestTypeDef,
-    ResolveCaseRequestRequestTypeDef,
-    TrustedAdvisorCostOptimizingSummaryTypeDef,
-    TrustedAdvisorResourceDetailTypeDef,
-    TrustedAdvisorResourcesSummaryTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    ResolveCaseResponseTypeDef,
-    CommunicationTypeDef,
-    DescribeAttachmentResponseTypeDef,
-    AttachmentTypeDef,
-    ServiceTypeDef,
-    CommunicationTypeOptionsTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    DescribeSeverityLevelsResponseTypeDef,
-    DescribeSupportedLanguagesResponseTypeDef,
-    DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
-    RefreshTrustedAdvisorCheckResponseTypeDef,
-    DescribeTrustedAdvisorChecksResponseTypeDef,
-    TrustedAdvisorCategorySpecificSummaryTypeDef,
-    DescribeCommunicationsResponseTypeDef,
-    RecentCaseCommunicationsTypeDef,
-    AttachmentUnionTypeDef,
-    DescribeServicesResponseTypeDef,
-    DescribeCreateCaseOptionsResponseTypeDef,
-    TrustedAdvisorCheckResultTypeDef,
-    TrustedAdvisorCheckSummaryTypeDef,
-    CaseDetailsTypeDef,
-    AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeTrustedAdvisorCheckResultResponseTypeDef,
-    DescribeTrustedAdvisorCheckSummariesResponseTypeDef,
-    DescribeCasesResponseTypeDef,
-)
+from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-support-2.5.2.post1/types_aiobotocore_support.egg-info/SOURCES.txt` & `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

