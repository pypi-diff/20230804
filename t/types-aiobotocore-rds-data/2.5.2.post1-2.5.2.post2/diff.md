# Comparing `tmp/types-aiobotocore-rds-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rds-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rds-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-rds-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-rds-data-2.5.2.post1.tar` & `types-aiobotocore-rds-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.661489 types-aiobotocore-rds-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-08-02 14:52:50.661489 types-aiobotocore-rds-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.661489 types-aiobotocore-rds-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-02 14:47:33.000000 types-aiobotocore-rds-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.661489 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:34.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.661489 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:50.000000 types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.716643 types-aiobotocore-rds-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:22.716643 types-aiobotocore-rds-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10765 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.716643 types-aiobotocore-rds-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2085 2023-08-04 13:50:12.000000 types-aiobotocore-rds-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.716643 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      480 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      479 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8553 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8539 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8291 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8289 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8948 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8939 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:13.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.716643 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:22.000000 types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/LICENSE` & `types-aiobotocore-rds-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-rds-data-2.5.2.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rds-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,72 +266,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rds_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `RDSDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/literals/).
+
 ```python
-from types_aiobotocore_rds_data.literals import (
-    DecimalReturnTypeType,
-    LongReturnTypeType,
-    RecordsFormatTypeType,
-    TypeHintType,
-    RDSDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_rds_data.literals import DecimalReturnTypeType
 
 
 def check_value(value: DecimalReturnTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rds_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RDSDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/type_defs/).
+
 ```python
-from types_aiobotocore_rds_data.type_defs import (
-    ArrayValueOutputTypeDef,
-    ArrayValueTypeDef,
-    ResponseMetadataTypeDef,
-    BeginTransactionRequestRequestTypeDef,
-    BlobTypeDef,
-    ColumnMetadataTypeDef,
-    CommitTransactionRequestRequestTypeDef,
-    ExecuteSqlRequestRequestTypeDef,
-    ResultSetOptionsTypeDef,
-    FieldOutputTypeDef,
-    RecordTypeDef,
-    RollbackTransactionRequestRequestTypeDef,
-    StructValueTypeDef,
-    ValueTypeDef,
-    BeginTransactionResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    RollbackTransactionResponseTypeDef,
-    FieldTypeDef,
-    ResultSetMetadataTypeDef,
-    ExecuteStatementResponseTypeDef,
-    UpdateResultTypeDef,
-    SqlParameterTypeDef,
-    ResultFrameTypeDef,
-    BatchExecuteStatementResponseTypeDef,
-    BatchExecuteStatementRequestRequestTypeDef,
-    ExecuteStatementRequestRequestTypeDef,
-    SqlStatementResultTypeDef,
-    ExecuteSqlResponseTypeDef,
-)
+from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef
 
 
-def get_value() -> ArrayValueOutputTypeDef:
+def get_value() -> ArrayValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/README.md` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-rds-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore rds-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rds-data"></a>
 
 # types-aiobotocore-rds-data
 
 [![PyPI - types-aiobotocore-rds-data](https://img.shields.io/pypi/v/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,72 +266,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rds_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `RDSDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/literals/).
+
 ```python
-from types_aiobotocore_rds_data.literals import (
-    DecimalReturnTypeType,
-    LongReturnTypeType,
-    RecordsFormatTypeType,
-    TypeHintType,
-    RDSDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_rds_data.literals import DecimalReturnTypeType
 
 
 def check_value(value: DecimalReturnTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rds_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RDSDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/type_defs/).
+
 ```python
-from types_aiobotocore_rds_data.type_defs import (
-    ArrayValueOutputTypeDef,
-    ArrayValueTypeDef,
-    ResponseMetadataTypeDef,
-    BeginTransactionRequestRequestTypeDef,
-    BlobTypeDef,
-    ColumnMetadataTypeDef,
-    CommitTransactionRequestRequestTypeDef,
-    ExecuteSqlRequestRequestTypeDef,
-    ResultSetOptionsTypeDef,
-    FieldOutputTypeDef,
-    RecordTypeDef,
-    RollbackTransactionRequestRequestTypeDef,
-    StructValueTypeDef,
-    ValueTypeDef,
-    BeginTransactionResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    RollbackTransactionResponseTypeDef,
-    FieldTypeDef,
-    ResultSetMetadataTypeDef,
-    ExecuteStatementResponseTypeDef,
-    UpdateResultTypeDef,
-    SqlParameterTypeDef,
-    ResultFrameTypeDef,
-    BatchExecuteStatementResponseTypeDef,
-    BatchExecuteStatementRequestRequestTypeDef,
-    ExecuteStatementRequestRequestTypeDef,
-    SqlStatementResultTypeDef,
-    ExecuteSqlResponseTypeDef,
-)
+from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef
 
 
-def get_value() -> ArrayValueOutputTypeDef:
+def get_value() -> ArrayValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/setup.py` & `types-aiobotocore-rds-data-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rds-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rds_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/__main__.py` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.RDSDataService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService\nOther"
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

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/client.py` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/client.pyi` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/literals.py` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DecimalReturnTypeType",
     "LongReturnTypeType",
     "RecordsFormatTypeType",
     "TypeHintType",
     "RDSDataServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DecimalReturnTypeType = Literal["DOUBLE_OR_LONG", "STRING"]
 LongReturnTypeType = Literal["LONG", "STRING"]
 RecordsFormatTypeType = Literal["JSON", "NONE"]
 TypeHintType = Literal["DATE", "DECIMAL", "JSON", "TIME", "TIMESTAMP", "UUID"]
 RDSDataServiceServiceName = Literal["rds-data"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -47,14 +45,15 @@
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
@@ -150,14 +149,15 @@
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
@@ -236,26 +236,28 @@
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

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/literals.pyi` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DecimalReturnTypeType",
     "LongReturnTypeType",
     "RecordsFormatTypeType",
     "TypeHintType",
     "RDSDataServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 DecimalReturnTypeType = Literal["DOUBLE_OR_LONG", "STRING"]
 LongReturnTypeType = Literal["LONG", "STRING"]
 RecordsFormatTypeType = Literal["JSON", "NONE"]
 TypeHintType = Literal["DATE", "DECIMAL", "JSON", "TIME", "TIMESTAMP", "UUID"]
 RDSDataServiceServiceName = Literal["rds-data"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -45,14 +47,15 @@
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
@@ -148,14 +151,15 @@
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
@@ -234,26 +238,28 @@
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

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/type_defs.py` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,75 +2,60 @@
 Type annotations for rds-data service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rds_data.type_defs import ArrayValueOutputTypeDef
+    from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef
 
-    data: ArrayValueOutputTypeDef = ...
+    data: ArrayValueTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import DecimalReturnTypeType, LongReturnTypeType, RecordsFormatTypeType, TypeHintType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "ArrayValueOutputTypeDef",
     "ArrayValueTypeDef",
     "ResponseMetadataTypeDef",
     "BeginTransactionRequestRequestTypeDef",
     "BlobTypeDef",
     "ColumnMetadataTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "ExecuteSqlRequestRequestTypeDef",
     "ResultSetOptionsTypeDef",
-    "FieldOutputTypeDef",
     "RecordTypeDef",
     "RollbackTransactionRequestRequestTypeDef",
     "StructValueTypeDef",
     "ValueTypeDef",
     "BeginTransactionResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "RollbackTransactionResponseTypeDef",
     "FieldTypeDef",
     "ResultSetMetadataTypeDef",
     "ExecuteStatementResponseTypeDef",
-    "UpdateResultTypeDef",
     "SqlParameterTypeDef",
+    "UpdateResultTypeDef",
     "ResultFrameTypeDef",
-    "BatchExecuteStatementResponseTypeDef",
     "BatchExecuteStatementRequestRequestTypeDef",
     "ExecuteStatementRequestRequestTypeDef",
+    "BatchExecuteStatementResponseTypeDef",
     "SqlStatementResultTypeDef",
     "ExecuteSqlResponseTypeDef",
 )
 
-ArrayValueOutputTypeDef = TypedDict(
-    "ArrayValueOutputTypeDef",
-    {
-        "booleanValues": List[bool],
-        "longValues": List[int],
-        "doubleValues": List[float],
-        "stringValues": List[str],
-        "arrayValues": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 ArrayValueTypeDef = TypedDict(
     "ArrayValueTypeDef",
     {
         "booleanValues": Sequence[bool],
         "longValues": Sequence[int],
         "doubleValues": Sequence[float],
         "stringValues": Sequence[str],
@@ -102,21 +87,19 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
-
 class BeginTransactionRequestRequestTypeDef(
     _RequiredBeginTransactionRequestRequestTypeDef, _OptionalBeginTransactionRequestRequestTypeDef
 ):
     pass
 
-
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "name": str,
         "type": int,
         "typeName": str,
@@ -157,44 +140,28 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
-
 class ExecuteSqlRequestRequestTypeDef(
     _RequiredExecuteSqlRequestRequestTypeDef, _OptionalExecuteSqlRequestRequestTypeDef
 ):
     pass
 
-
 ResultSetOptionsTypeDef = TypedDict(
     "ResultSetOptionsTypeDef",
     {
         "decimalReturnType": DecimalReturnTypeType,
         "longReturnType": LongReturnTypeType,
     },
     total=False,
 )
 
-FieldOutputTypeDef = TypedDict(
-    "FieldOutputTypeDef",
-    {
-        "isNull": bool,
-        "booleanValue": bool,
-        "longValue": int,
-        "doubleValue": float,
-        "stringValue": str,
-        "blobValue": bytes,
-        "arrayValue": "ArrayValueOutputTypeDef",
-    },
-    total=False,
-)
-
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "values": List["ValueTypeDef"],
     },
     total=False,
 )
@@ -207,15 +174,15 @@
         "transactionId": str,
     },
 )
 
 StructValueTypeDef = TypedDict(
     "StructValueTypeDef",
     {
-        "attributes": List[Dict[str, Any]],
+        "attributes": List["ValueTypeDef"],
     },
     total=False,
 )
 
 ValueTypeDef = TypedDict(
     "ValueTypeDef",
     {
@@ -279,56 +246,48 @@
     },
     total=False,
 )
 
 ExecuteStatementResponseTypeDef = TypedDict(
     "ExecuteStatementResponseTypeDef",
     {
-        "records": List[List[FieldOutputTypeDef]],
+        "records": List[List[FieldTypeDef]],
         "columnMetadata": List[ColumnMetadataTypeDef],
         "numberOfRecordsUpdated": int,
-        "generatedFields": List[FieldOutputTypeDef],
+        "generatedFields": List[FieldTypeDef],
         "formattedRecords": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateResultTypeDef = TypedDict(
-    "UpdateResultTypeDef",
-    {
-        "generatedFields": List[FieldOutputTypeDef],
-    },
-    total=False,
-)
-
 SqlParameterTypeDef = TypedDict(
     "SqlParameterTypeDef",
     {
         "name": str,
         "value": FieldTypeDef,
         "typeHint": TypeHintType,
     },
     total=False,
 )
 
-ResultFrameTypeDef = TypedDict(
-    "ResultFrameTypeDef",
+UpdateResultTypeDef = TypedDict(
+    "UpdateResultTypeDef",
     {
-        "resultSetMetadata": ResultSetMetadataTypeDef,
-        "records": List[RecordTypeDef],
+        "generatedFields": List[FieldTypeDef],
     },
     total=False,
 )
 
-BatchExecuteStatementResponseTypeDef = TypedDict(
-    "BatchExecuteStatementResponseTypeDef",
+ResultFrameTypeDef = TypedDict(
+    "ResultFrameTypeDef",
     {
-        "updateResults": List[UpdateResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resultSetMetadata": ResultSetMetadataTypeDef,
+        "records": List[RecordTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
@@ -342,22 +301,20 @@
         "schema": str,
         "parameterSets": Sequence[Sequence[SqlParameterTypeDef]],
         "transactionId": str,
     },
     total=False,
 )
 
-
 class BatchExecuteStatementRequestRequestTypeDef(
     _RequiredBatchExecuteStatementRequestRequestTypeDef,
     _OptionalBatchExecuteStatementRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -373,20 +330,26 @@
         "continueAfterTimeout": bool,
         "resultSetOptions": ResultSetOptionsTypeDef,
         "formatRecordsAs": RecordsFormatTypeType,
     },
     total=False,
 )
 
-
 class ExecuteStatementRequestRequestTypeDef(
     _RequiredExecuteStatementRequestRequestTypeDef, _OptionalExecuteStatementRequestRequestTypeDef
 ):
     pass
 
+BatchExecuteStatementResponseTypeDef = TypedDict(
+    "BatchExecuteStatementResponseTypeDef",
+    {
+        "updateResults": List[UpdateResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 SqlStatementResultTypeDef = TypedDict(
     "SqlStatementResultTypeDef",
     {
         "resultFrame": ResultFrameTypeDef,
         "numberOfRecordsUpdated": int,
     },
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data/type_defs.pyi` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,74 +2,61 @@
 Type annotations for rds-data service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_rds_data.type_defs import ArrayValueOutputTypeDef
+    from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef
 
-    data: ArrayValueOutputTypeDef = ...
+    data: ArrayValueTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import DecimalReturnTypeType, LongReturnTypeType, RecordsFormatTypeType, TypeHintType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "ArrayValueOutputTypeDef",
     "ArrayValueTypeDef",
     "ResponseMetadataTypeDef",
     "BeginTransactionRequestRequestTypeDef",
     "BlobTypeDef",
     "ColumnMetadataTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "ExecuteSqlRequestRequestTypeDef",
     "ResultSetOptionsTypeDef",
-    "FieldOutputTypeDef",
     "RecordTypeDef",
     "RollbackTransactionRequestRequestTypeDef",
     "StructValueTypeDef",
     "ValueTypeDef",
     "BeginTransactionResponseTypeDef",
     "CommitTransactionResponseTypeDef",
     "RollbackTransactionResponseTypeDef",
     "FieldTypeDef",
     "ResultSetMetadataTypeDef",
     "ExecuteStatementResponseTypeDef",
-    "UpdateResultTypeDef",
     "SqlParameterTypeDef",
+    "UpdateResultTypeDef",
     "ResultFrameTypeDef",
-    "BatchExecuteStatementResponseTypeDef",
     "BatchExecuteStatementRequestRequestTypeDef",
     "ExecuteStatementRequestRequestTypeDef",
+    "BatchExecuteStatementResponseTypeDef",
     "SqlStatementResultTypeDef",
     "ExecuteSqlResponseTypeDef",
 )
 
-ArrayValueOutputTypeDef = TypedDict(
-    "ArrayValueOutputTypeDef",
-    {
-        "booleanValues": List[bool],
-        "longValues": List[int],
-        "doubleValues": List[float],
-        "stringValues": List[str],
-        "arrayValues": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 ArrayValueTypeDef = TypedDict(
     "ArrayValueTypeDef",
     {
         "booleanValues": Sequence[bool],
         "longValues": Sequence[int],
         "doubleValues": Sequence[float],
         "stringValues": Sequence[str],
@@ -101,19 +88,21 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
+
 class BeginTransactionRequestRequestTypeDef(
     _RequiredBeginTransactionRequestRequestTypeDef, _OptionalBeginTransactionRequestRequestTypeDef
 ):
     pass
 
+
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "name": str,
         "type": int,
         "typeName": str,
@@ -154,42 +143,30 @@
     {
         "database": str,
         "schema": str,
     },
     total=False,
 )
 
+
 class ExecuteSqlRequestRequestTypeDef(
     _RequiredExecuteSqlRequestRequestTypeDef, _OptionalExecuteSqlRequestRequestTypeDef
 ):
     pass
 
+
 ResultSetOptionsTypeDef = TypedDict(
     "ResultSetOptionsTypeDef",
     {
         "decimalReturnType": DecimalReturnTypeType,
         "longReturnType": LongReturnTypeType,
     },
     total=False,
 )
 
-FieldOutputTypeDef = TypedDict(
-    "FieldOutputTypeDef",
-    {
-        "isNull": bool,
-        "booleanValue": bool,
-        "longValue": int,
-        "doubleValue": float,
-        "stringValue": str,
-        "blobValue": bytes,
-        "arrayValue": "ArrayValueOutputTypeDef",
-    },
-    total=False,
-)
-
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "values": List["ValueTypeDef"],
     },
     total=False,
 )
@@ -202,15 +179,15 @@
         "transactionId": str,
     },
 )
 
 StructValueTypeDef = TypedDict(
     "StructValueTypeDef",
     {
-        "attributes": List[Dict[str, Any]],
+        "attributes": List["ValueTypeDef"],
     },
     total=False,
 )
 
 ValueTypeDef = TypedDict(
     "ValueTypeDef",
     {
@@ -274,56 +251,48 @@
     },
     total=False,
 )
 
 ExecuteStatementResponseTypeDef = TypedDict(
     "ExecuteStatementResponseTypeDef",
     {
-        "records": List[List[FieldOutputTypeDef]],
+        "records": List[List[FieldTypeDef]],
         "columnMetadata": List[ColumnMetadataTypeDef],
         "numberOfRecordsUpdated": int,
-        "generatedFields": List[FieldOutputTypeDef],
+        "generatedFields": List[FieldTypeDef],
         "formattedRecords": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateResultTypeDef = TypedDict(
-    "UpdateResultTypeDef",
-    {
-        "generatedFields": List[FieldOutputTypeDef],
-    },
-    total=False,
-)
-
 SqlParameterTypeDef = TypedDict(
     "SqlParameterTypeDef",
     {
         "name": str,
         "value": FieldTypeDef,
         "typeHint": TypeHintType,
     },
     total=False,
 )
 
-ResultFrameTypeDef = TypedDict(
-    "ResultFrameTypeDef",
+UpdateResultTypeDef = TypedDict(
+    "UpdateResultTypeDef",
     {
-        "resultSetMetadata": ResultSetMetadataTypeDef,
-        "records": List[RecordTypeDef],
+        "generatedFields": List[FieldTypeDef],
     },
     total=False,
 )
 
-BatchExecuteStatementResponseTypeDef = TypedDict(
-    "BatchExecuteStatementResponseTypeDef",
+ResultFrameTypeDef = TypedDict(
+    "ResultFrameTypeDef",
     {
-        "updateResults": List[UpdateResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resultSetMetadata": ResultSetMetadataTypeDef,
+        "records": List[RecordTypeDef],
     },
+    total=False,
 )
 
 _RequiredBatchExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
@@ -337,20 +306,22 @@
         "schema": str,
         "parameterSets": Sequence[Sequence[SqlParameterTypeDef]],
         "transactionId": str,
     },
     total=False,
 )
 
+
 class BatchExecuteStatementRequestRequestTypeDef(
     _RequiredBatchExecuteStatementRequestRequestTypeDef,
     _OptionalBatchExecuteStatementRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredExecuteStatementRequestRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "secretArn": str,
         "sql": str,
     },
@@ -366,19 +337,29 @@
         "continueAfterTimeout": bool,
         "resultSetOptions": ResultSetOptionsTypeDef,
         "formatRecordsAs": RecordsFormatTypeType,
     },
     total=False,
 )
 
+
 class ExecuteStatementRequestRequestTypeDef(
     _RequiredExecuteStatementRequestRequestTypeDef, _OptionalExecuteStatementRequestRequestTypeDef
 ):
     pass
 
+
+BatchExecuteStatementResponseTypeDef = TypedDict(
+    "BatchExecuteStatementResponseTypeDef",
+    {
+        "updateResults": List[UpdateResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SqlStatementResultTypeDef = TypedDict(
     "SqlStatementResultTypeDef",
     {
         "resultFrame": ResultFrameTypeDef,
         "numberOfRecordsUpdated": int,
     },
     total=False,
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/PKG-INFO` & `types-aiobotocore-rds-data-2.5.2.post2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-rds-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.RDSDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore rds-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rds-data"></a>
 
 # types-aiobotocore-rds-data
 
 [![PyPI - types-aiobotocore-rds-data](https://img.shields.io/pypi/v/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rds-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rds-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/)
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
 [types-aiobotocore-rds-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,72 +234,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rds_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `RDSDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/literals/).
+
 ```python
-from types_aiobotocore_rds_data.literals import (
-    DecimalReturnTypeType,
-    LongReturnTypeType,
-    RecordsFormatTypeType,
-    TypeHintType,
-    RDSDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_rds_data.literals import DecimalReturnTypeType
 
 
 def check_value(value: DecimalReturnTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rds_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RDSDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds_data/type_defs/).
+
 ```python
-from types_aiobotocore_rds_data.type_defs import (
-    ArrayValueOutputTypeDef,
-    ArrayValueTypeDef,
-    ResponseMetadataTypeDef,
-    BeginTransactionRequestRequestTypeDef,
-    BlobTypeDef,
-    ColumnMetadataTypeDef,
-    CommitTransactionRequestRequestTypeDef,
-    ExecuteSqlRequestRequestTypeDef,
-    ResultSetOptionsTypeDef,
-    FieldOutputTypeDef,
-    RecordTypeDef,
-    RollbackTransactionRequestRequestTypeDef,
-    StructValueTypeDef,
-    ValueTypeDef,
-    BeginTransactionResponseTypeDef,
-    CommitTransactionResponseTypeDef,
-    RollbackTransactionResponseTypeDef,
-    FieldTypeDef,
-    ResultSetMetadataTypeDef,
-    ExecuteStatementResponseTypeDef,
-    UpdateResultTypeDef,
-    SqlParameterTypeDef,
-    ResultFrameTypeDef,
-    BatchExecuteStatementResponseTypeDef,
-    BatchExecuteStatementRequestRequestTypeDef,
-    ExecuteStatementRequestRequestTypeDef,
-    SqlStatementResultTypeDef,
-    ExecuteSqlResponseTypeDef,
-)
+from types_aiobotocore_rds_data.type_defs import ArrayValueTypeDef
 
 
-def get_value() -> ArrayValueOutputTypeDef:
+def get_value() -> ArrayValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-rds-data-2.5.2.post1/types_aiobotocore_rds_data.egg-info/SOURCES.txt` & `types-aiobotocore-rds-data-2.5.2.post2/types_aiobotocore_rds_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

