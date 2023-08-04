# Comparing `tmp/types-aiobotocore-acm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-acm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-acm-2.5.2.post1.tar` & `types-aiobotocore-acm-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-02 14:32:42.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:51:47.000000 types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.746887 types-aiobotocore-acm-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-04 12:00:19.742887 types-aiobotocore-acm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.746887 types-aiobotocore-acm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.734887 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-04 11:39:47.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-04 11:39:47.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-04 11:39:46.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.742887 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:19.000000 types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-2.5.2.post1/LICENSE` & `types-aiobotocore-acm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/PKG-INFO` & `types-aiobotocore-acm-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,97 +314,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_acm.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `ACM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/literals/).
+
 ```python
-from types_aiobotocore_acm.literals import (
-    CertificateStatusType,
-    CertificateTransparencyLoggingPreferenceType,
-    CertificateTypeType,
-    CertificateValidatedWaiterName,
-    DomainStatusType,
-    ExtendedKeyUsageNameType,
-    FailureReasonType,
-    KeyAlgorithmType,
-    KeyUsageNameType,
-    ListCertificatesPaginatorName,
-    RecordTypeType,
-    RenewalEligibilityType,
-    RenewalStatusType,
-    RevocationReasonType,
-    SortByType,
-    SortOrderType,
-    ValidationMethodType,
-    ACMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_acm.literals import CertificateStatusType
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ACM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/type_defs/).
+
 ```python
-from types_aiobotocore_acm.type_defs import (
-    TagTypeDef,
-    BlobTypeDef,
-    CertificateOptionsTypeDef,
-    ExtendedKeyUsageTypeDef,
-    KeyUsageTypeDef,
-    CertificateSummaryTypeDef,
-    DeleteCertificateRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCertificateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DomainValidationOptionTypeDef,
-    ResourceRecordTypeDef,
-    ExpiryEventsConfigurationTypeDef,
-    FiltersTypeDef,
-    GetCertificateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForCertificateRequestRequestTypeDef,
-    RenewCertificateRequestRequestTypeDef,
-    ResendValidationEmailRequestRequestTypeDef,
-    AddTagsToCertificateRequestRequestTypeDef,
-    RemoveTagsFromCertificateRequestRequestTypeDef,
-    ExportCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
-    UpdateCertificateOptionsRequestRequestTypeDef,
-    DescribeCertificateRequestCertificateValidatedWaitTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportCertificateResponseTypeDef,
-    GetCertificateResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
-    RequestCertificateResponseTypeDef,
-    RequestCertificateRequestRequestTypeDef,
-    DomainValidationTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    PutAccountConfigurationRequestRequestTypeDef,
-    ListCertificatesRequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
-    RenewalSummaryTypeDef,
-    CertificateDetailTypeDef,
-    DescribeCertificateResponseTypeDef,
-)
+from types_aiobotocore_acm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-acm-2.5.2.post1/README.md` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-acm
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore acm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,97 +314,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_acm.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `ACM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/literals/).
+
 ```python
-from types_aiobotocore_acm.literals import (
-    CertificateStatusType,
-    CertificateTransparencyLoggingPreferenceType,
-    CertificateTypeType,
-    CertificateValidatedWaiterName,
-    DomainStatusType,
-    ExtendedKeyUsageNameType,
-    FailureReasonType,
-    KeyAlgorithmType,
-    KeyUsageNameType,
-    ListCertificatesPaginatorName,
-    RecordTypeType,
-    RenewalEligibilityType,
-    RenewalStatusType,
-    RevocationReasonType,
-    SortByType,
-    SortOrderType,
-    ValidationMethodType,
-    ACMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_acm.literals import CertificateStatusType
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ACM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/type_defs/).
+
 ```python
-from types_aiobotocore_acm.type_defs import (
-    TagTypeDef,
-    BlobTypeDef,
-    CertificateOptionsTypeDef,
-    ExtendedKeyUsageTypeDef,
-    KeyUsageTypeDef,
-    CertificateSummaryTypeDef,
-    DeleteCertificateRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCertificateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DomainValidationOptionTypeDef,
-    ResourceRecordTypeDef,
-    ExpiryEventsConfigurationTypeDef,
-    FiltersTypeDef,
-    GetCertificateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForCertificateRequestRequestTypeDef,
-    RenewCertificateRequestRequestTypeDef,
-    ResendValidationEmailRequestRequestTypeDef,
-    AddTagsToCertificateRequestRequestTypeDef,
-    RemoveTagsFromCertificateRequestRequestTypeDef,
-    ExportCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
-    UpdateCertificateOptionsRequestRequestTypeDef,
-    DescribeCertificateRequestCertificateValidatedWaitTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportCertificateResponseTypeDef,
-    GetCertificateResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
-    RequestCertificateResponseTypeDef,
-    RequestCertificateRequestRequestTypeDef,
-    DomainValidationTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    PutAccountConfigurationRequestRequestTypeDef,
-    ListCertificatesRequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
-    RenewalSummaryTypeDef,
-    CertificateDetailTypeDef,
-    DescribeCertificateResponseTypeDef,
-)
+from types_aiobotocore_acm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-acm-2.5.2.post1/setup.py` & `types-aiobotocore-acm-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__init__.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/__main__.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ACM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/client.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/literals.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/paginator.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/type_defs.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.py` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm/waiter.pyi` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/PKG-INFO` & `types-aiobotocore-acm-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-acm
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore acm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm"></a>
 
 # types-aiobotocore-acm
 
 [![PyPI - types-aiobotocore-acm](https://img.shields.io/pypi/v/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
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
 [types-aiobotocore-acm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,97 +282,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_acm.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `ACM` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/literals/).
+
 ```python
-from types_aiobotocore_acm.literals import (
-    CertificateStatusType,
-    CertificateTransparencyLoggingPreferenceType,
-    CertificateTypeType,
-    CertificateValidatedWaiterName,
-    DomainStatusType,
-    ExtendedKeyUsageNameType,
-    FailureReasonType,
-    KeyAlgorithmType,
-    KeyUsageNameType,
-    ListCertificatesPaginatorName,
-    RecordTypeType,
-    RenewalEligibilityType,
-    RenewalStatusType,
-    RevocationReasonType,
-    SortByType,
-    SortOrderType,
-    ValidationMethodType,
-    ACMServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_acm.literals import CertificateStatusType
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_acm.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ACM` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/type_defs/).
+
 ```python
-from types_aiobotocore_acm.type_defs import (
-    TagTypeDef,
-    BlobTypeDef,
-    CertificateOptionsTypeDef,
-    ExtendedKeyUsageTypeDef,
-    KeyUsageTypeDef,
-    CertificateSummaryTypeDef,
-    DeleteCertificateRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCertificateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DomainValidationOptionTypeDef,
-    ResourceRecordTypeDef,
-    ExpiryEventsConfigurationTypeDef,
-    FiltersTypeDef,
-    GetCertificateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForCertificateRequestRequestTypeDef,
-    RenewCertificateRequestRequestTypeDef,
-    ResendValidationEmailRequestRequestTypeDef,
-    AddTagsToCertificateRequestRequestTypeDef,
-    RemoveTagsFromCertificateRequestRequestTypeDef,
-    ExportCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
-    UpdateCertificateOptionsRequestRequestTypeDef,
-    DescribeCertificateRequestCertificateValidatedWaitTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportCertificateResponseTypeDef,
-    GetCertificateResponseTypeDef,
-    ImportCertificateResponseTypeDef,
-    ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
-    RequestCertificateResponseTypeDef,
-    RequestCertificateRequestRequestTypeDef,
-    DomainValidationTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    PutAccountConfigurationRequestRequestTypeDef,
-    ListCertificatesRequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
-    RenewalSummaryTypeDef,
-    CertificateDetailTypeDef,
-    DescribeCertificateResponseTypeDef,
-)
+from types_aiobotocore_acm.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-acm-2.5.2.post1/types_aiobotocore_acm.egg-info/SOURCES.txt` & `types-aiobotocore-acm-2.5.2.post2/types_aiobotocore_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

