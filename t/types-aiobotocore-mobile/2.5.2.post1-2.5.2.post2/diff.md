# Comparing `tmp/types-aiobotocore-mobile-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mobile-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mobile-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-mobile-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-mobile-2.5.2.post1.tar` & `types-aiobotocore-mobile-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.649514 types-aiobotocore-mobile-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-08-02 14:52:42.649514 types-aiobotocore-mobile-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:42.649514 types-aiobotocore-mobile-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.645514 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-08-02 14:43:48.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-08-02 14:43:48.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:47.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.649514 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:42.000000 types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12934 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11420 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      791 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      790 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10204 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10184 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8070 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8068 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2941 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2937 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7655 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7648 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12934 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mobile-2.5.2.post1/LICENSE` & `types-aiobotocore-mobile-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/PKG-INFO` & `types-aiobotocore-mobile-2.5.2.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,68 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mobile.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Mobile` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/literals/).
+
 ```python
-from types_aiobotocore_mobile.literals import (
-    ListBundlesPaginatorName,
-    ListProjectsPaginatorName,
-    PlatformType,
-    ProjectStateType,
-    MobileServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_mobile.literals import ListBundlesPaginatorName
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mobile.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Mobile` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/type_defs/).
+
 ```python
-from types_aiobotocore_mobile.type_defs import (
-    BlobTypeDef,
-    BundleDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    ResourceTypeDef,
-    DescribeBundleRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ExportBundleRequestRequestTypeDef,
-    ExportProjectRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeBundleResultTypeDef,
-    ExportBundleResultTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesResultTypeDef,
-    DeleteProjectResultTypeDef,
-    ProjectDetailsTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    CreateProjectResultTypeDef,
-    DescribeProjectResultTypeDef,
-    UpdateProjectResultTypeDef,
-)
+from types_aiobotocore_mobile.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mobile-2.5.2.post1/README.md` & `types-aiobotocore-mobile-2.5.2.post2/README.md`

 * *Files 20% similar despite different names*

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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,68 +257,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mobile.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Mobile` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/literals/).
+
 ```python
-from types_aiobotocore_mobile.literals import (
-    ListBundlesPaginatorName,
-    ListProjectsPaginatorName,
-    PlatformType,
-    ProjectStateType,
-    MobileServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_mobile.literals import ListBundlesPaginatorName
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mobile.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Mobile` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/type_defs/).
+
 ```python
-from types_aiobotocore_mobile.type_defs import (
-    BlobTypeDef,
-    BundleDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    ResourceTypeDef,
-    DescribeBundleRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ExportBundleRequestRequestTypeDef,
-    ExportProjectRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeBundleResultTypeDef,
-    ExportBundleResultTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesResultTypeDef,
-    DeleteProjectResultTypeDef,
-    ProjectDetailsTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    CreateProjectResultTypeDef,
-    DescribeProjectResultTypeDef,
-    UpdateProjectResultTypeDef,
-)
+from types_aiobotocore_mobile.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mobile-2.5.2.post1/setup.py` & `types-aiobotocore-mobile-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mobile",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mobile"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__init__.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__init__.pyi` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/__main__.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Mobile 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Mobile 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile\nOther"
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

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/client.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/client.pyi` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/literals.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.pyi`

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
     "ListBundlesPaginatorName",
     "ListProjectsPaginatorName",
     "PlatformType",
     "ProjectStateType",
     "MobileServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListBundlesPaginatorName = Literal["list_bundles"]
 ListProjectsPaginatorName = Literal["list_projects"]
 PlatformType = Literal["ANDROID", "JAVASCRIPT", "LINUX", "OBJC", "OSX", "SWIFT", "WINDOWS"]
 ProjectStateType = Literal["IMPORTING", "NORMAL", "SYNCING"]
 MobileServiceName = Literal["mobile"]
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

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/literals.pyi` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListBundlesPaginatorName",
     "ListProjectsPaginatorName",
     "PlatformType",
     "ProjectStateType",
     "MobileServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ListBundlesPaginatorName = Literal["list_bundles"]
 ListProjectsPaginatorName = Literal["list_projects"]
 PlatformType = Literal["ANDROID", "JAVASCRIPT", "LINUX", "OBJC", "OSX", "SWIFT", "WINDOWS"]
 ProjectStateType = Literal["IMPORTING", "NORMAL", "SYNCING"]
 MobileServiceName = Literal["mobile"]
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

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/paginator.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/paginator.pyi` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/type_defs.py` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile/type_defs.pyi` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/PKG-INFO` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,68 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mobile.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Mobile` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/literals/).
+
 ```python
-from types_aiobotocore_mobile.literals import (
-    ListBundlesPaginatorName,
-    ListProjectsPaginatorName,
-    PlatformType,
-    ProjectStateType,
-    MobileServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_mobile.literals import ListBundlesPaginatorName
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mobile.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Mobile` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/type_defs/).
+
 ```python
-from types_aiobotocore_mobile.type_defs import (
-    BlobTypeDef,
-    BundleDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    ResourceTypeDef,
-    DescribeBundleRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ExportBundleRequestRequestTypeDef,
-    ExportProjectRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeBundleResultTypeDef,
-    ExportBundleResultTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesResultTypeDef,
-    DeleteProjectResultTypeDef,
-    ProjectDetailsTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    CreateProjectResultTypeDef,
-    DescribeProjectResultTypeDef,
-    UpdateProjectResultTypeDef,
-)
+from types_aiobotocore_mobile.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mobile-2.5.2.post1/types_aiobotocore_mobile.egg-info/SOURCES.txt` & `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

