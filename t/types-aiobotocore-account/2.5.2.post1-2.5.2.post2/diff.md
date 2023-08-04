# Comparing `tmp/types-aiobotocore-account-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-account-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-account-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-account-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-account-2.5.2.post1.tar` & `types-aiobotocore-account-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-account-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.845667 types-aiobotocore-account-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.718886 types-aiobotocore-account-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-08-04 12:00:19.718886 types-aiobotocore-account-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.718886 types-aiobotocore-account-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.718886 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:45.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.718886 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:19.000000 types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-account-2.5.2.post1/LICENSE` & `types-aiobotocore-account-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/PKG-INFO` & `types-aiobotocore-account-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,60 +288,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_account.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Account` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/literals/).
+
 ```python
-from types_aiobotocore_account.literals import (
-    AlternateContactTypeType,
-    ListRegionsPaginatorName,
-    RegionOptStatusType,
-    AccountServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_account.literals import AlternateContactTypeType
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Account` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/type_defs/).
+
 ```python
-from types_aiobotocore_account.type_defs import (
-    AlternateContactTypeDef,
-    ContactInformationTypeDef,
-    DeleteAlternateContactRequestRequestTypeDef,
-    DisableRegionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableRegionRequestRequestTypeDef,
-    GetAlternateContactRequestRequestTypeDef,
-    GetContactInformationRequestRequestTypeDef,
-    GetRegionOptStatusRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRegionsRequestRequestTypeDef,
-    RegionTypeDef,
-    PutAlternateContactRequestRequestTypeDef,
-    PutContactInformationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAlternateContactResponseTypeDef,
-    GetContactInformationResponseTypeDef,
-    GetRegionOptStatusResponseTypeDef,
-    ListRegionsRequestListRegionsPaginateTypeDef,
-    ListRegionsResponseTypeDef,
-)
+from types_aiobotocore_account.type_defs import AlternateContactTypeDef
 
 
 def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-account-2.5.2.post1/README.md` & `types-aiobotocore-account-2.5.2.post2/README.md`

 * *Files 8% similar despite different names*

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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,60 +256,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_account.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Account` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/literals/).
+
 ```python
-from types_aiobotocore_account.literals import (
-    AlternateContactTypeType,
-    ListRegionsPaginatorName,
-    RegionOptStatusType,
-    AccountServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_account.literals import AlternateContactTypeType
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Account` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/type_defs/).
+
 ```python
-from types_aiobotocore_account.type_defs import (
-    AlternateContactTypeDef,
-    ContactInformationTypeDef,
-    DeleteAlternateContactRequestRequestTypeDef,
-    DisableRegionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableRegionRequestRequestTypeDef,
-    GetAlternateContactRequestRequestTypeDef,
-    GetContactInformationRequestRequestTypeDef,
-    GetRegionOptStatusRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRegionsRequestRequestTypeDef,
-    RegionTypeDef,
-    PutAlternateContactRequestRequestTypeDef,
-    PutContactInformationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAlternateContactResponseTypeDef,
-    GetContactInformationResponseTypeDef,
-    GetRegionOptStatusResponseTypeDef,
-    ListRegionsRequestListRegionsPaginateTypeDef,
-    ListRegionsResponseTypeDef,
-)
+from types_aiobotocore_account.type_defs import AlternateContactTypeDef
 
 
 def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-account-2.5.2.post1/setup.py` & `types-aiobotocore-account-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-account",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.pyi` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__main__.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Account 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Account 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
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

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.pyi` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.pyi` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.pyi` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.py` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.pyi` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/PKG-INFO` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,60 +288,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_account.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Account` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/literals/).
+
 ```python
-from types_aiobotocore_account.literals import (
-    AlternateContactTypeType,
-    ListRegionsPaginatorName,
-    RegionOptStatusType,
-    AccountServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_account.literals import AlternateContactTypeType
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Account` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/type_defs/).
+
 ```python
-from types_aiobotocore_account.type_defs import (
-    AlternateContactTypeDef,
-    ContactInformationTypeDef,
-    DeleteAlternateContactRequestRequestTypeDef,
-    DisableRegionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableRegionRequestRequestTypeDef,
-    GetAlternateContactRequestRequestTypeDef,
-    GetContactInformationRequestRequestTypeDef,
-    GetRegionOptStatusRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRegionsRequestRequestTypeDef,
-    RegionTypeDef,
-    PutAlternateContactRequestRequestTypeDef,
-    PutContactInformationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAlternateContactResponseTypeDef,
-    GetContactInformationResponseTypeDef,
-    GetRegionOptStatusResponseTypeDef,
-    ListRegionsRequestListRegionsPaginateTypeDef,
-    ListRegionsResponseTypeDef,
-)
+from types_aiobotocore_account.type_defs import AlternateContactTypeDef
 
 
 def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/SOURCES.txt` & `types-aiobotocore-account-2.5.2.post2/types_aiobotocore_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

