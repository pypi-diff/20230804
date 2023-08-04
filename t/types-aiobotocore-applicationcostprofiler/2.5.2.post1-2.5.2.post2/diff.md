# Comparing `tmp/types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-applicationcostprofiler-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.817654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-02 14:33:16.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 14:33:16.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.479113 types-aiobotocore-applicationcostprofiler-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:00:25.475113 types-aiobotocore-applicationcostprofiler-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.479113 types-aiobotocore-applicationcostprofiler-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.471113 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:23.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.475113 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 12:00:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/LICENSE` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_applicationcostprofiler.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApplicationCostProfiler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/literals/).
+
 ```python
-from types_aiobotocore_applicationcostprofiler.literals import (
-    FormatType,
-    ListReportDefinitionsPaginatorName,
-    ReportFrequencyType,
-    S3BucketRegionType,
-    ApplicationCostProfilerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_applicationcostprofiler.literals import FormatType
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApplicationCostProfiler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/type_defs/).
+
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetReportDefinitionRequestRequestTypeDef,
-    S3LocationTypeDef,
-    SourceS3LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    PutReportDefinitionResultTypeDef,
-    UpdateReportDefinitionResultTypeDef,
-    GetReportDefinitionResultTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
-    UpdateReportDefinitionRequestRequestTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/README.md` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/README.md`

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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,59 +259,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_applicationcostprofiler.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApplicationCostProfiler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/literals/).
+
 ```python
-from types_aiobotocore_applicationcostprofiler.literals import (
-    FormatType,
-    ListReportDefinitionsPaginatorName,
-    ReportFrequencyType,
-    S3BucketRegionType,
-    ApplicationCostProfilerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_applicationcostprofiler.literals import FormatType
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApplicationCostProfiler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/type_defs/).
+
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetReportDefinitionRequestRequestTypeDef,
-    S3LocationTypeDef,
-    SourceS3LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    PutReportDefinitionResultTypeDef,
-    UpdateReportDefinitionResultTypeDef,
-    GetReportDefinitionResultTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
-    UpdateReportDefinitionRequestRequestTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-applicationcostprofiler",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_applicationcostprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__main__.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler\nOther"
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_applicationcostprofiler.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApplicationCostProfiler` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/literals/).
+
 ```python
-from types_aiobotocore_applicationcostprofiler.literals import (
-    FormatType,
-    ListReportDefinitionsPaginatorName,
-    ReportFrequencyType,
-    S3BucketRegionType,
-    ApplicationCostProfilerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_applicationcostprofiler.literals import FormatType
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApplicationCostProfiler` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/type_defs/).
+
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetReportDefinitionRequestRequestTypeDef,
-    S3LocationTypeDef,
-    SourceS3LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    PutReportDefinitionResultTypeDef,
-    UpdateReportDefinitionResultTypeDef,
-    GetReportDefinitionResultTypeDef,
-    PutReportDefinitionRequestRequestTypeDef,
-    ReportDefinitionTypeDef,
-    UpdateReportDefinitionRequestRequestTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-applicationcostprofiler-2.5.2.post2/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

