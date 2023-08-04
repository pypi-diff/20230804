# Comparing `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.933481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14297 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12711 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2183 2023-08-04 13:50:48.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1371 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1370 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1011 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12694 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12673 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9063 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9061 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6296 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6290 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8261 2023-08-04 13:50:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8256 2023-08-04 13:50:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14297 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1136 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       43 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/LICENSE` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,72 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resourcegroupstaggingapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroupsTaggingAPI` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/literals/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.literals import (
-    ErrorCodeType,
-    GetComplianceSummaryPaginatorName,
-    GetResourcesPaginatorName,
-    GetTagKeysPaginatorName,
-    GetTagValuesPaginatorName,
-    GroupByAttributeType,
-    TargetIdTypeType,
-    ResourceGroupsTaggingAPIServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resourcegroupstaggingapi.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ResourceGroupsTaggingAPI` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/type_defs/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
-    ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
-    GetComplianceSummaryInputRequestTypeDef,
-    SummaryTypeDef,
-    TagFilterTypeDef,
-    GetTagKeysInputRequestTypeDef,
-    GetTagValuesInputRequestTypeDef,
-    TagTypeDef,
-    StartReportCreationInputRequestTypeDef,
-    TagResourcesInputRequestTypeDef,
-    UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
-    TagResourcesOutputTypeDef,
-    UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
-    GetComplianceSummaryOutputTypeDef,
-    GetResourcesInputGetResourcesPaginateTypeDef,
-    GetResourcesInputRequestTypeDef,
-    ResourceTagMappingTypeDef,
-    GetResourcesOutputTypeDef,
-)
+from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef
 
 
 def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/README.md` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/README.md`

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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,72 +267,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resourcegroupstaggingapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroupsTaggingAPI` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/literals/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.literals import (
-    ErrorCodeType,
-    GetComplianceSummaryPaginatorName,
-    GetResourcesPaginatorName,
-    GetTagKeysPaginatorName,
-    GetTagValuesPaginatorName,
-    GroupByAttributeType,
-    TargetIdTypeType,
-    ResourceGroupsTaggingAPIServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resourcegroupstaggingapi.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ResourceGroupsTaggingAPI` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/type_defs/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
-    ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
-    GetComplianceSummaryInputRequestTypeDef,
-    SummaryTypeDef,
-    TagFilterTypeDef,
-    GetTagKeysInputRequestTypeDef,
-    GetTagValuesInputRequestTypeDef,
-    TagTypeDef,
-    StartReportCreationInputRequestTypeDef,
-    TagResourcesInputRequestTypeDef,
-    UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
-    TagResourcesOutputTypeDef,
-    UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
-    GetComplianceSummaryOutputTypeDef,
-    GetResourcesInputGetResourcesPaginateTypeDef,
-    GetResourcesInputRequestTypeDef,
-    ResourceTagMappingTypeDef,
-    GetResourcesOutputTypeDef,
-)
+from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef
 
 
 def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resourcegroupstaggingapi",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__main__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -157,14 +158,15 @@
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
@@ -243,26 +245,28 @@
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
@@ -424,14 +428,15 @@
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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
@@ -422,14 +426,15 @@
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,72 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_resourcegroupstaggingapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ResourceGroupsTaggingAPI` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/literals/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.literals import (
-    ErrorCodeType,
-    GetComplianceSummaryPaginatorName,
-    GetResourcesPaginatorName,
-    GetTagKeysPaginatorName,
-    GetTagValuesPaginatorName,
-    GroupByAttributeType,
-    TargetIdTypeType,
-    ResourceGroupsTaggingAPIServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_resourcegroupstaggingapi.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ResourceGroupsTaggingAPI` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/type_defs/).
+
 ```python
-from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
-    ComplianceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    FailureInfoTypeDef,
-    PaginatorConfigTypeDef,
-    GetComplianceSummaryInputRequestTypeDef,
-    SummaryTypeDef,
-    TagFilterTypeDef,
-    GetTagKeysInputRequestTypeDef,
-    GetTagValuesInputRequestTypeDef,
-    TagTypeDef,
-    StartReportCreationInputRequestTypeDef,
-    TagResourcesInputRequestTypeDef,
-    UntagResourcesInputRequestTypeDef,
-    DescribeReportCreationOutputTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesOutputTypeDef,
-    TagResourcesOutputTypeDef,
-    UntagResourcesOutputTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
-    GetComplianceSummaryOutputTypeDef,
-    GetResourcesInputGetResourcesPaginateTypeDef,
-    GetResourcesInputRequestTypeDef,
-    ResourceTagMappingTypeDef,
-    GetResourcesOutputTypeDef,
-)
+from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef
 
 
 def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

