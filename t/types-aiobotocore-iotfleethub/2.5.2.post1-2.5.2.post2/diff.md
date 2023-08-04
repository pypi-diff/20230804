# Comparing `tmp/types-aiobotocore-iotfleethub-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotfleethub-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleethub-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleethub-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotfleethub-2.5.2.post1.tar` & `types-aiobotocore-iotfleethub-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.645563 types-aiobotocore-iotfleethub-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-08-02 14:52:26.645563 types-aiobotocore-iotfleethub-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.645563 types-aiobotocore-iotfleethub-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.637563 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:49.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.645563 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.286642 types-aiobotocore-iotfleethub-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13169 2023-08-04 13:59:12.286642 types-aiobotocore-iotfleethub-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11635 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.286642 types-aiobotocore-iotfleethub-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.276642 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      691 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      690 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9569 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9551 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8224 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8222 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2055 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2052 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6165 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6156 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:04.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.286642 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13169 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/LICENSE` & `types-aiobotocore-iotfleethub-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iotfleethub-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleethub
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTFleetHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTFleetHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/
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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,56 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotfleethub.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTFleetHub` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/literals/).
+
 ```python
-from types_aiobotocore_iotfleethub.literals import (
-    ApplicationStateType,
-    ListApplicationsPaginatorName,
-    IoTFleetHubServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iotfleethub.literals import ApplicationStateType
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTFleetHub` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/type_defs/).
+
 ```python
-from types_aiobotocore_iotfleethub.type_defs import (
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DescribeApplicationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-)
+from types_aiobotocore_iotfleethub.type_defs import ApplicationSummaryTypeDef
 
 
 def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/README.md` & `types-aiobotocore-iotfleethub-2.5.2.post2/README.md`

 * *Files 15% similar despite different names*

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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,56 +259,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotfleethub.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTFleetHub` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/literals/).
+
 ```python
-from types_aiobotocore_iotfleethub.literals import (
-    ApplicationStateType,
-    ListApplicationsPaginatorName,
-    IoTFleetHubServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iotfleethub.literals import ApplicationStateType
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTFleetHub` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/type_defs/).
+
 ```python
-from types_aiobotocore_iotfleethub.type_defs import (
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DescribeApplicationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-)
+from types_aiobotocore_iotfleethub.type_defs import ApplicationSummaryTypeDef
 
 
 def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/setup.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleethub",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotfleethub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTFleetHub 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__init__.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__init__.pyi` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/__main__.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetHub 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTFleetHub 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\nOther"
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

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/client.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/client.pyi` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/literals.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -233,26 +235,28 @@
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

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/literals.pyi` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -231,26 +233,28 @@
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

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/paginator.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/paginator.pyi` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/type_defs.py` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub/type_defs.pyi` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/PKG-INFO` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleethub
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTFleetHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTFleetHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/
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
 [types-aiobotocore-iotfleethub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,56 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotfleethub.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTFleetHub` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/literals/).
+
 ```python
-from types_aiobotocore_iotfleethub.literals import (
-    ApplicationStateType,
-    ListApplicationsPaginatorName,
-    IoTFleetHubServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iotfleethub.literals import ApplicationStateType
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTFleetHub` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleethub/type_defs/).
+
 ```python
-from types_aiobotocore_iotfleethub.type_defs import (
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DescribeApplicationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-)
+from types_aiobotocore_iotfleethub.type_defs import ApplicationSummaryTypeDef
 
 
 def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotfleethub-2.5.2.post1/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleethub-2.5.2.post2/types_aiobotocore_iotfleethub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

