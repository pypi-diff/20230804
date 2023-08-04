# Comparing `tmp/types-aiobotocore-redshift-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-redshift-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-redshift-data-2.5.2.post1.tar` & `types-aiobotocore-redshift-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.893485 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.986643 types-aiobotocore-redshift-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14041 2023-08-04 13:59:22.986643 types-aiobotocore-redshift-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12490 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.986643 types-aiobotocore-redshift-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2123 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.956643 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1686 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1685 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      985 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15175 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15150 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8679 2023-08-04 13:50:28.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8677 2023-08-04 13:50:28.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8723 2023-08-04 13:50:28.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8715 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16702 2023-08-04 13:50:29.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16673 2023-08-04 13:50:29.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:25.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.986643 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14041 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/LICENSE` & `types-aiobotocore-redshift-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-redshift-data-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,79 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_redshift_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `RedshiftDataAPIService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/literals/).
+
 ```python
-from types_aiobotocore_redshift_data.literals import (
-    DescribeTablePaginatorName,
-    GetStatementResultPaginatorName,
-    ListDatabasesPaginatorName,
-    ListSchemasPaginatorName,
-    ListStatementsPaginatorName,
-    ListTablesPaginatorName,
-    StatementStatusStringType,
-    StatusStringType,
-    RedshiftDataAPIServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_redshift_data.literals import DescribeTablePaginatorName
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RedshiftDataAPIService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/type_defs/).
+
 ```python
-from types_aiobotocore_redshift_data.type_defs import (
-    BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CancelStatementRequestRequestTypeDef,
-    ColumnMetadataTypeDef,
-    DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
-    SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeTableRequestRequestTypeDef,
-    FieldTypeDef,
-    GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestRequestTypeDef,
-    ListSchemasRequestRequestTypeDef,
-    ListStatementsRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    StatementDataTypeDef,
-    DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    GetStatementResultResponseTypeDef,
-    ListTablesResponseTypeDef,
-    ListStatementsResponseTypeDef,
-)
+from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
 
 
 def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/README.md` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-redshift-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,79 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_redshift_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `RedshiftDataAPIService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/literals/).
+
 ```python
-from types_aiobotocore_redshift_data.literals import (
-    DescribeTablePaginatorName,
-    GetStatementResultPaginatorName,
-    ListDatabasesPaginatorName,
-    ListSchemasPaginatorName,
-    ListStatementsPaginatorName,
-    ListTablesPaginatorName,
-    StatementStatusStringType,
-    StatusStringType,
-    RedshiftDataAPIServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_redshift_data.literals import DescribeTablePaginatorName
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RedshiftDataAPIService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/type_defs/).
+
 ```python
-from types_aiobotocore_redshift_data.type_defs import (
-    BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CancelStatementRequestRequestTypeDef,
-    ColumnMetadataTypeDef,
-    DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
-    SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeTableRequestRequestTypeDef,
-    FieldTypeDef,
-    GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestRequestTypeDef,
-    ListSchemasRequestRequestTypeDef,
-    ListStatementsRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    StatementDataTypeDef,
-    DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    GetStatementResultResponseTypeDef,
-    ListTablesResponseTypeDef,
-    ListStatementsResponseTypeDef,
-)
+from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
 
 
 def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/setup.py` & `types-aiobotocore-redshift-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.pyi` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__main__.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
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

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.pyi` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.pyi` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -158,14 +159,15 @@
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
@@ -244,26 +246,28 @@
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

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.pyi` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.py` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.pyi` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/PKG-INFO` & `types-aiobotocore-redshift-data-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-redshift-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,79 +271,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_redshift_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `RedshiftDataAPIService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/literals/).
+
 ```python
-from types_aiobotocore_redshift_data.literals import (
-    DescribeTablePaginatorName,
-    GetStatementResultPaginatorName,
-    ListDatabasesPaginatorName,
-    ListSchemasPaginatorName,
-    ListStatementsPaginatorName,
-    ListTablesPaginatorName,
-    StatementStatusStringType,
-    StatusStringType,
-    RedshiftDataAPIServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_redshift_data.literals import DescribeTablePaginatorName
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RedshiftDataAPIService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/type_defs/).
+
 ```python
-from types_aiobotocore_redshift_data.type_defs import (
-    BatchExecuteStatementInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CancelStatementRequestRequestTypeDef,
-    ColumnMetadataTypeDef,
-    DescribeStatementRequestRequestTypeDef,
-    SqlParameterTypeDef,
-    SubStatementDataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeTableRequestRequestTypeDef,
-    FieldTypeDef,
-    GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestRequestTypeDef,
-    ListSchemasRequestRequestTypeDef,
-    ListStatementsRequestRequestTypeDef,
-    ListTablesRequestRequestTypeDef,
-    TableMemberTypeDef,
-    BatchExecuteStatementOutputTypeDef,
-    CancelStatementResponseTypeDef,
-    ExecuteStatementOutputTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasResponseTypeDef,
-    DescribeTableResponseTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    StatementDataTypeDef,
-    DescribeStatementResponseTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
-    GetStatementResultResponseTypeDef,
-    ListTablesResponseTypeDef,
-    ListStatementsResponseTypeDef,
-)
+from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
 
 
 def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-data-2.5.2.post2/types_aiobotocore_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

