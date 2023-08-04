# Comparing `tmp/types-aiobotocore-payment-cryptography-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1.tar` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:46.017503 types-aiobotocore-payment-cryptography-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-08-02 14:52:46.017503 types-aiobotocore-payment-cryptography-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:46.017503 types-aiobotocore-payment-cryptography-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:46.017503 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-08-02 14:44:38.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24018 2023-08-02 14:44:38.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23994 2023-08-02 14:44:38.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:37.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:46.017503 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 14:52:45.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.796643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13216 2023-08-04 13:59:20.786643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11623 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.796643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2193 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.776643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      601 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      600 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1021 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14727 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14708 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8822 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8820 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24018 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23994 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.786643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13216 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1040 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       44 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/LICENSE` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/README.md` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-payment-cryptography-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore payment-cryptography-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-payment-cryptography-data"></a>
 
 # types-aiobotocore-payment-cryptography-data
 
 [![PyPI - types-aiobotocore-payment-cryptography-data](https://img.shields.io/pypi/v/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
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
 [types-aiobotocore-payment-cryptography-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -235,111 +267,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_payment_cryptography_data.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PaymentCryptographyDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/literals/).
+
 ```python
-from types_aiobotocore_payment_cryptography_data.literals import (
-    DukptDerivationTypeType,
-    DukptEncryptionModeType,
-    DukptKeyVariantType,
-    EncryptionModeType,
-    MacAlgorithmType,
-    MajorKeyDerivationModeType,
-    PaddingTypeType,
-    PinBlockFormatForPinDataType,
-    SessionKeyDerivationModeType,
-    PaymentCryptographyDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_payment_cryptography_data.literals import DukptDerivationTypeType
 
 
 def check_value(value: DukptDerivationTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_payment_cryptography_data.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `PaymentCryptographyDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/type_defs/).
+
 ```python
 from types_aiobotocore_payment_cryptography_data.type_defs import (
     AmexCardSecurityCodeVersion1TypeDef,
-    AmexCardSecurityCodeVersion2TypeDef,
-    AsymmetricEncryptionAttributesTypeDef,
-    CardHolderVerificationValueTypeDef,
-    CardVerificationValue1TypeDef,
-    CardVerificationValue2TypeDef,
-    DynamicCardVerificationCodeTypeDef,
-    DynamicCardVerificationValueTypeDef,
-    DiscoverDynamicCardVerificationCodeTypeDef,
-    CryptogramVerificationArpcMethod1TypeDef,
-    CryptogramVerificationArpcMethod2TypeDef,
-    ResponseMetadataTypeDef,
-    DukptAttributesTypeDef,
-    DukptDerivationAttributesTypeDef,
-    DukptEncryptionAttributesTypeDef,
-    SymmetricEncryptionAttributesTypeDef,
-    PinDataTypeDef,
-    Ibm3624NaturalPinTypeDef,
-    Ibm3624PinFromOffsetTypeDef,
-    Ibm3624PinOffsetTypeDef,
-    Ibm3624PinVerificationTypeDef,
-    Ibm3624RandomPinTypeDef,
-    MacAlgorithmDukptTypeDef,
-    SessionKeyDerivationValueTypeDef,
-    VisaPinTypeDef,
-    VisaPinVerificationValueTypeDef,
-    VisaPinVerificationTypeDef,
-    SessionKeyAmexTypeDef,
-    SessionKeyEmv2000TypeDef,
-    SessionKeyEmvCommonTypeDef,
-    SessionKeyMastercardTypeDef,
-    SessionKeyVisaTypeDef,
-    TranslationPinDataIsoFormat034TypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
-    DecryptDataOutputTypeDef,
-    EncryptDataOutputTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
-    ReEncryptDataOutputTypeDef,
-    TranslatePinDataOutputTypeDef,
-    VerifyAuthRequestCryptogramOutputTypeDef,
-    VerifyCardValidationDataOutputTypeDef,
-    VerifyMacOutputTypeDef,
-    VerifyPinDataOutputTypeDef,
-    EncryptionDecryptionAttributesTypeDef,
-    ReEncryptionAttributesTypeDef,
-    GeneratePinDataOutputTypeDef,
-    MacAlgorithmEmvTypeDef,
-    PinGenerationAttributesTypeDef,
-    PinVerificationAttributesTypeDef,
-    SessionKeyDerivationTypeDef,
-    TranslationIsoFormatsTypeDef,
-    GenerateCardValidationDataInputRequestTypeDef,
-    VerifyCardValidationDataInputRequestTypeDef,
-    DecryptDataInputRequestTypeDef,
-    EncryptDataInputRequestTypeDef,
-    ReEncryptDataInputRequestTypeDef,
-    MacAttributesTypeDef,
-    GeneratePinDataInputRequestTypeDef,
-    VerifyPinDataInputRequestTypeDef,
-    VerifyAuthRequestCryptogramInputRequestTypeDef,
-    TranslatePinDataInputRequestTypeDef,
-    GenerateMacInputRequestTypeDef,
-    VerifyMacInputRequestTypeDef,
 )
 
 
 def get_value() -> AmexCardSecurityCodeVersion1TypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/setup.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__init__.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__init__.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/__main__.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/client.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/client.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/literals.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DukptDerivationTypeType",
     "DukptEncryptionModeType",
     "DukptKeyVariantType",
     "EncryptionModeType",
     "MacAlgorithmType",
     "MajorKeyDerivationModeType",
@@ -30,15 +29,14 @@
     "PinBlockFormatForPinDataType",
     "SessionKeyDerivationModeType",
     "PaymentCryptographyDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 DukptDerivationTypeType = Literal["AES_128", "AES_192", "AES_256", "TDES_2KEY", "TDES_3KEY"]
 DukptEncryptionModeType = Literal["CBC", "ECB"]
 DukptKeyVariantType = Literal["BIDIRECTIONAL", "REQUEST", "RESPONSE"]
 EncryptionModeType = Literal["CBC", "CFB", "CFB1", "CFB128", "CFB64", "CFB8", "ECB", "OFB"]
 MacAlgorithmType = Literal[
     "CMAC",
     "HMAC_SHA224",
@@ -66,14 +64,15 @@
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
@@ -169,14 +168,15 @@
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
@@ -255,26 +255,28 @@
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/literals.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DukptDerivationTypeType",
     "DukptEncryptionModeType",
     "DukptKeyVariantType",
     "EncryptionModeType",
     "MacAlgorithmType",
     "MajorKeyDerivationModeType",
@@ -29,14 +30,15 @@
     "PinBlockFormatForPinDataType",
     "SessionKeyDerivationModeType",
     "PaymentCryptographyDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
+
 DukptDerivationTypeType = Literal["AES_128", "AES_192", "AES_256", "TDES_2KEY", "TDES_3KEY"]
 DukptEncryptionModeType = Literal["CBC", "ECB"]
 DukptKeyVariantType = Literal["BIDIRECTIONAL", "REQUEST", "RESPONSE"]
 EncryptionModeType = Literal["CBC", "CFB", "CFB1", "CFB128", "CFB64", "CFB8", "ECB", "OFB"]
 MacAlgorithmType = Literal[
     "CMAC",
     "HMAC_SHA224",
@@ -64,14 +66,15 @@
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
@@ -167,14 +170,15 @@
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
@@ -253,26 +257,28 @@
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/type_defs.py` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data/type_defs.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post1/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

