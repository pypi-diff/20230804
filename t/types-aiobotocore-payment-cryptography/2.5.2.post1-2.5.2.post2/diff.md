# Comparing `tmp/types-aiobotocore-payment-cryptography-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1.tar` & `types-aiobotocore-payment-cryptography-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.325499 types-aiobotocore-payment-cryptography-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-08-02 14:52:47.325499 types-aiobotocore-payment-cryptography-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.325499 types-aiobotocore-payment-cryptography-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.321499 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:36.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.325499 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:47.000000 types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14028 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12447 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2166 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.896643 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1173 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1172 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1017 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19845 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19813 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9922 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9920 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4539 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4534 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17665 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17641 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14028 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1060 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       39 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/LICENSE` & `types-aiobotocore-payment-cryptography-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,107 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_payment_cryptography.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PaymentCryptographyControlPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/literals/).
+
 ```python
-from types_aiobotocore_payment_cryptography.literals import (
-    KeyAlgorithmType,
-    KeyCheckValueAlgorithmType,
-    KeyClassType,
-    KeyMaterialTypeType,
-    KeyOriginType,
-    KeyStateType,
-    KeyUsageType,
-    ListAliasesPaginatorName,
-    ListKeysPaginatorName,
-    ListTagsForResourcePaginatorName,
-    Tr34KeyBlockFormatType,
-    WrappedKeyMaterialFormatType,
-    PaymentCryptographyControlPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_payment_cryptography.literals import KeyAlgorithmType
 
 
 def check_value(value: KeyAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_payment_cryptography.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PaymentCryptographyControlPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/type_defs/).
+
 ```python
-from types_aiobotocore_payment_cryptography.type_defs import (
-    AliasTypeDef,
-    CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DeleteAliasInputRequestTypeDef,
-    DeleteKeyInputRequestTypeDef,
-    ExportTr31KeyBlockTypeDef,
-    ExportTr34KeyBlockTypeDef,
-    WrappedKeyTypeDef,
-    GetAliasInputRequestTypeDef,
-    GetKeyInputRequestTypeDef,
-    GetParametersForExportInputRequestTypeDef,
-    GetParametersForImportInputRequestTypeDef,
-    GetPublicKeyCertificateInputRequestTypeDef,
-    ImportTr31KeyBlockTypeDef,
-    ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
-    ListAliasesInputRequestTypeDef,
-    ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RestoreKeyInputRequestTypeDef,
-    StartKeyUsageInputRequestTypeDef,
-    StopKeyUsageInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateAliasInputRequestTypeDef,
-    CreateAliasOutputTypeDef,
-    GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
-    ListAliasesOutputTypeDef,
-    UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
-    ExportKeyMaterialTypeDef,
-    ExportKeyOutputTypeDef,
-    KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
-    KeySummaryTypeDef,
-    KeyTypeDef,
-    RootCertificatePublicKeyTypeDef,
-    TrustedCertificatePublicKeyTypeDef,
-    ListKeysOutputTypeDef,
-    CreateKeyOutputTypeDef,
-    DeleteKeyOutputTypeDef,
-    GetKeyOutputTypeDef,
-    ImportKeyOutputTypeDef,
-    RestoreKeyOutputTypeDef,
-    StartKeyUsageOutputTypeDef,
-    StopKeyUsageOutputTypeDef,
-    ImportKeyMaterialTypeDef,
-    ImportKeyInputRequestTypeDef,
-)
+from types_aiobotocore_payment_cryptography.type_defs import AliasTypeDef
 
 
 def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/README.md` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-payment-cryptography
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore payment-cryptography type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-payment-cryptography"></a>
 
 # types-aiobotocore-payment-cryptography
 
 [![PyPI - types-aiobotocore-payment-cryptography](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,107 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_payment_cryptography.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PaymentCryptographyControlPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/literals/).
+
 ```python
-from types_aiobotocore_payment_cryptography.literals import (
-    KeyAlgorithmType,
-    KeyCheckValueAlgorithmType,
-    KeyClassType,
-    KeyMaterialTypeType,
-    KeyOriginType,
-    KeyStateType,
-    KeyUsageType,
-    ListAliasesPaginatorName,
-    ListKeysPaginatorName,
-    ListTagsForResourcePaginatorName,
-    Tr34KeyBlockFormatType,
-    WrappedKeyMaterialFormatType,
-    PaymentCryptographyControlPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_payment_cryptography.literals import KeyAlgorithmType
 
 
 def check_value(value: KeyAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_payment_cryptography.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PaymentCryptographyControlPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/type_defs/).
+
 ```python
-from types_aiobotocore_payment_cryptography.type_defs import (
-    AliasTypeDef,
-    CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DeleteAliasInputRequestTypeDef,
-    DeleteKeyInputRequestTypeDef,
-    ExportTr31KeyBlockTypeDef,
-    ExportTr34KeyBlockTypeDef,
-    WrappedKeyTypeDef,
-    GetAliasInputRequestTypeDef,
-    GetKeyInputRequestTypeDef,
-    GetParametersForExportInputRequestTypeDef,
-    GetParametersForImportInputRequestTypeDef,
-    GetPublicKeyCertificateInputRequestTypeDef,
-    ImportTr31KeyBlockTypeDef,
-    ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
-    ListAliasesInputRequestTypeDef,
-    ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RestoreKeyInputRequestTypeDef,
-    StartKeyUsageInputRequestTypeDef,
-    StopKeyUsageInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateAliasInputRequestTypeDef,
-    CreateAliasOutputTypeDef,
-    GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
-    ListAliasesOutputTypeDef,
-    UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
-    ExportKeyMaterialTypeDef,
-    ExportKeyOutputTypeDef,
-    KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
-    KeySummaryTypeDef,
-    KeyTypeDef,
-    RootCertificatePublicKeyTypeDef,
-    TrustedCertificatePublicKeyTypeDef,
-    ListKeysOutputTypeDef,
-    CreateKeyOutputTypeDef,
-    DeleteKeyOutputTypeDef,
-    GetKeyOutputTypeDef,
-    ImportKeyOutputTypeDef,
-    RestoreKeyOutputTypeDef,
-    StartKeyUsageOutputTypeDef,
-    StopKeyUsageOutputTypeDef,
-    ImportKeyMaterialTypeDef,
-    ImportKeyInputRequestTypeDef,
-)
+from types_aiobotocore_payment_cryptography.type_defs import AliasTypeDef
 
 
 def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/setup.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated"
-        " with mypy-boto3-builder 7.17.1"
+        " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__init__.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__init__.pyi` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/__main__.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/client.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/client.pyi` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/literals.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
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
@@ -196,14 +197,15 @@
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
@@ -282,26 +284,28 @@
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

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/literals.pyi` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
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
@@ -194,14 +195,15 @@
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
@@ -280,26 +282,28 @@
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

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/paginator.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/paginator.pyi` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/type_defs.py` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography/type_defs.pyi` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.2.post2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-payment-cryptography
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore payment-cryptography type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-payment-cryptography"></a>
 
 # types-aiobotocore-payment-cryptography
 
 [![PyPI - types-aiobotocore-payment-cryptography](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
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
 [types-aiobotocore-payment-cryptography docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,107 +265,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_payment_cryptography.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PaymentCryptographyControlPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/literals/).
+
 ```python
-from types_aiobotocore_payment_cryptography.literals import (
-    KeyAlgorithmType,
-    KeyCheckValueAlgorithmType,
-    KeyClassType,
-    KeyMaterialTypeType,
-    KeyOriginType,
-    KeyStateType,
-    KeyUsageType,
-    ListAliasesPaginatorName,
-    ListKeysPaginatorName,
-    ListTagsForResourcePaginatorName,
-    Tr34KeyBlockFormatType,
-    WrappedKeyMaterialFormatType,
-    PaymentCryptographyControlPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_payment_cryptography.literals import KeyAlgorithmType
 
 
 def check_value(value: KeyAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_payment_cryptography.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PaymentCryptographyControlPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/type_defs/).
+
 ```python
-from types_aiobotocore_payment_cryptography.type_defs import (
-    AliasTypeDef,
-    CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DeleteAliasInputRequestTypeDef,
-    DeleteKeyInputRequestTypeDef,
-    ExportTr31KeyBlockTypeDef,
-    ExportTr34KeyBlockTypeDef,
-    WrappedKeyTypeDef,
-    GetAliasInputRequestTypeDef,
-    GetKeyInputRequestTypeDef,
-    GetParametersForExportInputRequestTypeDef,
-    GetParametersForImportInputRequestTypeDef,
-    GetPublicKeyCertificateInputRequestTypeDef,
-    ImportTr31KeyBlockTypeDef,
-    ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
-    ListAliasesInputRequestTypeDef,
-    ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    RestoreKeyInputRequestTypeDef,
-    StartKeyUsageInputRequestTypeDef,
-    StopKeyUsageInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateAliasInputRequestTypeDef,
-    CreateAliasOutputTypeDef,
-    GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
-    ListAliasesOutputTypeDef,
-    UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
-    ExportKeyMaterialTypeDef,
-    ExportKeyOutputTypeDef,
-    KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
-    KeySummaryTypeDef,
-    KeyTypeDef,
-    RootCertificatePublicKeyTypeDef,
-    TrustedCertificatePublicKeyTypeDef,
-    ListKeysOutputTypeDef,
-    CreateKeyOutputTypeDef,
-    DeleteKeyOutputTypeDef,
-    GetKeyOutputTypeDef,
-    ImportKeyOutputTypeDef,
-    RestoreKeyOutputTypeDef,
-    StartKeyUsageOutputTypeDef,
-    StopKeyUsageOutputTypeDef,
-    ImportKeyMaterialTypeDef,
-    ImportKeyInputRequestTypeDef,
-)
+from types_aiobotocore_payment_cryptography.type_defs import AliasTypeDef
 
 
 def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post1/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

