# Comparing `tmp/types-aiobotocore-connectcases-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-connectcases-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
```

## Comparing `types-aiobotocore-connectcases-2.5.2.post1.tar` & `types-aiobotocore-connectcases-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:53.000000 types-aiobotocore-connectcases-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23909 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32011 2023-08-02 14:35:55.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-08-04 11:43:14.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:13.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:41.991745 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:41.000000 types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/LICENSE` & `types-aiobotocore-connectcases-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,150 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_connectcases.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ConnectCases` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/literals/).
+
 ```python
-from types_aiobotocore_connectcases.literals import (
-    CommentBodyTextTypeType,
-    DomainStatusType,
-    FieldNamespaceType,
-    FieldTypeType,
-    OrderType,
-    RelatedItemTypeType,
-    SearchCasesPaginatorName,
-    SearchRelatedItemsPaginatorName,
-    TemplateStatusType,
-    ConnectCasesServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_connectcases.literals import CommentBodyTextTypeType
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_connectcases.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ConnectCases` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/type_defs/).
+
 ```python
-from types_aiobotocore_connectcases.type_defs import (
-    FieldIdentifierTypeDef,
-    FieldErrorTypeDef,
-    GetFieldResponseTypeDef,
-    ResponseMetadataTypeDef,
-    FieldOptionTypeDef,
-    FieldOptionErrorTypeDef,
-    CaseSummaryTypeDef,
-    CommentContentTypeDef,
-    ContactContentTypeDef,
-    ContactFilterTypeDef,
-    ContactTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateFieldRequestRequestTypeDef,
-    LayoutConfigurationTypeDef,
-    RequiredFieldTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DomainSummaryTypeDef,
-    RelatedItemEventIncludedDataTypeDef,
-    FieldItemTypeDef,
-    FieldSummaryTypeDef,
-    FieldValueUnionTypeDef,
-    GetCaseEventConfigurationRequestRequestTypeDef,
-    GetDomainRequestRequestTypeDef,
-    GetLayoutRequestRequestTypeDef,
-    GetTemplateRequestRequestTypeDef,
-    LayoutSummaryTypeDef,
-    ListCasesForContactRequestRequestTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListFieldOptionsRequestRequestTypeDef,
-    ListFieldsRequestRequestTypeDef,
-    ListLayoutsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTemplatesRequestRequestTypeDef,
-    TemplateSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    SortTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateFieldRequestRequestTypeDef,
-    BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
-    CaseEventIncludedDataTypeDef,
-    GetCaseRequestRequestTypeDef,
-    BatchGetFieldResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
-    CreateTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDomainResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
-    BatchPutFieldOptionsResponseTypeDef,
-    ListCasesForContactResponseTypeDef,
-    RelatedItemContentTypeDef,
-    RelatedItemTypeFilterTypeDef,
-    RelatedItemInputContentTypeDef,
-    CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
-    UpdateTemplateRequestRequestTypeDef,
-    ListDomainsResponseTypeDef,
-    FieldGroupOutputTypeDef,
-    FieldGroupTypeDef,
-    ListFieldsResponseTypeDef,
-    FieldValueTypeDef,
-    ListLayoutsResponseTypeDef,
-    ListTemplatesResponseTypeDef,
-    SearchCasesRequestRequestTypeDef,
-    SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
-    EventIncludedDataTypeDef,
-    SearchRelatedItemsResponseItemTypeDef,
-    SearchRelatedItemsRequestRequestTypeDef,
-    SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
-    CreateRelatedItemRequestRequestTypeDef,
-    SectionOutputTypeDef,
-    SectionTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    FieldFilterTypeDef,
-    GetCaseResponseTypeDef,
-    SearchCasesResponseItemTypeDef,
-    UpdateCaseRequestRequestTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
-    EventBridgeConfigurationTypeDef,
-    SearchRelatedItemsResponseTypeDef,
-    LayoutSectionsOutputTypeDef,
-    LayoutSectionsTypeDef,
-    CaseFilterTypeDef,
-    SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
-    PutCaseEventConfigurationRequestRequestTypeDef,
-    BasicLayoutOutputTypeDef,
-    BasicLayoutTypeDef,
-    LayoutContentOutputTypeDef,
-    LayoutContentTypeDef,
-    GetLayoutResponseTypeDef,
-    CreateLayoutRequestRequestTypeDef,
-    LayoutContentUnionTypeDef,
-    UpdateLayoutRequestRequestTypeDef,
-)
+from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
 
 def get_value() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/setup.py` & `types-aiobotocore-connectcases-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcases",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.pyi` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__main__.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentUnionTypeDef,
+    LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -172,15 +172,15 @@
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_field)
         """
 
     async def create_layout(
-        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_layout)
         """
@@ -365,15 +365,15 @@
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
 
     async def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#put_case_event_configuration)
@@ -450,20 +450,15 @@
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_field)
         """
 
     async def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: LayoutContentUnionTypeDef = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_layout)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.pyi` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentUnionTypeDef,
+    LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -160,15 +160,15 @@
         """
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_field)
         """
     async def create_layout(
-        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_layout)
         """
@@ -336,15 +336,15 @@
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
     async def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#put_case_event_configuration)
@@ -414,20 +414,15 @@
         """
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_field)
         """
     async def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: LayoutContentUnionTypeDef = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_layout)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.pyi` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.pyi` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.py` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
     data: FieldIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -71,15 +71,14 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
@@ -95,52 +94,43 @@
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
-    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
-    "SectionOutputTypeDef",
     "SectionTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "UpdateCaseRequestRequestTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
-    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
-    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
-    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
-    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
-    "LayoutContentUnionTypeDef",
+    "GetLayoutResponseTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
@@ -598,25 +588,18 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": Sequence[FieldIdentifierTypeDef],
+        "fields": List[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -864,33 +847,14 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -989,23 +953,14 @@
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
-    {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
-    },
-    total=False,
-)
-
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
@@ -1090,22 +1045,14 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
-SectionOutputTypeDef = TypedDict(
-    "SectionOutputTypeDef",
-    {
-        "fieldGroup": FieldGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
@@ -1185,35 +1132,14 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
 )
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
-        "includedData": EventIncludedDataOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1236,22 +1162,14 @@
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LayoutSectionsOutputTypeDef = TypedDict(
-    "LayoutSectionsOutputTypeDef",
-    {
-        "sections": List[SectionOutputTypeDef],
-    },
-    total=False,
-)
-
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
@@ -1274,86 +1192,65 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "eventBridge": EventBridgeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventBridgeConfigurationUnionTypeDef = Union[
-    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
-]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
-BasicLayoutOutputTypeDef = TypedDict(
-    "BasicLayoutOutputTypeDef",
-    {
-        "moreInfo": LayoutSectionsOutputTypeDef,
-        "topPanel": LayoutSectionsOutputTypeDef,
-    },
-    total=False,
-)
-
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
-LayoutContentOutputTypeDef = TypedDict(
-    "LayoutContentOutputTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "basic": BasicLayoutOutputTypeDef,
+        "basic": BasicLayoutTypeDef,
     },
     total=False,
 )
 
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
     {
-        "basic": BasicLayoutTypeDef,
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
     },
-    total=False,
 )
 
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentOutputTypeDef,
+        "content": LayoutContentTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
-    {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
-    },
-)
-
-LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.pyi` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
     data: FieldIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -70,15 +70,14 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
@@ -94,52 +93,43 @@
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
-    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
-    "SectionOutputTypeDef",
     "SectionTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "UpdateCaseRequestRequestTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
-    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
-    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
-    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
-    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
-    "LayoutContentUnionTypeDef",
+    "GetLayoutResponseTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
@@ -579,25 +569,18 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": Sequence[FieldIdentifierTypeDef],
+        "fields": List[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -839,31 +822,14 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
-    {
-        "name": str,
-    },
-    total=False,
-)
-
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -956,23 +922,14 @@
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
-    {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
-    },
-    total=False,
-)
-
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
@@ -1051,22 +1008,14 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
-SectionOutputTypeDef = TypedDict(
-    "SectionOutputTypeDef",
-    {
-        "fieldGroup": FieldGroupOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
@@ -1142,33 +1091,14 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
 )
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
-    {
-        "includedData": EventIncludedDataOutputTypeDef,
-    },
-    total=False,
-)
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1189,22 +1119,14 @@
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LayoutSectionsOutputTypeDef = TypedDict(
-    "LayoutSectionsOutputTypeDef",
-    {
-        "sections": List[SectionOutputTypeDef],
-    },
-    total=False,
-)
-
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
@@ -1227,86 +1149,65 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "eventBridge": EventBridgeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventBridgeConfigurationUnionTypeDef = Union[
-    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
-]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
-BasicLayoutOutputTypeDef = TypedDict(
-    "BasicLayoutOutputTypeDef",
-    {
-        "moreInfo": LayoutSectionsOutputTypeDef,
-        "topPanel": LayoutSectionsOutputTypeDef,
-    },
-    total=False,
-)
-
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
-LayoutContentOutputTypeDef = TypedDict(
-    "LayoutContentOutputTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "basic": BasicLayoutOutputTypeDef,
+        "basic": BasicLayoutTypeDef,
     },
     total=False,
 )
 
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
     {
-        "basic": BasicLayoutTypeDef,
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
     },
-    total=False,
 )
 
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentOutputTypeDef,
+        "content": LayoutContentTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
-    {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
-    },
-)
-
-LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,150 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_connectcases.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ConnectCases` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/literals/).
+
 ```python
-from types_aiobotocore_connectcases.literals import (
-    CommentBodyTextTypeType,
-    DomainStatusType,
-    FieldNamespaceType,
-    FieldTypeType,
-    OrderType,
-    RelatedItemTypeType,
-    SearchCasesPaginatorName,
-    SearchRelatedItemsPaginatorName,
-    TemplateStatusType,
-    ConnectCasesServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_connectcases.literals import CommentBodyTextTypeType
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_connectcases.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ConnectCases` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/type_defs/).
+
 ```python
-from types_aiobotocore_connectcases.type_defs import (
-    FieldIdentifierTypeDef,
-    FieldErrorTypeDef,
-    GetFieldResponseTypeDef,
-    ResponseMetadataTypeDef,
-    FieldOptionTypeDef,
-    FieldOptionErrorTypeDef,
-    CaseSummaryTypeDef,
-    CommentContentTypeDef,
-    ContactContentTypeDef,
-    ContactFilterTypeDef,
-    ContactTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateFieldRequestRequestTypeDef,
-    LayoutConfigurationTypeDef,
-    RequiredFieldTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DomainSummaryTypeDef,
-    RelatedItemEventIncludedDataTypeDef,
-    FieldItemTypeDef,
-    FieldSummaryTypeDef,
-    FieldValueUnionTypeDef,
-    GetCaseEventConfigurationRequestRequestTypeDef,
-    GetDomainRequestRequestTypeDef,
-    GetLayoutRequestRequestTypeDef,
-    GetTemplateRequestRequestTypeDef,
-    LayoutSummaryTypeDef,
-    ListCasesForContactRequestRequestTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListFieldOptionsRequestRequestTypeDef,
-    ListFieldsRequestRequestTypeDef,
-    ListLayoutsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTemplatesRequestRequestTypeDef,
-    TemplateSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    SortTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateFieldRequestRequestTypeDef,
-    BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
-    CaseEventIncludedDataTypeDef,
-    GetCaseRequestRequestTypeDef,
-    BatchGetFieldResponseTypeDef,
-    CreateCaseResponseTypeDef,
-    CreateDomainResponseTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
-    CreateTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDomainResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
-    BatchPutFieldOptionsResponseTypeDef,
-    ListCasesForContactResponseTypeDef,
-    RelatedItemContentTypeDef,
-    RelatedItemTypeFilterTypeDef,
-    RelatedItemInputContentTypeDef,
-    CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
-    UpdateTemplateRequestRequestTypeDef,
-    ListDomainsResponseTypeDef,
-    FieldGroupOutputTypeDef,
-    FieldGroupTypeDef,
-    ListFieldsResponseTypeDef,
-    FieldValueTypeDef,
-    ListLayoutsResponseTypeDef,
-    ListTemplatesResponseTypeDef,
-    SearchCasesRequestRequestTypeDef,
-    SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
-    EventIncludedDataTypeDef,
-    SearchRelatedItemsResponseItemTypeDef,
-    SearchRelatedItemsRequestRequestTypeDef,
-    SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
-    CreateRelatedItemRequestRequestTypeDef,
-    SectionOutputTypeDef,
-    SectionTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    FieldFilterTypeDef,
-    GetCaseResponseTypeDef,
-    SearchCasesResponseItemTypeDef,
-    UpdateCaseRequestRequestTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
-    EventBridgeConfigurationTypeDef,
-    SearchRelatedItemsResponseTypeDef,
-    LayoutSectionsOutputTypeDef,
-    LayoutSectionsTypeDef,
-    CaseFilterTypeDef,
-    SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
-    PutCaseEventConfigurationRequestRequestTypeDef,
-    BasicLayoutOutputTypeDef,
-    BasicLayoutTypeDef,
-    LayoutContentOutputTypeDef,
-    LayoutContentTypeDef,
-    GetLayoutResponseTypeDef,
-    CreateLayoutRequestRequestTypeDef,
-    LayoutContentUnionTypeDef,
-    UpdateLayoutRequestRequestTypeDef,
-)
+from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
 
 def get_value() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/SOURCES.txt` & `types-aiobotocore-connectcases-2.5.2.post2/types_aiobotocore_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

