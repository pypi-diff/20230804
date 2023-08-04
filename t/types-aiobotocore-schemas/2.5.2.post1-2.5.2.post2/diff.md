# Comparing `tmp/types-aiobotocore-schemas-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-schemas-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-schemas-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-schemas-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-schemas-2.5.2.post1.tar` & `types-aiobotocore-schemas-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.769464 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25217 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26095 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14181 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12663 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1647 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1646 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25263 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25217 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9045 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9043 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6566 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6559 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26134 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26095 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1674 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1673 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14181 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-schemas-2.5.2.post1/LICENSE` & `types-aiobotocore-schemas-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/README.md` & `types-aiobotocore-schemas-2.5.2.post2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-schemas
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore schemas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,119 +323,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_schemas.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Schemas` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/literals/).
+
 ```python
-from types_aiobotocore_schemas.literals import (
-    CodeBindingExistsWaiterName,
-    CodeGenerationStatusType,
-    DiscovererStateType,
-    ListDiscoverersPaginatorName,
-    ListRegistriesPaginatorName,
-    ListSchemaVersionsPaginatorName,
-    ListSchemasPaginatorName,
-    SearchSchemasPaginatorName,
-    TypeType,
-    SchemasServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_schemas.literals import CodeBindingExistsWaiterName
 
 
 def check_value(value: CodeBindingExistsWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_schemas.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Schemas` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/type_defs/).
+
 ```python
-from types_aiobotocore_schemas.type_defs import (
-    CreateDiscovererRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateRegistryRequestRequestTypeDef,
-    CreateSchemaRequestRequestTypeDef,
-    DeleteDiscovererRequestRequestTypeDef,
-    DeleteRegistryRequestRequestTypeDef,
-    DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaVersionRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCodeBindingRequestRequestTypeDef,
-    DescribeDiscovererRequestRequestTypeDef,
-    DescribeRegistryRequestRequestTypeDef,
-    DescribeSchemaRequestRequestTypeDef,
-    DiscovererSummaryTypeDef,
-    ExportSchemaRequestRequestTypeDef,
-    GetCodeBindingSourceRequestRequestTypeDef,
-    GetDiscoveredSchemaRequestRequestTypeDef,
-    GetResourcePolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestRequestTypeDef,
-    RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestRequestTypeDef,
-    SchemaVersionSummaryTypeDef,
-    ListSchemasRequestRequestTypeDef,
-    SchemaSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutCodeBindingRequestRequestTypeDef,
-    PutResourcePolicyRequestRequestTypeDef,
-    SearchSchemaVersionSummaryTypeDef,
-    SearchSchemasRequestRequestTypeDef,
-    StartDiscovererRequestRequestTypeDef,
-    StopDiscovererRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDiscovererRequestRequestTypeDef,
-    UpdateRegistryRequestRequestTypeDef,
-    UpdateSchemaRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DescribeCodeBindingResponseTypeDef,
-    DescribeDiscovererResponseTypeDef,
-    DescribeRegistryResponseTypeDef,
-    DescribeSchemaResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportSchemaResponseTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutCodeBindingResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartDiscovererResponseTypeDef,
-    StopDiscovererResponseTypeDef,
-    UpdateDiscovererResponseTypeDef,
-    UpdateRegistryResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
-    ListDiscoverersResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
-    ListRegistriesResponseTypeDef,
-    ListSchemaVersionsResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    SearchSchemaSummaryTypeDef,
-    SearchSchemasResponseTypeDef,
-)
+from types_aiobotocore_schemas.type_defs import CreateDiscovererRequestRequestTypeDef
 
 
 def get_value() -> CreateDiscovererRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-schemas-2.5.2.post1/setup.py` & `types-aiobotocore-schemas-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-schemas",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__main__.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Schemas 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Schemas 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -162,14 +163,15 @@
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
@@ -248,26 +250,28 @@
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

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -160,14 +161,15 @@
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
@@ -246,26 +248,28 @@
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

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.py` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.pyi` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/SOURCES.txt` & `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

