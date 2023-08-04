# Comparing `tmp/types-aiobotocore-mwaa-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mwaa-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mwaa-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-mwaa-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-mwaa-2.5.2.post1.tar` & `types-aiobotocore-mwaa-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.001513 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-08-02 14:43:52.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-mwaa-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12776 2023-08-04 13:59:19.306643 types-aiobotocore-mwaa-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11270 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.306643 types-aiobotocore-mwaa-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2027 2023-08-04 13:45:22.000000 types-aiobotocore-mwaa-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      635 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      634 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      920 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12292 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12271 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9160 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9158 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1960 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1957 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11700 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11693 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:23.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12776 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:19.000000 types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/LICENSE` & `types-aiobotocore-mwaa-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/PKG-INFO` & `types-aiobotocore-mwaa-2.5.2.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,80 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mwaa.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MWAA` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/literals/).
+
 ```python
-from types_aiobotocore_mwaa.literals import (
-    EnvironmentStatusType,
-    ListEnvironmentsPaginatorName,
-    LoggingLevelType,
-    UnitType,
-    UpdateStatusType,
-    WebserverAccessModeType,
-    MWAAServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mwaa.literals import EnvironmentStatusType
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MWAA` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/type_defs/).
+
 ```python
-from types_aiobotocore_mwaa.type_defs import (
-    CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateWebLoginTokenRequestRequestTypeDef,
-    DeleteEnvironmentInputRequestTypeDef,
-    DimensionTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    GetEnvironmentInputRequestTypeDef,
-    UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnvironmentsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ModuleLoggingConfigurationInputTypeDef,
-    ModuleLoggingConfigurationTypeDef,
-    StatisticSetTypeDef,
-    TimestampTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    NetworkConfigurationUnionTypeDef,
-    LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    LoggingConfigurationInputTypeDef,
-    LoggingConfigurationTypeDef,
-    MetricDatumTypeDef,
-    CreateEnvironmentInputRequestTypeDef,
-    UpdateEnvironmentInputRequestTypeDef,
-    EnvironmentTypeDef,
-    PublishMetricsInputRequestTypeDef,
-    GetEnvironmentOutputTypeDef,
-)
+from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/README.md` & `types-aiobotocore-mwaa-2.5.2.post2/README.md`

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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,80 +257,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mwaa.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MWAA` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/literals/).
+
 ```python
-from types_aiobotocore_mwaa.literals import (
-    EnvironmentStatusType,
-    ListEnvironmentsPaginatorName,
-    LoggingLevelType,
-    UnitType,
-    UpdateStatusType,
-    WebserverAccessModeType,
-    MWAAServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mwaa.literals import EnvironmentStatusType
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MWAA` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/type_defs/).
+
 ```python
-from types_aiobotocore_mwaa.type_defs import (
-    CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateWebLoginTokenRequestRequestTypeDef,
-    DeleteEnvironmentInputRequestTypeDef,
-    DimensionTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    GetEnvironmentInputRequestTypeDef,
-    UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnvironmentsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ModuleLoggingConfigurationInputTypeDef,
-    ModuleLoggingConfigurationTypeDef,
-    StatisticSetTypeDef,
-    TimestampTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    NetworkConfigurationUnionTypeDef,
-    LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    LoggingConfigurationInputTypeDef,
-    LoggingConfigurationTypeDef,
-    MetricDatumTypeDef,
-    CreateEnvironmentInputRequestTypeDef,
-    UpdateEnvironmentInputRequestTypeDef,
-    EnvironmentTypeDef,
-    PublishMetricsInputRequestTypeDef,
-    GetEnvironmentOutputTypeDef,
-)
+from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/setup.py` & `types-aiobotocore-mwaa-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mwaa",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.pyi` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__main__.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MWAA 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MWAA 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -104,15 +104,15 @@
 
     async def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
+        NetworkConfiguration: NetworkConfigurationTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.pyi` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -96,15 +96,15 @@
         """
     async def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
+        NetworkConfiguration: NetworkConfigurationTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
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
@@ -194,14 +195,15 @@
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
@@ -280,26 +282,28 @@
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

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.pyi` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
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
@@ -192,14 +193,15 @@
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
@@ -278,26 +280,28 @@
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

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.pyi` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.py` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,21 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
     "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
@@ -51,15 +49,14 @@
     "UpdateNetworkConfigurationInputTypeDef",
     "CreateCliTokenResponseTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenResponseTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
-    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
@@ -113,23 +110,14 @@
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-    },
-    total=False,
-)
-
 GetEnvironmentInputRequestTypeDef = TypedDict(
     "GetEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -268,17 +256,14 @@
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
@@ -332,19 +317,17 @@
         "StatisticValues": StatisticSetTypeDef,
         "Unit": UnitType,
         "Value": float,
     },
     total=False,
 )
 
-
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
-
 _RequiredCreateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentInputRequestTypeDef",
     {
         "DagS3Path": str,
         "ExecutionRoleArn": str,
         "Name": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
@@ -371,21 +354,19 @@
         "Tags": Mapping[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
-
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEnvironmentInputRequestTypeDef = TypedDict(
@@ -410,21 +391,19 @@
         "StartupScriptS3Path": str,
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "AirflowConfigurationOptions": Dict[str, str],
         "AirflowVersion": str,
         "Arn": str,
         "CreatedAt": datetime,
@@ -433,15 +412,15 @@
         "ExecutionRoleArn": str,
         "KmsKey": str,
         "LastUpdate": LastUpdateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaxWorkers": int,
         "MinWorkers": int,
         "Name": str,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.pyi` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
     "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
@@ -50,15 +50,14 @@
     "UpdateNetworkConfigurationInputTypeDef",
     "CreateCliTokenResponseTypeDef",
     "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenResponseTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
-    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
@@ -112,23 +111,14 @@
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-    },
-    total=False,
-)
-
 GetEnvironmentInputRequestTypeDef = TypedDict(
     "GetEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -267,17 +257,14 @@
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
@@ -331,17 +318,19 @@
         "StatisticValues": StatisticSetTypeDef,
         "Unit": UnitType,
         "Value": float,
     },
     total=False,
 )
 
+
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
+
 _RequiredCreateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentInputRequestTypeDef",
     {
         "DagS3Path": str,
         "ExecutionRoleArn": str,
         "Name": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
@@ -368,19 +357,21 @@
         "Tags": Mapping[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
+
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEnvironmentInputRequestTypeDef = TypedDict(
@@ -405,19 +396,21 @@
         "StartupScriptS3Path": str,
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "AirflowConfigurationOptions": Dict[str, str],
         "AirflowVersion": str,
         "Arn": str,
         "CreatedAt": datetime,
@@ -426,15 +419,15 @@
         "ExecutionRoleArn": str,
         "KmsKey": str,
         "LastUpdate": LastUpdateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaxWorkers": int,
         "MinWorkers": int,
         "Name": str,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/PKG-INFO` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,80 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_mwaa.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `MWAA` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/literals/).
+
 ```python
-from types_aiobotocore_mwaa.literals import (
-    EnvironmentStatusType,
-    ListEnvironmentsPaginatorName,
-    LoggingLevelType,
-    UnitType,
-    UpdateStatusType,
-    WebserverAccessModeType,
-    MWAAServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_mwaa.literals import EnvironmentStatusType
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `MWAA` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/type_defs/).
+
 ```python
-from types_aiobotocore_mwaa.type_defs import (
-    CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    NetworkConfigurationTypeDef,
-    CreateWebLoginTokenRequestRequestTypeDef,
-    DeleteEnvironmentInputRequestTypeDef,
-    DimensionTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    GetEnvironmentInputRequestTypeDef,
-    UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ListEnvironmentsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ModuleLoggingConfigurationInputTypeDef,
-    ModuleLoggingConfigurationTypeDef,
-    StatisticSetTypeDef,
-    TimestampTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateEnvironmentOutputTypeDef,
-    NetworkConfigurationUnionTypeDef,
-    LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
-    LoggingConfigurationInputTypeDef,
-    LoggingConfigurationTypeDef,
-    MetricDatumTypeDef,
-    CreateEnvironmentInputRequestTypeDef,
-    UpdateEnvironmentInputRequestTypeDef,
-    EnvironmentTypeDef,
-    PublishMetricsInputRequestTypeDef,
-    GetEnvironmentOutputTypeDef,
-)
+from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/SOURCES.txt` & `types-aiobotocore-mwaa-2.5.2.post2/types_aiobotocore_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

