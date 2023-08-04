# Comparing `tmp/types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-arc-zonal-shift-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.985653 types-aiobotocore-arc-zonal-shift-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.985653 types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-02 14:33:30.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-02 14:33:30.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.647120 types-aiobotocore-arc-zonal-shift-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-08-04 12:00:25.647120 types-aiobotocore-arc-zonal-shift-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.647120 types-aiobotocore-arc-zonal-shift-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.635119 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-04 11:40:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-04 11:40:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 11:40:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-04 11:40:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-04 11:40:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-04 11:40:40.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 11:40:40.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:38.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.647120 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:00:25.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/LICENSE` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,59 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_arc_zonal_shift.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ARCZonalShift` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/literals/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.literals import (
-    AppliedStatusType,
-    ListManagedResourcesPaginatorName,
-    ListZonalShiftsPaginatorName,
-    ZonalShiftStatusType,
-    ARCZonalShiftServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_arc_zonal_shift.literals import AppliedStatusType
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ARCZonalShift` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/type_defs/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.type_defs import (
-    CancelZonalShiftRequestRequestTypeDef,
-    GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListManagedResourcesRequestRequestTypeDef,
-    ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestRequestTypeDef,
-    ZonalShiftSummaryTypeDef,
-    StartZonalShiftRequestRequestTypeDef,
-    UpdateZonalShiftRequestRequestTypeDef,
-    ZonalShiftTypeDef,
-    GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
-    ListManagedResourcesResponseTypeDef,
-    ListZonalShiftsResponseTypeDef,
-)
+from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
 
 def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/README.md` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/README.md`

 * *Files 10% similar despite different names*

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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,59 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_arc_zonal_shift.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ARCZonalShift` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/literals/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.literals import (
-    AppliedStatusType,
-    ListManagedResourcesPaginatorName,
-    ListZonalShiftsPaginatorName,
-    ZonalShiftStatusType,
-    ARCZonalShiftServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_arc_zonal_shift.literals import AppliedStatusType
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ARCZonalShift` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/type_defs/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.type_defs import (
-    CancelZonalShiftRequestRequestTypeDef,
-    GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListManagedResourcesRequestRequestTypeDef,
-    ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestRequestTypeDef,
-    ZonalShiftSummaryTypeDef,
-    StartZonalShiftRequestRequestTypeDef,
-    UpdateZonalShiftRequestRequestTypeDef,
-    ZonalShiftTypeDef,
-    GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
-    ListManagedResourcesResponseTypeDef,
-    ListZonalShiftsResponseTypeDef,
-)
+from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
 
 def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-arc-zonal-shift",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__main__.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ARCZonalShift 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,59 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_arc_zonal_shift.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ARCZonalShift` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/literals/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.literals import (
-    AppliedStatusType,
-    ListManagedResourcesPaginatorName,
-    ListZonalShiftsPaginatorName,
-    ZonalShiftStatusType,
-    ARCZonalShiftServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_arc_zonal_shift.literals import AppliedStatusType
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ARCZonalShift` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/type_defs/).
+
 ```python
-from types_aiobotocore_arc_zonal_shift.type_defs import (
-    CancelZonalShiftRequestRequestTypeDef,
-    GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListManagedResourcesRequestRequestTypeDef,
-    ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestRequestTypeDef,
-    ZonalShiftSummaryTypeDef,
-    StartZonalShiftRequestRequestTypeDef,
-    UpdateZonalShiftRequestRequestTypeDef,
-    ZonalShiftTypeDef,
-    GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
-    ListManagedResourcesResponseTypeDef,
-    ListZonalShiftsResponseTypeDef,
-)
+from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
 
 def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt` & `types-aiobotocore-arc-zonal-shift-2.5.2.post2/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

