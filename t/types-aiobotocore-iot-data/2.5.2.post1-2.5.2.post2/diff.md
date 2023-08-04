# Comparing `tmp/types-aiobotocore-iot-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-iot-data-2.5.2.post1.tar` & `types-aiobotocore-iot-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:25.269567 types-aiobotocore-iot-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-02 14:52:25.269567 types-aiobotocore-iot-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:25.269567 types-aiobotocore-iot-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:25.261567 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:35.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:25.269567 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:25.000000 types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.216642 types-aiobotocore-iot-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13052 2023-08-04 13:59:11.216642 types-aiobotocore-iot-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11526 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.216642 types-aiobotocore-iot-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2083 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.216642 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      713 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      712 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9467 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9450 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8358 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8356 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2082 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6872 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6861 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:44.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.216642 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13052 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:11.000000 types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/LICENSE` & `types-aiobotocore-iot-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iot-data-2.5.2.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/
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
 [types-aiobotocore-iot-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `IoTDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/literals/).
+
 ```python
-from types_aiobotocore_iot_data.literals import (
-    ListRetainedMessagesPaginatorName,
-    PayloadFormatIndicatorType,
-    IoTDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot_data.literals import ListRetainedMessagesPaginatorName
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_data.type_defs import (
-    BlobTypeDef,
-    DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRetainedMessageRequestRequestTypeDef,
-    GetThingShadowRequestRequestTypeDef,
-    ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRetainedMessagesRequestRequestTypeDef,
-    RetainedMessageSummaryTypeDef,
-    PublishRequestRequestTypeDef,
-    UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
-    UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
-    ListRetainedMessagesResponseTypeDef,
-)
+from types_aiobotocore_iot_data.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/README.md` & `types-aiobotocore-iot-data-2.5.2.post2/README.md`

 * *Files 7% similar despite different names*

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
 [types-aiobotocore-iot-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,59 +259,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `IoTDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/literals/).
+
 ```python
-from types_aiobotocore_iot_data.literals import (
-    ListRetainedMessagesPaginatorName,
-    PayloadFormatIndicatorType,
-    IoTDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot_data.literals import ListRetainedMessagesPaginatorName
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_data.type_defs import (
-    BlobTypeDef,
-    DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRetainedMessageRequestRequestTypeDef,
-    GetThingShadowRequestRequestTypeDef,
-    ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRetainedMessagesRequestRequestTypeDef,
-    RetainedMessageSummaryTypeDef,
-    PublishRequestRequestTypeDef,
-    UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
-    UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
-    ListRetainedMessagesResponseTypeDef,
-)
+from types_aiobotocore_iot_data.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/setup.py` & `types-aiobotocore-iot-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTDataPlane 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__init__.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__init__.pyi` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/__main__.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTDataPlane 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTDataPlane 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane\nOther"
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

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/client.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/client.pyi` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/literals.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListRetainedMessagesPaginatorName",
     "PayloadFormatIndicatorType",
     "IoTDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListRetainedMessagesPaginatorName = Literal["list_retained_messages"]
 PayloadFormatIndicatorType = Literal["UNSPECIFIED_BYTES", "UTF8_DATA"]
 IoTDataPlaneServiceName = Literal["iot-data"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -44,14 +42,15 @@
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
@@ -147,14 +146,15 @@
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
@@ -233,26 +233,28 @@
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

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/literals.pyi` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListRetainedMessagesPaginatorName",
     "PayloadFormatIndicatorType",
     "IoTDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListRetainedMessagesPaginatorName = Literal["list_retained_messages"]
 PayloadFormatIndicatorType = Literal["UNSPECIFIED_BYTES", "UTF8_DATA"]
 IoTDataPlaneServiceName = Literal["iot-data"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -42,14 +44,15 @@
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
@@ -145,14 +148,15 @@
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
@@ -231,26 +235,28 @@
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

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/paginator.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/paginator.pyi` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/type_defs.py` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data/type_defs.pyi` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/PKG-INFO` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/
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
 [types-aiobotocore-iot-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_data.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `IoTDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/literals/).
+
 ```python
-from types_aiobotocore_iot_data.literals import (
-    ListRetainedMessagesPaginatorName,
-    PayloadFormatIndicatorType,
-    IoTDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot_data.literals import ListRetainedMessagesPaginatorName
 
 
 def check_value(value: ListRetainedMessagesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_data.type_defs import (
-    BlobTypeDef,
-    DeleteThingShadowRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRetainedMessageRequestRequestTypeDef,
-    GetThingShadowRequestRequestTypeDef,
-    ListNamedShadowsForThingRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRetainedMessagesRequestRequestTypeDef,
-    RetainedMessageSummaryTypeDef,
-    PublishRequestRequestTypeDef,
-    UpdateThingShadowRequestRequestTypeDef,
-    DeleteThingShadowResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRetainedMessageResponseTypeDef,
-    GetThingShadowResponseTypeDef,
-    ListNamedShadowsForThingResponseTypeDef,
-    UpdateThingShadowResponseTypeDef,
-    ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef,
-    ListRetainedMessagesResponseTypeDef,
-)
+from types_aiobotocore_iot_data.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-data-2.5.2.post1/types_aiobotocore_iot_data.egg-info/SOURCES.txt` & `types-aiobotocore-iot-data-2.5.2.post2/types_aiobotocore_iot_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

