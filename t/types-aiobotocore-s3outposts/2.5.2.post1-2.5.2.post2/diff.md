# Comparing `tmp/types-aiobotocore-s3outposts-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-s3outposts-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3outposts-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3outposts-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
```

## Comparing `types-aiobotocore-s3outposts-2.5.2.post1.tar` & `types-aiobotocore-s3outposts-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.489470 types-aiobotocore-s3outposts-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-02 14:52:56.489470 types-aiobotocore-s3outposts-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:56.489470 types-aiobotocore-s3outposts-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:48:29.000000 types-aiobotocore-s3outposts-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.469471 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:30.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.489470 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:56.000000 types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3outposts-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13439 2023-08-04 13:59:24.836643 types-aiobotocore-s3outposts-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11909 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.836643 types-aiobotocore-s3outposts-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1129 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1128 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9035 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9018 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8740 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8738 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4280 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4275 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6507 2023-08-04 13:51:46.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6500 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:45.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13439 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:24.000000 types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/LICENSE` & `types-aiobotocore-s3outposts-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/PKG-INFO` & `types-aiobotocore-s3outposts-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3outposts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.S3Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.S3Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/
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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,62 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_s3outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `S3Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/literals/).
+
 ```python
-from types_aiobotocore_s3outposts.literals import (
-    EndpointAccessTypeType,
-    EndpointStatusType,
-    ListEndpointsPaginatorName,
-    ListOutpostsWithS3PaginatorName,
-    ListSharedEndpointsPaginatorName,
-    S3OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_s3outposts.literals import EndpointAccessTypeType
 
 
 def check_value(value: EndpointAccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `S3Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/type_defs/).
+
 ```python
-from types_aiobotocore_s3outposts.type_defs import (
-    CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteEndpointRequestRequestTypeDef,
-    FailedReasonTypeDef,
-    NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestRequestTypeDef,
-    OutpostTypeDef,
-    ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    ListOutpostsWithS3ResultTypeDef,
-    ListEndpointsResultTypeDef,
-    ListSharedEndpointsResultTypeDef,
-)
+from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestRequestTypeDef
 
 
 def get_value() -> CreateEndpointRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/README.md` & `types-aiobotocore-s3outposts-2.5.2.post2/README.md`

 * *Files 6% similar despite different names*

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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,62 +267,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_s3outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `S3Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/literals/).
+
 ```python
-from types_aiobotocore_s3outposts.literals import (
-    EndpointAccessTypeType,
-    EndpointStatusType,
-    ListEndpointsPaginatorName,
-    ListOutpostsWithS3PaginatorName,
-    ListSharedEndpointsPaginatorName,
-    S3OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_s3outposts.literals import EndpointAccessTypeType
 
 
 def check_value(value: EndpointAccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `S3Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/type_defs/).
+
 ```python
-from types_aiobotocore_s3outposts.type_defs import (
-    CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteEndpointRequestRequestTypeDef,
-    FailedReasonTypeDef,
-    NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestRequestTypeDef,
-    OutpostTypeDef,
-    ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    ListOutpostsWithS3ResultTypeDef,
-    ListEndpointsResultTypeDef,
-    ListSharedEndpointsResultTypeDef,
-)
+from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestRequestTypeDef
 
 
 def get_value() -> CreateEndpointRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/setup.py` & `types-aiobotocore-s3outposts-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3outposts",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_s3outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.S3Outposts 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__init__.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__init__.pyi` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/__main__.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3Outposts 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.S3Outposts 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts\nOther"
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

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/client.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/client.pyi` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/literals.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "EndpointAccessTypeType",
     "EndpointStatusType",
     "ListEndpointsPaginatorName",
     "ListOutpostsWithS3PaginatorName",
     "ListSharedEndpointsPaginatorName",
     "S3OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 EndpointAccessTypeType = Literal["CustomerOwnedIp", "Private"]
 EndpointStatusType = Literal["Available", "Create_Failed", "Delete_Failed", "Deleting", "Pending"]
 ListEndpointsPaginatorName = Literal["list_endpoints"]
 ListOutpostsWithS3PaginatorName = Literal["list_outposts_with_s3"]
 ListSharedEndpointsPaginatorName = Literal["list_shared_endpoints"]
 S3OutpostsServiceName = Literal["s3outposts"]
 ServiceName = Literal[
@@ -50,14 +48,15 @@
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
@@ -153,14 +152,15 @@
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
@@ -239,26 +239,28 @@
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

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/literals.pyi` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "EndpointAccessTypeType",
     "EndpointStatusType",
     "ListEndpointsPaginatorName",
     "ListOutpostsWithS3PaginatorName",
     "ListSharedEndpointsPaginatorName",
     "S3OutpostsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 EndpointAccessTypeType = Literal["CustomerOwnedIp", "Private"]
 EndpointStatusType = Literal["Available", "Create_Failed", "Delete_Failed", "Deleting", "Pending"]
 ListEndpointsPaginatorName = Literal["list_endpoints"]
 ListOutpostsWithS3PaginatorName = Literal["list_outposts_with_s3"]
 ListSharedEndpointsPaginatorName = Literal["list_shared_endpoints"]
 S3OutpostsServiceName = Literal["s3outposts"]
 ServiceName = Literal[
@@ -48,14 +50,15 @@
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
@@ -151,14 +154,15 @@
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
@@ -237,26 +241,28 @@
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

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/paginator.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/paginator.pyi` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/type_defs.py` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts/type_defs.pyi` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/PKG-INFO` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3outposts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.S3Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.S3Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/
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
 [types-aiobotocore-s3outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,62 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_s3outposts.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `S3Outposts` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/literals/).
+
 ```python
-from types_aiobotocore_s3outposts.literals import (
-    EndpointAccessTypeType,
-    EndpointStatusType,
-    ListEndpointsPaginatorName,
-    ListOutpostsWithS3PaginatorName,
-    ListSharedEndpointsPaginatorName,
-    S3OutpostsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_s3outposts.literals import EndpointAccessTypeType
 
 
 def check_value(value: EndpointAccessTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_s3outposts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `S3Outposts` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3outposts/type_defs/).
+
 ```python
-from types_aiobotocore_s3outposts.type_defs import (
-    CreateEndpointRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteEndpointRequestRequestTypeDef,
-    FailedReasonTypeDef,
-    NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
-    ListEndpointsRequestRequestTypeDef,
-    ListOutpostsWithS3RequestRequestTypeDef,
-    OutpostTypeDef,
-    ListSharedEndpointsRequestRequestTypeDef,
-    CreateEndpointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointTypeDef,
-    ListEndpointsRequestListEndpointsPaginateTypeDef,
-    ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef,
-    ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef,
-    ListOutpostsWithS3ResultTypeDef,
-    ListEndpointsResultTypeDef,
-    ListSharedEndpointsResultTypeDef,
-)
+from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestRequestTypeDef
 
 
 def get_value() -> CreateEndpointRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-s3outposts-2.5.2.post1/types_aiobotocore_s3outposts.egg-info/SOURCES.txt` & `types-aiobotocore-s3outposts-2.5.2.post2/types_aiobotocore_s3outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

