# Comparing `tmp/types-aiobotocore-controltower-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-controltower-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-controltower-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-controltower-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
```

## Comparing `types-aiobotocore-controltower-2.5.2.post1.tar` & `types-aiobotocore-controltower-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.357613 types-aiobotocore-controltower-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 14:52:07.345613 types-aiobotocore-controltower-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.357613 types-aiobotocore-controltower-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:55.000000 types-aiobotocore-controltower-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.345613 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.103750 types-aiobotocore-controltower-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-08-04 12:00:42.103750 types-aiobotocore-controltower-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.103750 types-aiobotocore-controltower-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.091749 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-04 11:43:16.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-04 11:43:16.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-08-04 11:43:16.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-04 11:43:16.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:15.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.103750 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:41.000000 types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-controltower-2.5.2.post1/LICENSE` & `types-aiobotocore-controltower-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/PKG-INFO` & `types-aiobotocore-controltower-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,54 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_controltower.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ControlTower` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/literals/).
+
 ```python
-from types_aiobotocore_controltower.literals import (
-    ControlOperationStatusType,
-    ControlOperationTypeType,
-    ListEnabledControlsPaginatorName,
-    ControlTowerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_controltower.literals import ControlOperationStatusType
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ControlTower` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/type_defs/).
+
 ```python
-from types_aiobotocore_controltower.type_defs import (
-    ControlOperationTypeDef,
-    DisableControlInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableControlInputRequestTypeDef,
-    EnabledControlSummaryTypeDef,
-    GetControlOperationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
-    DisableControlOutputTypeDef,
-    EnableControlOutputTypeDef,
-    GetControlOperationOutputTypeDef,
-    ListEnabledControlsOutputTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-)
+from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef
 
 
 def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-controltower-2.5.2.post1/README.md` & `types-aiobotocore-controltower-2.5.2.post2/README.md`

 * *Files 12% similar despite different names*

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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,54 +259,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_controltower.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ControlTower` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/literals/).
+
 ```python
-from types_aiobotocore_controltower.literals import (
-    ControlOperationStatusType,
-    ControlOperationTypeType,
-    ListEnabledControlsPaginatorName,
-    ControlTowerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_controltower.literals import ControlOperationStatusType
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ControlTower` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/type_defs/).
+
 ```python
-from types_aiobotocore_controltower.type_defs import (
-    ControlOperationTypeDef,
-    DisableControlInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableControlInputRequestTypeDef,
-    EnabledControlSummaryTypeDef,
-    GetControlOperationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
-    DisableControlOutputTypeDef,
-    EnableControlOutputTypeDef,
-    GetControlOperationOutputTypeDef,
-    ListEnabledControlsOutputTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-)
+from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef
 
 
 def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-controltower-2.5.2.post1/setup.py` & `types-aiobotocore-controltower-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-controltower",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_controltower"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ControlTower 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.pyi` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__main__.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ControlTower 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ControlTower 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower\nOther"
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

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.pyi` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.pyi` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.pyi` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.py` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.pyi` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/PKG-INFO` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,54 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_controltower.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ControlTower` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/literals/).
+
 ```python
-from types_aiobotocore_controltower.literals import (
-    ControlOperationStatusType,
-    ControlOperationTypeType,
-    ListEnabledControlsPaginatorName,
-    ControlTowerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_controltower.literals import ControlOperationStatusType
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ControlTower` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/type_defs/).
+
 ```python
-from types_aiobotocore_controltower.type_defs import (
-    ControlOperationTypeDef,
-    DisableControlInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    EnableControlInputRequestTypeDef,
-    EnabledControlSummaryTypeDef,
-    GetControlOperationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
-    DisableControlOutputTypeDef,
-    EnableControlOutputTypeDef,
-    GetControlOperationOutputTypeDef,
-    ListEnabledControlsOutputTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-)
+from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef
 
 
 def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/SOURCES.txt` & `types-aiobotocore-controltower-2.5.2.post2/types_aiobotocore_controltower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

