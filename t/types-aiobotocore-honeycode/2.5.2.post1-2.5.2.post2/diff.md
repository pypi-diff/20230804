# Comparing `tmp/types-aiobotocore-honeycode-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-honeycode-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-honeycode-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-honeycode-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:48 2023, max compression
```

## Comparing `types-aiobotocore-honeycode-2.5.2.post1.tar` & `types-aiobotocore-honeycode-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.013573 types-aiobotocore-honeycode-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:23.013573 types-aiobotocore-honeycode-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-08-02 14:39:57.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21410 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.751929 types-aiobotocore-honeycode-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:48.751929 types-aiobotocore-honeycode-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-08-04 12:24:57.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/LICENSE` & `types-aiobotocore-honeycode-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/PKG-INFO` & `types-aiobotocore-honeycode-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,109 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_honeycode.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Honeycode` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/literals/).
+
 ```python
-from types_aiobotocore_honeycode.literals import (
-    ErrorCodeType,
-    FormatType,
-    ImportDataCharacterEncodingType,
-    ImportSourceDataFormatType,
-    ListTableColumnsPaginatorName,
-    ListTableRowsPaginatorName,
-    ListTablesPaginatorName,
-    QueryTableRowsPaginatorName,
-    TableDataImportJobStatusType,
-    UpsertActionType,
-    HoneycodeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_honeycode.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Honeycode` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/type_defs/).
+
 ```python
-from types_aiobotocore_honeycode.type_defs import (
-    FailedBatchItemTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteTableRowsRequestRequestTypeDef,
-    UpsertRowsResultTypeDef,
-    CellInputTypeDef,
-    CellTypeDef,
-    ColumnMetadataTypeDef,
-    DataItemTypeDef,
-    DelimitedTextImportOptionsTypeDef,
-    DescribeTableDataImportJobRequestRequestTypeDef,
-    SourceDataColumnPropertiesTypeDef,
-    FilterTypeDef,
-    VariableValueTypeDef,
-    ImportDataSourceConfigTypeDef,
-    ImportJobSubmitterTypeDef,
-    PaginatorConfigTypeDef,
-    ListTableColumnsRequestRequestTypeDef,
-    TableColumnTypeDef,
-    ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    TableTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchCreateTableRowsResultTypeDef,
-    BatchDeleteTableRowsResultTypeDef,
-    BatchUpdateTableRowsResultTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartTableDataImportJobResultTypeDef,
-    BatchUpsertTableRowsResultTypeDef,
-    CreateRowDataTypeDef,
-    UpdateRowDataTypeDef,
-    TableRowTypeDef,
-    ResultRowTypeDef,
-    DestinationOptionsOutputTypeDef,
-    DestinationOptionsTypeDef,
-    QueryTableRowsRequestRequestTypeDef,
-    UpsertRowDataTypeDef,
-    GetScreenDataRequestRequestTypeDef,
-    InvokeScreenAutomationRequestRequestTypeDef,
-    ImportDataSourceTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    ListTableColumnsResultTypeDef,
-    ListTablesResultTypeDef,
-    BatchCreateTableRowsRequestRequestTypeDef,
-    BatchUpdateTableRowsRequestRequestTypeDef,
-    ListTableRowsResultTypeDef,
-    QueryTableRowsResultTypeDef,
-    ResultSetTypeDef,
-    ImportOptionsOutputTypeDef,
-    ImportOptionsTypeDef,
-    BatchUpsertTableRowsRequestRequestTypeDef,
-    GetScreenDataResultTypeDef,
-    TableDataImportJobMetadataTypeDef,
-    ImportOptionsUnionTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
-    DescribeTableDataImportJobResultTypeDef,
-)
+from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
 
 def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/README.md` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-honeycode
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore honeycode type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,109 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_honeycode.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Honeycode` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/literals/).
+
 ```python
-from types_aiobotocore_honeycode.literals import (
-    ErrorCodeType,
-    FormatType,
-    ImportDataCharacterEncodingType,
-    ImportSourceDataFormatType,
-    ListTableColumnsPaginatorName,
-    ListTableRowsPaginatorName,
-    ListTablesPaginatorName,
-    QueryTableRowsPaginatorName,
-    TableDataImportJobStatusType,
-    UpsertActionType,
-    HoneycodeServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_honeycode.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Honeycode` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/type_defs/).
+
 ```python
-from types_aiobotocore_honeycode.type_defs import (
-    FailedBatchItemTypeDef,
-    ResponseMetadataTypeDef,
-    BatchDeleteTableRowsRequestRequestTypeDef,
-    UpsertRowsResultTypeDef,
-    CellInputTypeDef,
-    CellTypeDef,
-    ColumnMetadataTypeDef,
-    DataItemTypeDef,
-    DelimitedTextImportOptionsTypeDef,
-    DescribeTableDataImportJobRequestRequestTypeDef,
-    SourceDataColumnPropertiesTypeDef,
-    FilterTypeDef,
-    VariableValueTypeDef,
-    ImportDataSourceConfigTypeDef,
-    ImportJobSubmitterTypeDef,
-    PaginatorConfigTypeDef,
-    ListTableColumnsRequestRequestTypeDef,
-    TableColumnTypeDef,
-    ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    TableTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchCreateTableRowsResultTypeDef,
-    BatchDeleteTableRowsResultTypeDef,
-    BatchUpdateTableRowsResultTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    StartTableDataImportJobResultTypeDef,
-    BatchUpsertTableRowsResultTypeDef,
-    CreateRowDataTypeDef,
-    UpdateRowDataTypeDef,
-    TableRowTypeDef,
-    ResultRowTypeDef,
-    DestinationOptionsOutputTypeDef,
-    DestinationOptionsTypeDef,
-    QueryTableRowsRequestRequestTypeDef,
-    UpsertRowDataTypeDef,
-    GetScreenDataRequestRequestTypeDef,
-    InvokeScreenAutomationRequestRequestTypeDef,
-    ImportDataSourceTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    ListTableColumnsResultTypeDef,
-    ListTablesResultTypeDef,
-    BatchCreateTableRowsRequestRequestTypeDef,
-    BatchUpdateTableRowsRequestRequestTypeDef,
-    ListTableRowsResultTypeDef,
-    QueryTableRowsResultTypeDef,
-    ResultSetTypeDef,
-    ImportOptionsOutputTypeDef,
-    ImportOptionsTypeDef,
-    BatchUpsertTableRowsRequestRequestTypeDef,
-    GetScreenDataResultTypeDef,
-    TableDataImportJobMetadataTypeDef,
-    ImportOptionsUnionTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
-    DescribeTableDataImportJobResultTypeDef,
-)
+from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
 
 def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/setup.py` & `types-aiobotocore-honeycode-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-honeycode",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.pyi` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__main__.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Honeycode 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Honeycode 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsUnionTypeDef,
+    ImportOptionsTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -299,15 +299,15 @@
     async def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsUnionTypeDef,
+        importOptions: ImportOptionsTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.pyi` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsUnionTypeDef,
+    ImportOptionsTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -279,15 +279,15 @@
     async def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsUnionTypeDef,
+        importOptions: ImportOptionsTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.pyi` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.pyi` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.py` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
     data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -28,15 +28,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FailedBatchItemTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
@@ -65,15 +64,14 @@
     "ListTagsForResourceResultTypeDef",
     "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
-    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
     "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
@@ -83,21 +81,19 @@
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
-    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "TableDataImportJobMetadataTypeDef",
-    "ImportOptionsUnionTypeDef",
     "StartTableDataImportJobRequestRequestTypeDef",
+    "TableDataImportJobMetadataTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
@@ -128,22 +124,20 @@
     "_OptionalBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableRowsRequestRequestTypeDef(
     _RequiredBatchDeleteTableRowsRequestRequestTypeDef,
     _OptionalBatchDeleteTableRowsRequestRequestTypeDef,
 ):
     pass
 
-
 UpsertRowsResultTypeDef = TypedDict(
     "UpsertRowsResultTypeDef",
     {
         "rowIds": List[str],
         "upsertAction": UpsertActionType,
     },
 )
@@ -199,21 +193,19 @@
         "hasHeaderRow": bool,
         "ignoreEmptyRows": bool,
         "dataCharacterEncoding": ImportDataCharacterEncodingType,
     },
     total=False,
 )
 
-
 class DelimitedTextImportOptionsTypeDef(
     _RequiredDelimitedTextImportOptionsTypeDef, _OptionalDelimitedTextImportOptionsTypeDef
 ):
     pass
 
-
 DescribeTableDataImportJobRequestRequestTypeDef = TypedDict(
     "DescribeTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
@@ -237,19 +229,17 @@
     "_OptionalFilterTypeDef",
     {
         "contextRowId": str,
     },
     total=False,
 )
 
-
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
-
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
@@ -291,21 +281,19 @@
     "_OptionalListTableColumnsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTableColumnsRequestRequestTypeDef(
     _RequiredListTableColumnsRequestRequestTypeDef, _OptionalListTableColumnsRequestRequestTypeDef
 ):
     pass
 
-
 TableColumnTypeDef = TypedDict(
     "TableColumnTypeDef",
     {
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
@@ -325,21 +313,19 @@
         "rowIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -347,21 +333,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTablesRequestRequestTypeDef(
     _RequiredListTablesRequestRequestTypeDef, _OptionalListTablesRequestRequestTypeDef
 ):
     pass
 
-
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "tableId": str,
         "tableName": str,
     },
     total=False,
@@ -487,31 +471,21 @@
     "_OptionalResultRowTypeDef",
     {
         "rowId": str,
     },
     total=False,
 )
 
-
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
-
-DestinationOptionsOutputTypeDef = TypedDict(
-    "DestinationOptionsOutputTypeDef",
-    {
-        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
-    },
-    total=False,
-)
-
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
-        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
+        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
@@ -525,21 +499,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class QueryTableRowsRequestRequestTypeDef(
     _RequiredQueryTableRowsRequestRequestTypeDef, _OptionalQueryTableRowsRequestRequestTypeDef
 ):
     pass
 
-
 UpsertRowDataTypeDef = TypedDict(
     "UpsertRowDataTypeDef",
     {
         "batchItemId": str,
         "filter": FilterTypeDef,
         "cellsToUpdate": Mapping[str, CellInputTypeDef],
     },
@@ -559,21 +531,19 @@
         "variables": Mapping[str, VariableValueTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class GetScreenDataRequestRequestTypeDef(
     _RequiredGetScreenDataRequestRequestTypeDef, _OptionalGetScreenDataRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInvokeScreenAutomationRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeScreenAutomationRequestRequestTypeDef",
     {
         "workbookId": str,
         "appId": str,
         "screenId": str,
         "screenAutomationId": str,
@@ -585,22 +555,20 @@
         "variables": Mapping[str, VariableValueTypeDef],
         "rowId": str,
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
-
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
@@ -615,22 +583,20 @@
     "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
     _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
     _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
     "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -639,44 +605,40 @@
     {
         "rowIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTableRowsRequestListTableRowsPaginateTypeDef(
     _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
     _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
     "_RequiredListTablesRequestListTablesPaginateTypeDef",
     {
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
     "_OptionalListTablesRequestListTablesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTablesRequestListTablesPaginateTypeDef(
     _RequiredListTablesRequestListTablesPaginateTypeDef,
     _OptionalListTablesRequestListTablesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -685,22 +647,20 @@
     "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
     _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
 ):
     pass
 
-
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -729,22 +689,20 @@
     "_OptionalBatchCreateTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class BatchCreateTableRowsRequestRequestTypeDef(
     _RequiredBatchCreateTableRowsRequestRequestTypeDef,
     _OptionalBatchCreateTableRowsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchUpdateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowsToUpdate": Sequence[UpdateRowDataTypeDef],
     },
@@ -753,22 +711,20 @@
     "_OptionalBatchUpdateTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class BatchUpdateTableRowsRequestRequestTypeDef(
     _RequiredBatchUpdateTableRowsRequestRequestTypeDef,
     _OptionalBatchUpdateTableRowsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTableRowsResultTypeDef = TypedDict(
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
@@ -792,23 +748,14 @@
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
-ImportOptionsOutputTypeDef = TypedDict(
-    "ImportOptionsOutputTypeDef",
-    {
-        "destinationOptions": DestinationOptionsOutputTypeDef,
-        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
-    },
-    total=False,
-)
-
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -826,55 +773,52 @@
     "_OptionalBatchUpsertTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class BatchUpsertTableRowsRequestRequestTypeDef(
     _RequiredBatchUpsertTableRowsRequestRequestTypeDef,
     _OptionalBatchUpsertTableRowsRequestRequestTypeDef,
 ):
     pass
 
-
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsOutputTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
-ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
+    },
+)
+
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.pyi` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
     data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -28,14 +28,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FailedBatchItemTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
@@ -64,15 +65,14 @@
     "ListTagsForResourceResultTypeDef",
     "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
-    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
     "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
@@ -82,21 +82,19 @@
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
-    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "TableDataImportJobMetadataTypeDef",
-    "ImportOptionsUnionTypeDef",
     "StartTableDataImportJobRequestRequestTypeDef",
+    "TableDataImportJobMetadataTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
@@ -127,20 +125,22 @@
     "_OptionalBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableRowsRequestRequestTypeDef(
     _RequiredBatchDeleteTableRowsRequestRequestTypeDef,
     _OptionalBatchDeleteTableRowsRequestRequestTypeDef,
 ):
     pass
 
+
 UpsertRowsResultTypeDef = TypedDict(
     "UpsertRowsResultTypeDef",
     {
         "rowIds": List[str],
         "upsertAction": UpsertActionType,
     },
 )
@@ -196,19 +196,21 @@
         "hasHeaderRow": bool,
         "ignoreEmptyRows": bool,
         "dataCharacterEncoding": ImportDataCharacterEncodingType,
     },
     total=False,
 )
 
+
 class DelimitedTextImportOptionsTypeDef(
     _RequiredDelimitedTextImportOptionsTypeDef, _OptionalDelimitedTextImportOptionsTypeDef
 ):
     pass
 
+
 DescribeTableDataImportJobRequestRequestTypeDef = TypedDict(
     "DescribeTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
@@ -232,17 +234,19 @@
     "_OptionalFilterTypeDef",
     {
         "contextRowId": str,
     },
     total=False,
 )
 
+
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
+
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
@@ -284,19 +288,21 @@
     "_OptionalListTableColumnsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTableColumnsRequestRequestTypeDef(
     _RequiredListTableColumnsRequestRequestTypeDef, _OptionalListTableColumnsRequestRequestTypeDef
 ):
     pass
 
+
 TableColumnTypeDef = TypedDict(
     "TableColumnTypeDef",
     {
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
@@ -316,19 +322,21 @@
         "rowIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -336,19 +344,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTablesRequestRequestTypeDef(
     _RequiredListTablesRequestRequestTypeDef, _OptionalListTablesRequestRequestTypeDef
 ):
     pass
 
+
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "tableId": str,
         "tableName": str,
     },
     total=False,
@@ -474,29 +484,23 @@
     "_OptionalResultRowTypeDef",
     {
         "rowId": str,
     },
     total=False,
 )
 
+
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
-DestinationOptionsOutputTypeDef = TypedDict(
-    "DestinationOptionsOutputTypeDef",
-    {
-        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
-    },
-    total=False,
-)
 
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
-        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
+        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
@@ -510,19 +514,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class QueryTableRowsRequestRequestTypeDef(
     _RequiredQueryTableRowsRequestRequestTypeDef, _OptionalQueryTableRowsRequestRequestTypeDef
 ):
     pass
 
+
 UpsertRowDataTypeDef = TypedDict(
     "UpsertRowDataTypeDef",
     {
         "batchItemId": str,
         "filter": FilterTypeDef,
         "cellsToUpdate": Mapping[str, CellInputTypeDef],
     },
@@ -542,19 +548,21 @@
         "variables": Mapping[str, VariableValueTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class GetScreenDataRequestRequestTypeDef(
     _RequiredGetScreenDataRequestRequestTypeDef, _OptionalGetScreenDataRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInvokeScreenAutomationRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeScreenAutomationRequestRequestTypeDef",
     {
         "workbookId": str,
         "appId": str,
         "screenId": str,
         "screenAutomationId": str,
@@ -566,20 +574,22 @@
         "variables": Mapping[str, VariableValueTypeDef],
         "rowId": str,
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
+
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
@@ -594,20 +604,22 @@
     "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
     _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
     _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
     "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -616,40 +628,44 @@
     {
         "rowIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTableRowsRequestListTableRowsPaginateTypeDef(
     _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
     _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
     "_RequiredListTablesRequestListTablesPaginateTypeDef",
     {
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
     "_OptionalListTablesRequestListTablesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTablesRequestListTablesPaginateTypeDef(
     _RequiredListTablesRequestListTablesPaginateTypeDef,
     _OptionalListTablesRequestListTablesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -658,20 +674,22 @@
     "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
     _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
 ):
     pass
 
+
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -700,20 +718,22 @@
     "_OptionalBatchCreateTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class BatchCreateTableRowsRequestRequestTypeDef(
     _RequiredBatchCreateTableRowsRequestRequestTypeDef,
     _OptionalBatchCreateTableRowsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchUpdateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowsToUpdate": Sequence[UpdateRowDataTypeDef],
     },
@@ -722,20 +742,22 @@
     "_OptionalBatchUpdateTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class BatchUpdateTableRowsRequestRequestTypeDef(
     _RequiredBatchUpdateTableRowsRequestRequestTypeDef,
     _OptionalBatchUpdateTableRowsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTableRowsResultTypeDef = TypedDict(
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
@@ -759,23 +781,14 @@
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
-ImportOptionsOutputTypeDef = TypedDict(
-    "ImportOptionsOutputTypeDef",
-    {
-        "destinationOptions": DestinationOptionsOutputTypeDef,
-        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
-    },
-    total=False,
-)
-
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -793,53 +806,54 @@
     "_OptionalBatchUpsertTableRowsRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class BatchUpsertTableRowsRequestRequestTypeDef(
     _RequiredBatchUpsertTableRowsRequestRequestTypeDef,
     _OptionalBatchUpsertTableRowsRequestRequestTypeDef,
 ):
     pass
 
+
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsOutputTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
-ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
+    },
+)
+
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/SOURCES.txt` & `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

