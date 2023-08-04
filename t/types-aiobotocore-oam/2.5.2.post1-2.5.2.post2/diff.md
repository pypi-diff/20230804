# Comparing `tmp/types-aiobotocore-oam-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-oam-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-oam-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-oam-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-oam-2.5.2.post1.tar` & `types-aiobotocore-oam-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.709510 types-aiobotocore-oam-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.709510 types-aiobotocore-oam-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-02 14:44:12.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13313 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11778 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2053 2023-08-04 13:45:47.000000 types-aiobotocore-oam-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1127 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1126 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      982 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14752 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14725 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8741 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8739 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4190 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4185 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9647 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9638 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13313 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-oam-2.5.2.post1/LICENSE` & `types-aiobotocore-oam-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/PKG-INFO` & `types-aiobotocore-oam-2.5.2.post2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,76 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_oam.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/literals/).
+
 ```python
-from types_aiobotocore_oam.literals import (
-    ListAttachedLinksPaginatorName,
-    ListLinksPaginatorName,
-    ListSinksPaginatorName,
-    ResourceTypeType,
-    CloudWatchObservabilityAccessManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_oam.literals import ListAttachedLinksPaginatorName
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/type_defs/).
+
 ```python
-from types_aiobotocore_oam.type_defs import (
-    CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateSinkInputRequestTypeDef,
-    DeleteLinkInputRequestTypeDef,
-    DeleteSinkInputRequestTypeDef,
-    GetLinkInputRequestTypeDef,
-    GetSinkInputRequestTypeDef,
-    GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAttachedLinksInputRequestTypeDef,
-    ListAttachedLinksItemTypeDef,
-    ListLinksInputRequestTypeDef,
-    ListLinksItemTypeDef,
-    ListSinksInputRequestTypeDef,
-    ListSinksItemTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    PutSinkPolicyInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
-    ListAttachedLinksOutputTypeDef,
-    ListLinksOutputTypeDef,
-    ListSinksOutputTypeDef,
-)
+from types_aiobotocore_oam.type_defs import CreateLinkInputRequestTypeDef
 
 
 def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-oam-2.5.2.post1/README.md` & `types-aiobotocore-oam-2.5.2.post2/README.md`

 * *Files 12% similar despite different names*

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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,76 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_oam.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/literals/).
+
 ```python
-from types_aiobotocore_oam.literals import (
-    ListAttachedLinksPaginatorName,
-    ListLinksPaginatorName,
-    ListSinksPaginatorName,
-    ResourceTypeType,
-    CloudWatchObservabilityAccessManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_oam.literals import ListAttachedLinksPaginatorName
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/type_defs/).
+
 ```python
-from types_aiobotocore_oam.type_defs import (
-    CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateSinkInputRequestTypeDef,
-    DeleteLinkInputRequestTypeDef,
-    DeleteSinkInputRequestTypeDef,
-    GetLinkInputRequestTypeDef,
-    GetSinkInputRequestTypeDef,
-    GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAttachedLinksInputRequestTypeDef,
-    ListAttachedLinksItemTypeDef,
-    ListLinksInputRequestTypeDef,
-    ListLinksItemTypeDef,
-    ListSinksInputRequestTypeDef,
-    ListSinksItemTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    PutSinkPolicyInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
-    ListAttachedLinksOutputTypeDef,
-    ListLinksOutputTypeDef,
-    ListSinksOutputTypeDef,
-)
+from types_aiobotocore_oam.type_defs import CreateLinkInputRequestTypeDef
 
 
 def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-oam-2.5.2.post1/setup.py` & `types-aiobotocore-oam-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-oam",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_oam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service"
-        " generated with mypy-boto3-builder 7.17.1"
+        " generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.pyi` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__main__.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2\nVersion:     "
-        "    2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        "    2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager\nOther"
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

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.pyi` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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
@@ -418,14 +422,15 @@
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

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.pyi` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -235,26 +237,28 @@
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
@@ -416,14 +420,15 @@
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

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.pyi` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.py` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.pyi` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/PKG-INFO` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,76 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_oam.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/literals/).
+
 ```python
-from types_aiobotocore_oam.literals import (
-    ListAttachedLinksPaginatorName,
-    ListLinksPaginatorName,
-    ListSinksPaginatorName,
-    ResourceTypeType,
-    CloudWatchObservabilityAccessManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_oam.literals import ListAttachedLinksPaginatorName
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchObservabilityAccessManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/type_defs/).
+
 ```python
-from types_aiobotocore_oam.type_defs import (
-    CreateLinkInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateSinkInputRequestTypeDef,
-    DeleteLinkInputRequestTypeDef,
-    DeleteSinkInputRequestTypeDef,
-    GetLinkInputRequestTypeDef,
-    GetSinkInputRequestTypeDef,
-    GetSinkPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAttachedLinksInputRequestTypeDef,
-    ListAttachedLinksItemTypeDef,
-    ListLinksInputRequestTypeDef,
-    ListLinksItemTypeDef,
-    ListSinksInputRequestTypeDef,
-    ListSinksItemTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    PutSinkPolicyInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
-    CreateSinkOutputTypeDef,
-    GetLinkOutputTypeDef,
-    GetSinkOutputTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    UpdateLinkOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
-    ListAttachedLinksOutputTypeDef,
-    ListLinksOutputTypeDef,
-    ListSinksOutputTypeDef,
-)
+from types_aiobotocore_oam.type_defs import CreateLinkInputRequestTypeDef
 
 
 def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/SOURCES.txt` & `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

