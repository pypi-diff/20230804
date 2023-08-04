# Comparing `tmp/types-aiobotocore-cur-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cur-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cur-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-cur-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
```

## Comparing `types-aiobotocore-cur-2.5.2.post1.tar` & `types-aiobotocore-cur-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.493612 types-aiobotocore-cur-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-08-02 14:52:07.493612 types-aiobotocore-cur-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.493612 types-aiobotocore-cur-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.489612 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-02 14:35:58.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-02 14:35:58.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-02 14:35:58.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-08-02 14:35:58.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:57.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.493612 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:07.000000 types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 11:43:16.000000 types-aiobotocore-cur-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.195753 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:17.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:42.000000 types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/LICENSE` & `types-aiobotocore-cur-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cur-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,58 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cur.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CostandUsageReportService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/literals/).
+
 ```python
-from types_aiobotocore_cur.literals import (
-    AWSRegionType,
-    AdditionalArtifactType,
-    CompressionFormatType,
-    DescribeReportDefinitionsPaginatorName,
-    ReportFormatType,
-    ReportVersioningType,
-    SchemaElementType,
-    TimeUnitType,
-    CostandUsageReportServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cur.literals import AWSRegionType
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cur.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CostandUsageReportService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/type_defs/).
+
 ```python
-from types_aiobotocore_cur.type_defs import (
-    DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionOutputTypeDef,
-    ReportDefinitionTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
-    DescribeReportDefinitionsResponseTypeDef,
-    ModifyReportDefinitionRequestRequestTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionUnionTypeDef,
-)
+from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/README.md` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-cur
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore cur type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cur"></a>
 
 # types-aiobotocore-cur
 
 [![PyPI - types-aiobotocore-cur](https://img.shields.io/pypi/v/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -258,58 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cur.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CostandUsageReportService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/literals/).
+
 ```python
-from types_aiobotocore_cur.literals import (
-    AWSRegionType,
-    AdditionalArtifactType,
-    CompressionFormatType,
-    DescribeReportDefinitionsPaginatorName,
-    ReportFormatType,
-    ReportVersioningType,
-    SchemaElementType,
-    TimeUnitType,
-    CostandUsageReportServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cur.literals import AWSRegionType
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cur.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CostandUsageReportService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/type_defs/).
+
 ```python
-from types_aiobotocore_cur.type_defs import (
-    DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionOutputTypeDef,
-    ReportDefinitionTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
-    DescribeReportDefinitionsResponseTypeDef,
-    ModifyReportDefinitionRequestRequestTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionUnionTypeDef,
-)
+from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/setup.py` & `types-aiobotocore-cur-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cur",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__init__.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__init__.pyi` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/__main__.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CostandUsageReportService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/client.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
-    ReportDefinitionUnionTypeDef,
+    ReportDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -116,25 +116,25 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#generate_presigned_url)
         """
 
     async def modify_report_definition(
-        self, *, ReportName: str, ReportDefinition: ReportDefinitionUnionTypeDef
+        self, *, ReportName: str, ReportDefinition: ReportDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#modify_report_definition)
         """
 
     async def put_report_definition(
-        self, *, ReportDefinition: ReportDefinitionUnionTypeDef
+        self, *, ReportDefinition: ReportDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#put_report_definition)
         """
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/client.pyi` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
-    ReportDefinitionUnionTypeDef,
+    ReportDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -106,24 +106,24 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#generate_presigned_url)
         """
     async def modify_report_definition(
-        self, *, ReportName: str, ReportDefinition: ReportDefinitionUnionTypeDef
+        self, *, ReportName: str, ReportDefinition: ReportDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#modify_report_definition)
         """
     async def put_report_definition(
-        self, *, ReportDefinition: ReportDefinitionUnionTypeDef
+        self, *, ReportDefinition: ReportDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/client/#put_report_definition)
         """
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/literals.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/literals.pyi` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/paginator.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/paginator.pyi` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/type_defs.py` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
     data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -31,22 +31,20 @@
 
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
-    "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
-    "ReportDefinitionUnionTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
@@ -79,62 +77,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredReportDefinitionOutputTypeDef = TypedDict(
-    "_RequiredReportDefinitionOutputTypeDef",
-    {
-        "ReportName": str,
-        "TimeUnit": TimeUnitType,
-        "Format": ReportFormatType,
-        "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[SchemaElementType],
-        "S3Bucket": str,
-        "S3Prefix": str,
-        "S3Region": AWSRegionType,
-    },
-)
-_OptionalReportDefinitionOutputTypeDef = TypedDict(
-    "_OptionalReportDefinitionOutputTypeDef",
-    {
-        "AdditionalArtifacts": List[AdditionalArtifactType],
-        "RefreshClosedReports": bool,
-        "ReportVersioning": ReportVersioningType,
-        "BillingViewArn": str,
-    },
-    total=False,
-)
-
-
-class ReportDefinitionOutputTypeDef(
-    _RequiredReportDefinitionOutputTypeDef, _OptionalReportDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": Sequence[SchemaElementType],
+        "AdditionalSchemaElements": List[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
     {
-        "AdditionalArtifacts": Sequence[AdditionalArtifactType],
+        "AdditionalArtifacts": List[AdditionalArtifactType],
         "RefreshClosedReports": bool,
         "ReportVersioning": ReportVersioningType,
         "BillingViewArn": str,
     },
     total=False,
 )
 
@@ -158,15 +125,15 @@
     },
     total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
-        "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
+        "ReportDefinitions": List[ReportDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
@@ -178,9 +145,7 @@
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "ReportDefinition": ReportDefinitionTypeDef,
     },
 )
-
-ReportDefinitionUnionTypeDef = Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur/type_defs.pyi` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
     data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -30,22 +30,20 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
-    "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
-    "ReportDefinitionUnionTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
@@ -78,60 +76,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredReportDefinitionOutputTypeDef = TypedDict(
-    "_RequiredReportDefinitionOutputTypeDef",
-    {
-        "ReportName": str,
-        "TimeUnit": TimeUnitType,
-        "Format": ReportFormatType,
-        "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[SchemaElementType],
-        "S3Bucket": str,
-        "S3Prefix": str,
-        "S3Region": AWSRegionType,
-    },
-)
-_OptionalReportDefinitionOutputTypeDef = TypedDict(
-    "_OptionalReportDefinitionOutputTypeDef",
-    {
-        "AdditionalArtifacts": List[AdditionalArtifactType],
-        "RefreshClosedReports": bool,
-        "ReportVersioning": ReportVersioningType,
-        "BillingViewArn": str,
-    },
-    total=False,
-)
-
-class ReportDefinitionOutputTypeDef(
-    _RequiredReportDefinitionOutputTypeDef, _OptionalReportDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": Sequence[SchemaElementType],
+        "AdditionalSchemaElements": List[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
     {
-        "AdditionalArtifacts": Sequence[AdditionalArtifactType],
+        "AdditionalArtifacts": List[AdditionalArtifactType],
         "RefreshClosedReports": bool,
         "ReportVersioning": ReportVersioningType,
         "BillingViewArn": str,
     },
     total=False,
 )
 
@@ -153,15 +122,15 @@
     },
     total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
-        "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
+        "ReportDefinitions": List[ReportDefinitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
@@ -173,9 +142,7 @@
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "ReportDefinition": ReportDefinitionTypeDef,
     },
 )
-
-ReportDefinitionUnionTypeDef = Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/PKG-INFO` & `types-aiobotocore-cur-2.5.2.post2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-cur
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cur type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cur"></a>
 
 # types-aiobotocore-cur
 
 [![PyPI - types-aiobotocore-cur](https://img.shields.io/pypi/v/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
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
 [types-aiobotocore-cur docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,58 +258,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cur.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `CostandUsageReportService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/literals/).
+
 ```python
-from types_aiobotocore_cur.literals import (
-    AWSRegionType,
-    AdditionalArtifactType,
-    CompressionFormatType,
-    DescribeReportDefinitionsPaginatorName,
-    ReportFormatType,
-    ReportVersioningType,
-    SchemaElementType,
-    TimeUnitType,
-    CostandUsageReportServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cur.literals import AWSRegionType
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cur.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CostandUsageReportService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/type_defs/).
+
 ```python
-from types_aiobotocore_cur.type_defs import (
-    DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeReportDefinitionsRequestRequestTypeDef,
-    ReportDefinitionOutputTypeDef,
-    ReportDefinitionTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
-    DescribeReportDefinitionsResponseTypeDef,
-    ModifyReportDefinitionRequestRequestTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionUnionTypeDef,
-)
+from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cur-2.5.2.post1/types_aiobotocore_cur.egg-info/SOURCES.txt` & `types-aiobotocore-cur-2.5.2.post2/types_aiobotocore_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

