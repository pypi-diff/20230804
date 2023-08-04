# Comparing `tmp/types-aiobotocore-cloudcontrol-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudcontrol-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1.tar` & `types-aiobotocore-cloudcontrol-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.667427 types-aiobotocore-cloudcontrol-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-08-04 12:00:33.667427 types-aiobotocore-cloudcontrol-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.667427 types-aiobotocore-cloudcontrol-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.663427 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-04 11:41:34.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-04 11:41:34.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-04 11:41:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.667427 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:33.000000 types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudcontrol-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.2.post2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,70 +320,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudcontrol.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudControlApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/literals/).
+
 ```python
-from types_aiobotocore_cloudcontrol.literals import (
-    HandlerErrorCodeType,
-    ListResourceRequestsPaginatorName,
-    ListResourcesPaginatorName,
-    OperationStatusType,
-    OperationType,
-    ResourceRequestSuccessWaiterName,
-    CloudControlApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_cloudcontrol.literals import HandlerErrorCodeType
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudControlApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/type_defs/).
+
 ```python
-from types_aiobotocore_cloudcontrol.type_defs import (
-    CancelResourceRequestInputRequestTypeDef,
-    ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
-    CreateResourceInputRequestTypeDef,
-    DeleteResourceInputRequestTypeDef,
-    GetResourceInputRequestTypeDef,
-    ResourceDescriptionTypeDef,
-    GetResourceRequestStatusInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputRequestTypeDef,
-    UpdateResourceInputRequestTypeDef,
-    CancelResourceRequestOutputTypeDef,
-    CreateResourceOutputTypeDef,
-    DeleteResourceOutputTypeDef,
-    GetResourceRequestStatusOutputTypeDef,
-    ListResourceRequestsOutputTypeDef,
-    UpdateResourceOutputTypeDef,
-    GetResourceOutputTypeDef,
-    ListResourcesOutputTypeDef,
-    GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
-    ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
-    ListResourceRequestsInputRequestTypeDef,
-)
+from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef
 
 
 def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/README.md` & `types-aiobotocore-cloudcontrol-2.5.2.post2/README.md`

 * *Files 11% similar despite different names*

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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,70 +288,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudcontrol.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudControlApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/literals/).
+
 ```python
-from types_aiobotocore_cloudcontrol.literals import (
-    HandlerErrorCodeType,
-    ListResourceRequestsPaginatorName,
-    ListResourcesPaginatorName,
-    OperationStatusType,
-    OperationType,
-    ResourceRequestSuccessWaiterName,
-    CloudControlApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_cloudcontrol.literals import HandlerErrorCodeType
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudControlApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/type_defs/).
+
 ```python
-from types_aiobotocore_cloudcontrol.type_defs import (
-    CancelResourceRequestInputRequestTypeDef,
-    ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
-    CreateResourceInputRequestTypeDef,
-    DeleteResourceInputRequestTypeDef,
-    GetResourceInputRequestTypeDef,
-    ResourceDescriptionTypeDef,
-    GetResourceRequestStatusInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputRequestTypeDef,
-    UpdateResourceInputRequestTypeDef,
-    CancelResourceRequestOutputTypeDef,
-    CreateResourceOutputTypeDef,
-    DeleteResourceOutputTypeDef,
-    GetResourceRequestStatusOutputTypeDef,
-    ListResourceRequestsOutputTypeDef,
-    UpdateResourceOutputTypeDef,
-    GetResourceOutputTypeDef,
-    ListResourcesOutputTypeDef,
-    GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
-    ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
-    ListResourceRequestsInputRequestTypeDef,
-)
+from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef
 
 
 def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/setup.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudcontrol",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__main__.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudControlApi 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.py` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,70 +320,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudcontrol.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudControlApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/literals/).
+
 ```python
-from types_aiobotocore_cloudcontrol.literals import (
-    HandlerErrorCodeType,
-    ListResourceRequestsPaginatorName,
-    ListResourcesPaginatorName,
-    OperationStatusType,
-    OperationType,
-    ResourceRequestSuccessWaiterName,
-    CloudControlApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_cloudcontrol.literals import HandlerErrorCodeType
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudControlApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/type_defs/).
+
 ```python
-from types_aiobotocore_cloudcontrol.type_defs import (
-    CancelResourceRequestInputRequestTypeDef,
-    ProgressEventTypeDef,
-    ResponseMetadataTypeDef,
-    CreateResourceInputRequestTypeDef,
-    DeleteResourceInputRequestTypeDef,
-    GetResourceInputRequestTypeDef,
-    ResourceDescriptionTypeDef,
-    GetResourceRequestStatusInputRequestTypeDef,
-    WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
-    ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputRequestTypeDef,
-    UpdateResourceInputRequestTypeDef,
-    CancelResourceRequestOutputTypeDef,
-    CreateResourceOutputTypeDef,
-    DeleteResourceOutputTypeDef,
-    GetResourceRequestStatusOutputTypeDef,
-    ListResourceRequestsOutputTypeDef,
-    UpdateResourceOutputTypeDef,
-    GetResourceOutputTypeDef,
-    ListResourcesOutputTypeDef,
-    GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
-    ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
-    ListResourceRequestsInputRequestTypeDef,
-)
+from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef
 
 
 def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt` & `types-aiobotocore-cloudcontrol-2.5.2.post2/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

