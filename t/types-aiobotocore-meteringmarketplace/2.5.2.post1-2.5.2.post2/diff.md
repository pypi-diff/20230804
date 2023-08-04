# Comparing `tmp/types-aiobotocore-meteringmarketplace-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-meteringmarketplace-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-meteringmarketplace-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-meteringmarketplace-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1.tar` & `types-aiobotocore-meteringmarketplace-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.717521 types-aiobotocore-meteringmarketplace-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-08-02 14:52:40.713521 types-aiobotocore-meteringmarketplace-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.717521 types-aiobotocore-meteringmarketplace-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.713521 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:34.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.713521 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.000000 types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.346643 types-aiobotocore-meteringmarketplace-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12846 2023-08-04 13:59:18.346643 types-aiobotocore-meteringmarketplace-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11280 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.346643 types-aiobotocore-meteringmarketplace-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2132 2023-08-04 13:44:52.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.346643 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      538 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      537 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8016 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8004 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8422 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8420 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4905 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4896 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:53.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.346643 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12846 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.000000 types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/LICENSE` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/PKG-INFO` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-meteringmarketplace
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MarketplaceMetering 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MarketplaceMetering 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/
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
 [types-aiobotocore-meteringmarketplace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_meteringmarketplace.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceMetering` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/literals/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.literals import (
-    UsageRecordResultStatusType,
-    MarketplaceMeteringServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_meteringmarketplace.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceMetering` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/type_defs/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
-    MeterUsageResultTypeDef,
-    RegisterUsageResultTypeDef,
-    ResolveCustomerResultTypeDef,
-    UsageAllocationOutputTypeDef,
-    UsageAllocationTypeDef,
-    UsageRecordOutputTypeDef,
-    UsageAllocationUnionTypeDef,
-    UsageRecordTypeDef,
-    UsageRecordResultTypeDef,
-    MeterUsageRequestRequestTypeDef,
-    UsageRecordUnionTypeDef,
-    BatchMeterUsageResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
-)
+from types_aiobotocore_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/README.md` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/README.md`

 * *Files 10% similar despite different names*

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
 [types-aiobotocore-meteringmarketplace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,57 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_meteringmarketplace.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceMetering` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/literals/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.literals import (
-    UsageRecordResultStatusType,
-    MarketplaceMeteringServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_meteringmarketplace.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceMetering` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/type_defs/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
-    MeterUsageResultTypeDef,
-    RegisterUsageResultTypeDef,
-    ResolveCustomerResultTypeDef,
-    UsageAllocationOutputTypeDef,
-    UsageAllocationTypeDef,
-    UsageRecordOutputTypeDef,
-    UsageAllocationUnionTypeDef,
-    UsageRecordTypeDef,
-    UsageRecordResultTypeDef,
-    MeterUsageRequestRequestTypeDef,
-    UsageRecordUnionTypeDef,
-    BatchMeterUsageResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
-)
+from types_aiobotocore_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/setup.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-meteringmarketplace",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MarketplaceMetering 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__init__.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__init__.pyi` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/__main__.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MarketplaceMetering 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/client.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
     TimestampTypeDef,
-    UsageAllocationUnionTypeDef,
-    UsageRecordUnionTypeDef,
+    UsageAllocationTypeDef,
+    UsageRecordTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -75,15 +75,15 @@
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#exceptions)
         """
 
     async def batch_meter_usage(
-        self, *, UsageRecords: Sequence[UsageRecordUnionTypeDef], ProductCode: str
+        self, *, UsageRecords: Sequence[UsageRecordTypeDef], ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#batch_meter_usage)
@@ -123,15 +123,15 @@
         self,
         *,
         ProductCode: str,
         Timestamp: TimestampTypeDef,
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[UsageAllocationUnionTypeDef] = ...
+        UsageAllocations: Sequence[UsageAllocationTypeDef] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#meter_usage)
         """
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/client.pyi` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
     TimestampTypeDef,
-    UsageAllocationUnionTypeDef,
-    UsageRecordUnionTypeDef,
+    UsageAllocationTypeDef,
+    UsageRecordTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -71,15 +71,15 @@
         """
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#exceptions)
         """
     async def batch_meter_usage(
-        self, *, UsageRecords: Sequence[UsageRecordUnionTypeDef], ProductCode: str
+        self, *, UsageRecords: Sequence[UsageRecordTypeDef], ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#batch_meter_usage)
@@ -115,15 +115,15 @@
         self,
         *,
         ProductCode: str,
         Timestamp: TimestampTypeDef,
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[UsageAllocationUnionTypeDef] = ...
+        UsageAllocations: Sequence[UsageAllocationTypeDef] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/client/#meter_usage)
         """
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/literals.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/literals.py`

 * *Files 2% similar despite different names*

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
@@ -410,14 +414,15 @@
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

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/literals.pyi` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
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
@@ -142,14 +143,15 @@
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
@@ -228,26 +230,28 @@
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
@@ -408,14 +412,15 @@
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

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/type_defs.py` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,24 +28,20 @@
     "TimestampTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "TagTypeDef",
     "MeterUsageResultTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerResultTypeDef",
-    "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
-    "UsageRecordOutputTypeDef",
-    "UsageAllocationUnionTypeDef",
+    "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
-    "MeterUsageRequestRequestTypeDef",
-    "UsageRecordUnionTypeDef",
     "BatchMeterUsageResultTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -116,35 +112,14 @@
         "CustomerIdentifier": str,
         "ProductCode": str,
         "CustomerAWSAccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUsageAllocationOutputTypeDef = TypedDict(
-    "_RequiredUsageAllocationOutputTypeDef",
-    {
-        "AllocatedUsageQuantity": int,
-    },
-)
-_OptionalUsageAllocationOutputTypeDef = TypedDict(
-    "_OptionalUsageAllocationOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class UsageAllocationOutputTypeDef(
-    _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
-):
-    pass
-
-
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
@@ -156,39 +131,39 @@
 )
 
 
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
 
-_RequiredUsageRecordOutputTypeDef = TypedDict(
-    "_RequiredUsageRecordOutputTypeDef",
+_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
+    "_RequiredMeterUsageRequestRequestTypeDef",
     {
-        "Timestamp": datetime,
-        "CustomerIdentifier": str,
-        "Dimension": str,
+        "ProductCode": str,
+        "Timestamp": TimestampTypeDef,
+        "UsageDimension": str,
     },
 )
-_OptionalUsageRecordOutputTypeDef = TypedDict(
-    "_OptionalUsageRecordOutputTypeDef",
+_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
+    "_OptionalMeterUsageRequestRequestTypeDef",
     {
-        "Quantity": int,
-        "UsageAllocations": List[UsageAllocationOutputTypeDef],
+        "UsageQuantity": int,
+        "DryRun": bool,
+        "UsageAllocations": Sequence[UsageAllocationTypeDef],
     },
     total=False,
 )
 
 
-class UsageRecordOutputTypeDef(
-    _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
+class MeterUsageRequestRequestTypeDef(
+    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
 ):
     pass
 
 
-UsageAllocationUnionTypeDef = Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
 _RequiredUsageRecordTypeDef = TypedDict(
     "_RequiredUsageRecordTypeDef",
     {
         "Timestamp": TimestampTypeDef,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
@@ -203,59 +178,33 @@
 )
 
 
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
 
-UsageRecordResultTypeDef = TypedDict(
-    "UsageRecordResultTypeDef",
-    {
-        "UsageRecord": UsageRecordOutputTypeDef,
-        "MeteringRecordId": str,
-        "Status": UsageRecordResultStatusType,
-    },
-    total=False,
-)
-
-_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
-    "_RequiredMeterUsageRequestRequestTypeDef",
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
     {
+        "UsageRecords": Sequence[UsageRecordTypeDef],
         "ProductCode": str,
-        "Timestamp": TimestampTypeDef,
-        "UsageDimension": str,
     },
 )
-_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
-    "_OptionalMeterUsageRequestRequestTypeDef",
+
+UsageRecordResultTypeDef = TypedDict(
+    "UsageRecordResultTypeDef",
     {
-        "UsageQuantity": int,
-        "DryRun": bool,
-        "UsageAllocations": Sequence[UsageAllocationUnionTypeDef],
+        "UsageRecord": UsageRecordTypeDef,
+        "MeteringRecordId": str,
+        "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
-
-class MeterUsageRequestRequestTypeDef(
-    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
-):
-    pass
-
-
-UsageRecordUnionTypeDef = Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
-        "UnprocessedRecords": List[UsageRecordOutputTypeDef],
+        "UnprocessedRecords": List[UsageRecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
-    {
-        "UsageRecords": Sequence[UsageRecordUnionTypeDef],
-        "ProductCode": str,
-    },
-)
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace/type_defs.pyi` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -27,24 +27,20 @@
     "TimestampTypeDef",
     "RegisterUsageRequestRequestTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
     "TagTypeDef",
     "MeterUsageResultTypeDef",
     "RegisterUsageResultTypeDef",
     "ResolveCustomerResultTypeDef",
-    "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
-    "UsageRecordOutputTypeDef",
-    "UsageAllocationUnionTypeDef",
+    "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
+    "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
-    "MeterUsageRequestRequestTypeDef",
-    "UsageRecordUnionTypeDef",
     "BatchMeterUsageResultTypeDef",
-    "BatchMeterUsageRequestRequestTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -113,33 +109,14 @@
         "CustomerIdentifier": str,
         "ProductCode": str,
         "CustomerAWSAccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUsageAllocationOutputTypeDef = TypedDict(
-    "_RequiredUsageAllocationOutputTypeDef",
-    {
-        "AllocatedUsageQuantity": int,
-    },
-)
-_OptionalUsageAllocationOutputTypeDef = TypedDict(
-    "_OptionalUsageAllocationOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class UsageAllocationOutputTypeDef(
-    _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
-):
-    pass
-
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationTypeDef = TypedDict(
@@ -149,37 +126,37 @@
     },
     total=False,
 )
 
 class UsageAllocationTypeDef(_RequiredUsageAllocationTypeDef, _OptionalUsageAllocationTypeDef):
     pass
 
-_RequiredUsageRecordOutputTypeDef = TypedDict(
-    "_RequiredUsageRecordOutputTypeDef",
+_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
+    "_RequiredMeterUsageRequestRequestTypeDef",
     {
-        "Timestamp": datetime,
-        "CustomerIdentifier": str,
-        "Dimension": str,
+        "ProductCode": str,
+        "Timestamp": TimestampTypeDef,
+        "UsageDimension": str,
     },
 )
-_OptionalUsageRecordOutputTypeDef = TypedDict(
-    "_OptionalUsageRecordOutputTypeDef",
+_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
+    "_OptionalMeterUsageRequestRequestTypeDef",
     {
-        "Quantity": int,
-        "UsageAllocations": List[UsageAllocationOutputTypeDef],
+        "UsageQuantity": int,
+        "DryRun": bool,
+        "UsageAllocations": Sequence[UsageAllocationTypeDef],
     },
     total=False,
 )
 
-class UsageRecordOutputTypeDef(
-    _RequiredUsageRecordOutputTypeDef, _OptionalUsageRecordOutputTypeDef
+class MeterUsageRequestRequestTypeDef(
+    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
 ):
     pass
 
-UsageAllocationUnionTypeDef = Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
 _RequiredUsageRecordTypeDef = TypedDict(
     "_RequiredUsageRecordTypeDef",
     {
         "Timestamp": TimestampTypeDef,
         "CustomerIdentifier": str,
         "Dimension": str,
     },
@@ -192,57 +169,33 @@
     },
     total=False,
 )
 
 class UsageRecordTypeDef(_RequiredUsageRecordTypeDef, _OptionalUsageRecordTypeDef):
     pass
 
-UsageRecordResultTypeDef = TypedDict(
-    "UsageRecordResultTypeDef",
-    {
-        "UsageRecord": UsageRecordOutputTypeDef,
-        "MeteringRecordId": str,
-        "Status": UsageRecordResultStatusType,
-    },
-    total=False,
-)
-
-_RequiredMeterUsageRequestRequestTypeDef = TypedDict(
-    "_RequiredMeterUsageRequestRequestTypeDef",
+BatchMeterUsageRequestRequestTypeDef = TypedDict(
+    "BatchMeterUsageRequestRequestTypeDef",
     {
+        "UsageRecords": Sequence[UsageRecordTypeDef],
         "ProductCode": str,
-        "Timestamp": TimestampTypeDef,
-        "UsageDimension": str,
     },
 )
-_OptionalMeterUsageRequestRequestTypeDef = TypedDict(
-    "_OptionalMeterUsageRequestRequestTypeDef",
+
+UsageRecordResultTypeDef = TypedDict(
+    "UsageRecordResultTypeDef",
     {
-        "UsageQuantity": int,
-        "DryRun": bool,
-        "UsageAllocations": Sequence[UsageAllocationUnionTypeDef],
+        "UsageRecord": UsageRecordTypeDef,
+        "MeteringRecordId": str,
+        "Status": UsageRecordResultStatusType,
     },
     total=False,
 )
 
-class MeterUsageRequestRequestTypeDef(
-    _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
-):
-    pass
-
-UsageRecordUnionTypeDef = Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
-        "UnprocessedRecords": List[UsageRecordOutputTypeDef],
+        "UnprocessedRecords": List[UsageRecordTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-BatchMeterUsageRequestRequestTypeDef = TypedDict(
-    "BatchMeterUsageRequestRequestTypeDef",
-    {
-        "UsageRecords": Sequence[UsageRecordUnionTypeDef],
-        "ProductCode": str,
-    },
-)
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/PKG-INFO` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-meteringmarketplace
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MarketplaceMetering 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MarketplaceMetering 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/
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
 [types-aiobotocore-meteringmarketplace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_meteringmarketplace.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MarketplaceMetering` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/literals/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.literals import (
-    UsageRecordResultStatusType,
-    MarketplaceMeteringServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType
 
 
 def check_value(value: UsageRecordResultStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_meteringmarketplace.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MarketplaceMetering` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/type_defs/).
+
 ```python
-from types_aiobotocore_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
-    MeterUsageResultTypeDef,
-    RegisterUsageResultTypeDef,
-    ResolveCustomerResultTypeDef,
-    UsageAllocationOutputTypeDef,
-    UsageAllocationTypeDef,
-    UsageRecordOutputTypeDef,
-    UsageAllocationUnionTypeDef,
-    UsageRecordTypeDef,
-    UsageRecordResultTypeDef,
-    MeterUsageRequestRequestTypeDef,
-    UsageRecordUnionTypeDef,
-    BatchMeterUsageResultTypeDef,
-    BatchMeterUsageRequestRequestTypeDef,
-)
+from types_aiobotocore_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-meteringmarketplace-2.5.2.post1/types_aiobotocore_meteringmarketplace.egg-info/SOURCES.txt` & `types-aiobotocore-meteringmarketplace-2.5.2.post2/types_aiobotocore_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

