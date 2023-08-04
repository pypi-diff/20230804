# Comparing `tmp/types-aiobotocore-savingsplans-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-savingsplans-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-savingsplans-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-savingsplans-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-savingsplans-2.5.2.post1.tar` & `types-aiobotocore-savingsplans-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.785467 types-aiobotocore-savingsplans-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-08-02 14:52:57.785467 types-aiobotocore-savingsplans-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.785467 types-aiobotocore-savingsplans-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:49:01.000000 types-aiobotocore-savingsplans-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.777467 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:02.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.785467 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:57.000000 types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.466643 types-aiobotocore-savingsplans-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2023-08-04 13:59:25.466643 types-aiobotocore-savingsplans-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10901 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.466643 types-aiobotocore-savingsplans-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.466643 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      482 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      481 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11362 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11345 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9484 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9482 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11506 2023-08-04 13:52:33.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11501 2023-08-04 13:52:33.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:32.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.466643 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:25.000000 types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/LICENSE` & `types-aiobotocore-savingsplans-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/PKG-INFO` & `types-aiobotocore-savingsplans-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-savingsplans
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SavingsPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SavingsPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/
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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,78 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_savingsplans.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SavingsPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/literals/).
+
 ```python
-from types_aiobotocore_savingsplans.literals import (
-    CurrencyCodeType,
-    SavingsPlanOfferingFilterAttributeType,
-    SavingsPlanOfferingPropertyKeyType,
-    SavingsPlanPaymentOptionType,
-    SavingsPlanProductTypeType,
-    SavingsPlanRateFilterAttributeType,
-    SavingsPlanRateFilterNameType,
-    SavingsPlanRatePropertyKeyType,
-    SavingsPlanRateServiceCodeType,
-    SavingsPlanRateUnitType,
-    SavingsPlanStateType,
-    SavingsPlanTypeType,
-    SavingsPlansFilterNameType,
-    SavingsPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_savingsplans.literals import CurrencyCodeType
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_savingsplans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SavingsPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/type_defs/).
+
 ```python
-from types_aiobotocore_savingsplans.type_defs import (
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteQueuedSavingsPlanRequestRequestTypeDef,
-    SavingsPlanRateFilterTypeDef,
-    SavingsPlanOfferingRateFilterElementTypeDef,
-    SavingsPlanOfferingFilterElementTypeDef,
-    SavingsPlanFilterTypeDef,
-    SavingsPlanTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ParentSavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingPropertyTypeDef,
-    SavingsPlanOfferingRatePropertyTypeDef,
-    SavingsPlanRatePropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DescribeSavingsPlanRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingsRequestRequestTypeDef,
-    DescribeSavingsPlansRequestRequestTypeDef,
-    DescribeSavingsPlansResponseTypeDef,
-    SavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingRateTypeDef,
-    SavingsPlanRateTypeDef,
-    DescribeSavingsPlansOfferingsResponseTypeDef,
-    DescribeSavingsPlansOfferingRatesResponseTypeDef,
-    DescribeSavingsPlanRatesResponseTypeDef,
-)
+from types_aiobotocore_savingsplans.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/README.md` & `types-aiobotocore-savingsplans-2.5.2.post2/README.md`

 * *Files 16% similar despite different names*

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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,78 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_savingsplans.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SavingsPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/literals/).
+
 ```python
-from types_aiobotocore_savingsplans.literals import (
-    CurrencyCodeType,
-    SavingsPlanOfferingFilterAttributeType,
-    SavingsPlanOfferingPropertyKeyType,
-    SavingsPlanPaymentOptionType,
-    SavingsPlanProductTypeType,
-    SavingsPlanRateFilterAttributeType,
-    SavingsPlanRateFilterNameType,
-    SavingsPlanRatePropertyKeyType,
-    SavingsPlanRateServiceCodeType,
-    SavingsPlanRateUnitType,
-    SavingsPlanStateType,
-    SavingsPlanTypeType,
-    SavingsPlansFilterNameType,
-    SavingsPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_savingsplans.literals import CurrencyCodeType
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_savingsplans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SavingsPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/type_defs/).
+
 ```python
-from types_aiobotocore_savingsplans.type_defs import (
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteQueuedSavingsPlanRequestRequestTypeDef,
-    SavingsPlanRateFilterTypeDef,
-    SavingsPlanOfferingRateFilterElementTypeDef,
-    SavingsPlanOfferingFilterElementTypeDef,
-    SavingsPlanFilterTypeDef,
-    SavingsPlanTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ParentSavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingPropertyTypeDef,
-    SavingsPlanOfferingRatePropertyTypeDef,
-    SavingsPlanRatePropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DescribeSavingsPlanRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingsRequestRequestTypeDef,
-    DescribeSavingsPlansRequestRequestTypeDef,
-    DescribeSavingsPlansResponseTypeDef,
-    SavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingRateTypeDef,
-    SavingsPlanRateTypeDef,
-    DescribeSavingsPlansOfferingsResponseTypeDef,
-    DescribeSavingsPlansOfferingRatesResponseTypeDef,
-    DescribeSavingsPlanRatesResponseTypeDef,
-)
+from types_aiobotocore_savingsplans.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/setup.py` & `types-aiobotocore-savingsplans-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-savingsplans",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_savingsplans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SavingsPlans 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/__main__.py` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SavingsPlans 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SavingsPlans 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans\nOther"
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

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/client.py` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/client.pyi` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/literals.py` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/literals.pyi` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
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
@@ -192,14 +193,15 @@
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
@@ -278,26 +280,28 @@
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

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/type_defs.py` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans/type_defs.pyi` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/PKG-INFO` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-savingsplans
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SavingsPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SavingsPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/
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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,78 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_savingsplans.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SavingsPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/literals/).
+
 ```python
-from types_aiobotocore_savingsplans.literals import (
-    CurrencyCodeType,
-    SavingsPlanOfferingFilterAttributeType,
-    SavingsPlanOfferingPropertyKeyType,
-    SavingsPlanPaymentOptionType,
-    SavingsPlanProductTypeType,
-    SavingsPlanRateFilterAttributeType,
-    SavingsPlanRateFilterNameType,
-    SavingsPlanRatePropertyKeyType,
-    SavingsPlanRateServiceCodeType,
-    SavingsPlanRateUnitType,
-    SavingsPlanStateType,
-    SavingsPlanTypeType,
-    SavingsPlansFilterNameType,
-    SavingsPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_savingsplans.literals import CurrencyCodeType
 
 
 def check_value(value: CurrencyCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_savingsplans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SavingsPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/type_defs/).
+
 ```python
-from types_aiobotocore_savingsplans.type_defs import (
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteQueuedSavingsPlanRequestRequestTypeDef,
-    SavingsPlanRateFilterTypeDef,
-    SavingsPlanOfferingRateFilterElementTypeDef,
-    SavingsPlanOfferingFilterElementTypeDef,
-    SavingsPlanFilterTypeDef,
-    SavingsPlanTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ParentSavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingPropertyTypeDef,
-    SavingsPlanOfferingRatePropertyTypeDef,
-    SavingsPlanRatePropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSavingsPlanRequestRequestTypeDef,
-    CreateSavingsPlanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DescribeSavingsPlanRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingRatesRequestRequestTypeDef,
-    DescribeSavingsPlansOfferingsRequestRequestTypeDef,
-    DescribeSavingsPlansRequestRequestTypeDef,
-    DescribeSavingsPlansResponseTypeDef,
-    SavingsPlanOfferingTypeDef,
-    SavingsPlanOfferingRateTypeDef,
-    SavingsPlanRateTypeDef,
-    DescribeSavingsPlansOfferingsResponseTypeDef,
-    DescribeSavingsPlansOfferingRatesResponseTypeDef,
-    DescribeSavingsPlanRatesResponseTypeDef,
-)
+from types_aiobotocore_savingsplans.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-savingsplans-2.5.2.post1/types_aiobotocore_savingsplans.egg-info/SOURCES.txt` & `types-aiobotocore-savingsplans-2.5.2.post2/types_aiobotocore_savingsplans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

