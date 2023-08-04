# Comparing `tmp/types-aiobotocore-mediastore-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediastore-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediastore-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediastore-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-mediastore-2.5.2.post1.tar` & `types-aiobotocore-mediastore-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.277522 types-aiobotocore-mediastore-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-08-02 14:52:40.273522 types-aiobotocore-mediastore-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.277522 types-aiobotocore-mediastore-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.273522 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:26.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.273522 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:40.000000 types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13080 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11550 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      671 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      670 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16111 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16080 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8280 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8278 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2014 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2011 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9296 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9287 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13080 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/LICENSE` & `types-aiobotocore-mediastore-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/PKG-INFO` & `types-aiobotocore-mediastore-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,83 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediastore.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MediaStore` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/literals/).
+
 ```python
-from types_aiobotocore_mediastore.literals import (
-    ContainerLevelMetricsType,
-    ContainerStatusType,
-    ListContainersPaginatorName,
-    MethodNameType,
-    MediaStoreServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediastore.literals import ContainerLevelMetricsType
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaStore` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/type_defs/).
+
 ```python
-from types_aiobotocore_mediastore.type_defs import (
-    ContainerTypeDef,
-    CorsRuleOutputTypeDef,
-    CorsRuleTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteContainerInputRequestTypeDef,
-    DeleteContainerPolicyInputRequestTypeDef,
-    DeleteCorsPolicyInputRequestTypeDef,
-    DeleteLifecyclePolicyInputRequestTypeDef,
-    DeleteMetricPolicyInputRequestTypeDef,
-    DescribeContainerInputRequestTypeDef,
-    GetContainerPolicyInputRequestTypeDef,
-    GetCorsPolicyInputRequestTypeDef,
-    GetLifecyclePolicyInputRequestTypeDef,
-    GetMetricPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListContainersInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    MetricPolicyRuleTypeDef,
-    PutContainerPolicyInputRequestTypeDef,
-    PutLifecyclePolicyInputRequestTypeDef,
-    StartAccessLoggingInputRequestTypeDef,
-    StopAccessLoggingInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CorsRuleUnionTypeDef,
-    CreateContainerInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    GetContainerPolicyOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
-    ListContainersOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
-    MetricPolicyOutputTypeDef,
-    MetricPolicyTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
-    GetMetricPolicyOutputTypeDef,
-    MetricPolicyUnionTypeDef,
-    PutMetricPolicyInputRequestTypeDef,
-)
+from types_aiobotocore_mediastore.type_defs import ContainerTypeDef
 
 
 def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/README.md` & `types-aiobotocore-mediastore-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,83 +257,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediastore.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MediaStore` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/literals/).
+
 ```python
-from types_aiobotocore_mediastore.literals import (
-    ContainerLevelMetricsType,
-    ContainerStatusType,
-    ListContainersPaginatorName,
-    MethodNameType,
-    MediaStoreServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediastore.literals import ContainerLevelMetricsType
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaStore` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/type_defs/).
+
 ```python
-from types_aiobotocore_mediastore.type_defs import (
-    ContainerTypeDef,
-    CorsRuleOutputTypeDef,
-    CorsRuleTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteContainerInputRequestTypeDef,
-    DeleteContainerPolicyInputRequestTypeDef,
-    DeleteCorsPolicyInputRequestTypeDef,
-    DeleteLifecyclePolicyInputRequestTypeDef,
-    DeleteMetricPolicyInputRequestTypeDef,
-    DescribeContainerInputRequestTypeDef,
-    GetContainerPolicyInputRequestTypeDef,
-    GetCorsPolicyInputRequestTypeDef,
-    GetLifecyclePolicyInputRequestTypeDef,
-    GetMetricPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListContainersInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    MetricPolicyRuleTypeDef,
-    PutContainerPolicyInputRequestTypeDef,
-    PutLifecyclePolicyInputRequestTypeDef,
-    StartAccessLoggingInputRequestTypeDef,
-    StopAccessLoggingInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CorsRuleUnionTypeDef,
-    CreateContainerInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    GetContainerPolicyOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
-    ListContainersOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
-    MetricPolicyOutputTypeDef,
-    MetricPolicyTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
-    GetMetricPolicyOutputTypeDef,
-    MetricPolicyUnionTypeDef,
-    PutMetricPolicyInputRequestTypeDef,
-)
+from types_aiobotocore_mediastore.type_defs import ContainerTypeDef
 
 
 def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/setup.py` & `types-aiobotocore-mediastore-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediastore",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaStore 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__init__.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__init__.pyi` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/__main__.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaStore 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaStore 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/client.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
-    CorsRuleUnionTypeDef,
+    CorsRuleTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    MetricPolicyUnionTypeDef,
+    MetricPolicyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -227,15 +227,15 @@
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_container_policy)
         """
 
     async def put_cors_policy(
-        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleUnionTypeDef]
+        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_cors_policy)
@@ -248,15 +248,15 @@
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_lifecycle_policy)
         """
 
     async def put_metric_policy(
-        self, *, ContainerName: str, MetricPolicy: MetricPolicyUnionTypeDef
+        self, *, ContainerName: str, MetricPolicy: MetricPolicyTypeDef
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_metric_policy)
         """
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/client.pyi` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListContainersPaginator
 from .type_defs import (
-    CorsRuleUnionTypeDef,
+    CorsRuleTypeDef,
     CreateContainerOutputTypeDef,
     DescribeContainerOutputTypeDef,
     GetContainerPolicyOutputTypeDef,
     GetCorsPolicyOutputTypeDef,
     GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyOutputTypeDef,
     ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    MetricPolicyUnionTypeDef,
+    MetricPolicyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -205,15 +205,15 @@
         Creates an access policy for the specified container to restrict the users and
         clients that can access it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_container_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_container_policy)
         """
     async def put_cors_policy(
-        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleUnionTypeDef]
+        self, *, ContainerName: str, CorsPolicy: Sequence[CorsRuleTypeDef]
     ) -> Dict[str, Any]:
         """
         Sets the cross-origin resource sharing (CORS) configuration on a container so
         that the container can service cross-origin requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_cors_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_cors_policy)
@@ -224,15 +224,15 @@
         """
         Writes an object lifecycle policy to a container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_lifecycle_policy)
         """
     async def put_metric_policy(
-        self, *, ContainerName: str, MetricPolicy: MetricPolicyUnionTypeDef
+        self, *, ContainerName: str, MetricPolicy: MetricPolicyTypeDef
     ) -> Dict[str, Any]:
         """
         The metric policy that you want to add to the container.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client.put_metric_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/client/#put_metric_policy)
         """
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/literals.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.py`

 * *Files 2% similar despite different names*

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
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/literals.pyi` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.pyi`

 * *Files 2% similar despite different names*

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
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/paginator.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/paginator.pyi` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/type_defs.py` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,26 @@
     from types_aiobotocore_mediastore.type_defs import ContainerTypeDef
 
     data: ContainerTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ContainerTypeDef",
-    "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
@@ -44,30 +43,27 @@
     "ListTagsForResourceInputRequestTypeDef",
     "MetricPolicyRuleTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CorsRuleUnionTypeDef",
+    "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
-    "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
-    "PutCorsPolicyInputRequestTypeDef",
     "GetMetricPolicyOutputTypeDef",
-    "MetricPolicyUnionTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "Endpoint": str,
@@ -76,49 +72,27 @@
         "Name": str,
         "Status": ContainerStatusType,
         "AccessLoggingEnabled": bool,
     },
     total=False,
 )
 
-_RequiredCorsRuleOutputTypeDef = TypedDict(
-    "_RequiredCorsRuleOutputTypeDef",
-    {
-        "AllowedOrigins": List[str],
-        "AllowedHeaders": List[str],
-    },
-)
-_OptionalCorsRuleOutputTypeDef = TypedDict(
-    "_OptionalCorsRuleOutputTypeDef",
-    {
-        "AllowedMethods": List[MethodNameType],
-        "MaxAgeSeconds": int,
-        "ExposeHeaders": List[str],
-    },
-    total=False,
-)
-
-
-class CorsRuleOutputTypeDef(_RequiredCorsRuleOutputTypeDef, _OptionalCorsRuleOutputTypeDef):
-    pass
-
-
 _RequiredCorsRuleTypeDef = TypedDict(
     "_RequiredCorsRuleTypeDef",
     {
-        "AllowedOrigins": Sequence[str],
-        "AllowedHeaders": Sequence[str],
+        "AllowedOrigins": List[str],
+        "AllowedHeaders": List[str],
     },
 )
 _OptionalCorsRuleTypeDef = TypedDict(
     "_OptionalCorsRuleTypeDef",
     {
-        "AllowedMethods": Sequence[MethodNameType],
+        "AllowedMethods": List[MethodNameType],
         "MaxAgeSeconds": int,
-        "ExposeHeaders": Sequence[str],
+        "ExposeHeaders": List[str],
     },
     total=False,
 )
 
 
 class CorsRuleTypeDef(_RequiredCorsRuleTypeDef, _OptionalCorsRuleTypeDef):
     pass
@@ -293,15 +267,22 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-CorsRuleUnionTypeDef = Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]
+PutCorsPolicyInputRequestTypeDef = TypedDict(
+    "PutCorsPolicyInputRequestTypeDef",
+    {
+        "ContainerName": str,
+        "CorsPolicy": Sequence[CorsRuleTypeDef],
+    },
+)
+
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 _OptionalCreateContainerInputRequestTypeDef = TypedDict(
@@ -350,15 +331,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCorsPolicyOutputTypeDef = TypedDict(
     "GetCorsPolicyOutputTypeDef",
     {
-        "CorsPolicy": List[CorsRuleOutputTypeDef],
+        "CorsPolicy": List[CorsRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyOutputTypeDef = TypedDict(
     "GetLifecyclePolicyOutputTypeDef",
     {
@@ -388,71 +369,41 @@
     "ListContainersInputListContainersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredMetricPolicyOutputTypeDef = TypedDict(
-    "_RequiredMetricPolicyOutputTypeDef",
-    {
-        "ContainerLevelMetrics": ContainerLevelMetricsType,
-    },
-)
-_OptionalMetricPolicyOutputTypeDef = TypedDict(
-    "_OptionalMetricPolicyOutputTypeDef",
-    {
-        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
-    },
-    total=False,
-)
-
-
-class MetricPolicyOutputTypeDef(
-    _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricPolicyTypeDef = TypedDict(
     "_RequiredMetricPolicyTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyTypeDef = TypedDict(
     "_OptionalMetricPolicyTypeDef",
     {
-        "MetricPolicyRules": Sequence[MetricPolicyRuleTypeDef],
+        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
 
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
 
-PutCorsPolicyInputRequestTypeDef = TypedDict(
-    "PutCorsPolicyInputRequestTypeDef",
-    {
-        "ContainerName": str,
-        "CorsPolicy": Sequence[CorsRuleUnionTypeDef],
-    },
-)
-
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
-        "MetricPolicy": MetricPolicyOutputTypeDef,
+        "MetricPolicy": MetricPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricPolicyUnionTypeDef = Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "MetricPolicy": MetricPolicyTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore/type_defs.pyi` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
     from types_aiobotocore_mediastore.type_defs import ContainerTypeDef
 
     data: ContainerTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ContainerLevelMetricsType, ContainerStatusType, MethodNameType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ContainerTypeDef",
-    "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
@@ -43,30 +42,27 @@
     "ListTagsForResourceInputRequestTypeDef",
     "MetricPolicyRuleTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CorsRuleUnionTypeDef",
+    "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateContainerOutputTypeDef",
     "DescribeContainerOutputTypeDef",
     "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyOutputTypeDef",
     "GetLifecyclePolicyOutputTypeDef",
     "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListContainersInputListContainersPaginateTypeDef",
-    "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
-    "PutCorsPolicyInputRequestTypeDef",
     "GetMetricPolicyOutputTypeDef",
-    "MetricPolicyUnionTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "Endpoint": str,
@@ -75,47 +71,27 @@
         "Name": str,
         "Status": ContainerStatusType,
         "AccessLoggingEnabled": bool,
     },
     total=False,
 )
 
-_RequiredCorsRuleOutputTypeDef = TypedDict(
-    "_RequiredCorsRuleOutputTypeDef",
-    {
-        "AllowedOrigins": List[str],
-        "AllowedHeaders": List[str],
-    },
-)
-_OptionalCorsRuleOutputTypeDef = TypedDict(
-    "_OptionalCorsRuleOutputTypeDef",
-    {
-        "AllowedMethods": List[MethodNameType],
-        "MaxAgeSeconds": int,
-        "ExposeHeaders": List[str],
-    },
-    total=False,
-)
-
-class CorsRuleOutputTypeDef(_RequiredCorsRuleOutputTypeDef, _OptionalCorsRuleOutputTypeDef):
-    pass
-
 _RequiredCorsRuleTypeDef = TypedDict(
     "_RequiredCorsRuleTypeDef",
     {
-        "AllowedOrigins": Sequence[str],
-        "AllowedHeaders": Sequence[str],
+        "AllowedOrigins": List[str],
+        "AllowedHeaders": List[str],
     },
 )
 _OptionalCorsRuleTypeDef = TypedDict(
     "_OptionalCorsRuleTypeDef",
     {
-        "AllowedMethods": Sequence[MethodNameType],
+        "AllowedMethods": List[MethodNameType],
         "MaxAgeSeconds": int,
-        "ExposeHeaders": Sequence[str],
+        "ExposeHeaders": List[str],
     },
     total=False,
 )
 
 class CorsRuleTypeDef(_RequiredCorsRuleTypeDef, _OptionalCorsRuleTypeDef):
     pass
 
@@ -286,15 +262,22 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-CorsRuleUnionTypeDef = Union[CorsRuleTypeDef, CorsRuleOutputTypeDef]
+PutCorsPolicyInputRequestTypeDef = TypedDict(
+    "PutCorsPolicyInputRequestTypeDef",
+    {
+        "ContainerName": str,
+        "CorsPolicy": Sequence[CorsRuleTypeDef],
+    },
+)
+
 _RequiredCreateContainerInputRequestTypeDef = TypedDict(
     "_RequiredCreateContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 _OptionalCreateContainerInputRequestTypeDef = TypedDict(
@@ -341,15 +324,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCorsPolicyOutputTypeDef = TypedDict(
     "GetCorsPolicyOutputTypeDef",
     {
-        "CorsPolicy": List[CorsRuleOutputTypeDef],
+        "CorsPolicy": List[CorsRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyOutputTypeDef = TypedDict(
     "GetLifecyclePolicyOutputTypeDef",
     {
@@ -379,67 +362,39 @@
     "ListContainersInputListContainersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredMetricPolicyOutputTypeDef = TypedDict(
-    "_RequiredMetricPolicyOutputTypeDef",
-    {
-        "ContainerLevelMetrics": ContainerLevelMetricsType,
-    },
-)
-_OptionalMetricPolicyOutputTypeDef = TypedDict(
-    "_OptionalMetricPolicyOutputTypeDef",
-    {
-        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
-    },
-    total=False,
-)
-
-class MetricPolicyOutputTypeDef(
-    _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
-):
-    pass
-
 _RequiredMetricPolicyTypeDef = TypedDict(
     "_RequiredMetricPolicyTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyTypeDef = TypedDict(
     "_OptionalMetricPolicyTypeDef",
     {
-        "MetricPolicyRules": Sequence[MetricPolicyRuleTypeDef],
+        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
-PutCorsPolicyInputRequestTypeDef = TypedDict(
-    "PutCorsPolicyInputRequestTypeDef",
-    {
-        "ContainerName": str,
-        "CorsPolicy": Sequence[CorsRuleUnionTypeDef],
-    },
-)
-
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
-        "MetricPolicy": MetricPolicyOutputTypeDef,
+        "MetricPolicy": MetricPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MetricPolicyUnionTypeDef = Union[MetricPolicyTypeDef, MetricPolicyOutputTypeDef]
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "MetricPolicy": MetricPolicyTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/PKG-INFO` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
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
 [types-aiobotocore-mediastore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,83 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mediastore.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MediaStore` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/literals/).
+
 ```python
-from types_aiobotocore_mediastore.literals import (
-    ContainerLevelMetricsType,
-    ContainerStatusType,
-    ListContainersPaginatorName,
-    MethodNameType,
-    MediaStoreServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mediastore.literals import ContainerLevelMetricsType
 
 
 def check_value(value: ContainerLevelMetricsType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mediastore.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MediaStore` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/type_defs/).
+
 ```python
-from types_aiobotocore_mediastore.type_defs import (
-    ContainerTypeDef,
-    CorsRuleOutputTypeDef,
-    CorsRuleTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteContainerInputRequestTypeDef,
-    DeleteContainerPolicyInputRequestTypeDef,
-    DeleteCorsPolicyInputRequestTypeDef,
-    DeleteLifecyclePolicyInputRequestTypeDef,
-    DeleteMetricPolicyInputRequestTypeDef,
-    DescribeContainerInputRequestTypeDef,
-    GetContainerPolicyInputRequestTypeDef,
-    GetCorsPolicyInputRequestTypeDef,
-    GetLifecyclePolicyInputRequestTypeDef,
-    GetMetricPolicyInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListContainersInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    MetricPolicyRuleTypeDef,
-    PutContainerPolicyInputRequestTypeDef,
-    PutLifecyclePolicyInputRequestTypeDef,
-    StartAccessLoggingInputRequestTypeDef,
-    StopAccessLoggingInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CorsRuleUnionTypeDef,
-    CreateContainerInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    GetContainerPolicyOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
-    ListContainersOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
-    MetricPolicyOutputTypeDef,
-    MetricPolicyTypeDef,
-    PutCorsPolicyInputRequestTypeDef,
-    GetMetricPolicyOutputTypeDef,
-    MetricPolicyUnionTypeDef,
-    PutMetricPolicyInputRequestTypeDef,
-)
+from types_aiobotocore_mediastore.type_defs import ContainerTypeDef
 
 
 def get_value() -> ContainerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post1/types_aiobotocore_mediastore.egg-info/SOURCES.txt` & `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

