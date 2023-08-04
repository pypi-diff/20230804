# Comparing `tmp/types-aiobotocore-rbin-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rbin-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rbin-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-rbin-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-rbin-2.5.2.post1.tar` & `types-aiobotocore-rbin-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.593489 types-aiobotocore-rbin-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-08-02 14:52:50.589489 types-aiobotocore-rbin-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.593489 types-aiobotocore-rbin-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.585489 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-02 14:47:20.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-02 14:47:20.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:19.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.589489 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:50.000000 types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12768 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11256 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2033 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.216643 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      623 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      622 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      932 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10323 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10303 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8703 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2142 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2139 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9441 2023-08-04 13:49:55.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9430 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.216643 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12768 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rbin-2.5.2.post1/LICENSE` & `types-aiobotocore-rbin-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/PKG-INFO` & `types-aiobotocore-rbin-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rbin
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
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
 [types-aiobotocore-rbin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,70 +287,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rbin.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `RecycleBin` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/literals/).
+
 ```python
-from types_aiobotocore_rbin.literals import (
-    ListRulesPaginatorName,
-    LockStateType,
-    ResourceTypeType,
-    RetentionPeriodUnitType,
-    RuleStatusType,
-    UnlockDelayUnitType,
-    RecycleBinServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rbin.literals import ListRulesPaginatorName
 
 
 def check_value(value: ListRulesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rbin.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RecycleBin` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/type_defs/).
+
 ```python
-from types_aiobotocore_rbin.type_defs import (
-    ResourceTagTypeDef,
-    RetentionPeriodTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteRuleRequestRequestTypeDef,
-    GetRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UnlockDelayTypeDef,
-    UnlockRuleRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ListRulesRequestRequestTypeDef,
-    RuleSummaryTypeDef,
-    UpdateRuleRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRuleResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    LockConfigurationTypeDef,
-    ListRulesResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseTypeDef,
-    GetRuleResponseTypeDef,
-    LockRuleRequestRequestTypeDef,
-    LockRuleResponseTypeDef,
-    UnlockRuleResponseTypeDef,
-)
+from types_aiobotocore_rbin.type_defs import ResourceTagTypeDef
 
 
 def get_value() -> ResourceTagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-rbin-2.5.2.post1/README.md` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-rbin
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore rbin type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-rbin"></a>
 
 # types-aiobotocore-rbin
 
 [![PyPI - types-aiobotocore-rbin](https://img.shields.io/pypi/v/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
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
 [types-aiobotocore-rbin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -255,70 +287,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rbin.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `RecycleBin` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/literals/).
+
 ```python
-from types_aiobotocore_rbin.literals import (
-    ListRulesPaginatorName,
-    LockStateType,
-    ResourceTypeType,
-    RetentionPeriodUnitType,
-    RuleStatusType,
-    UnlockDelayUnitType,
-    RecycleBinServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rbin.literals import ListRulesPaginatorName
 
 
 def check_value(value: ListRulesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rbin.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `RecycleBin` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/type_defs/).
+
 ```python
-from types_aiobotocore_rbin.type_defs import (
-    ResourceTagTypeDef,
-    RetentionPeriodTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteRuleRequestRequestTypeDef,
-    GetRuleRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UnlockDelayTypeDef,
-    UnlockRuleRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ListRulesRequestRequestTypeDef,
-    RuleSummaryTypeDef,
-    UpdateRuleRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateRuleResponseTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    LockConfigurationTypeDef,
-    ListRulesResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
-    CreateRuleResponseTypeDef,
-    GetRuleResponseTypeDef,
-    LockRuleRequestRequestTypeDef,
-    LockRuleResponseTypeDef,
-    UnlockRuleResponseTypeDef,
-)
+from types_aiobotocore_rbin.type_defs import ResourceTagTypeDef
 
 
 def get_value() -> ResourceTagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-rbin-2.5.2.post1/setup.py` & `types-aiobotocore-rbin-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rbin",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__init__.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__init__.pyi` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/__main__.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RecycleBin 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.RecycleBin 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/client.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/client.pyi` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/literals.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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
@@ -422,14 +426,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/literals.pyi` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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
@@ -420,14 +424,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/paginator.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/paginator.pyi` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/type_defs.py` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin/type_defs.pyi` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post1/types_aiobotocore_rbin.egg-info/SOURCES.txt` & `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

