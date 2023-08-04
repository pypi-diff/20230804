# Comparing `tmp/types-aiobotocore-iot1click-devices-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot1click-devices-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-devices-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-devices-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1.tar` & `types-aiobotocore-iot1click-devices-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.353569 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.226642 types-aiobotocore-iot1click-devices-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13779 2023-08-04 13:59:11.226642 types-aiobotocore-iot1click-devices-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12215 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.226642 types-aiobotocore-iot1click-devices-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2148 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.226642 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      954 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      953 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      995 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14000 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13976 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7985 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7983 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3425 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3421 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9779 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9768 2023-08-04 13:40:50.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:49.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.226642 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13779 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1003 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       36 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/LICENSE` & `types-aiobotocore-iot1click-devices-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-devices
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,71 +295,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_devices.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickDevicesService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/literals/).
+
 ```python
-from types_aiobotocore_iot1click_devices.literals import (
-    ListDeviceEventsPaginatorName,
-    ListDevicesPaginatorName,
-    IoT1ClickDevicesServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_iot1click_devices.literals import ListDeviceEventsPaginatorName
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickDevicesService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeDeviceRequestRequestTypeDef,
-    DeviceDescriptionTypeDef,
-    DeviceTypeDef,
-    DeviceMethodTypeDef,
-    FinalizeDeviceClaimRequestRequestTypeDef,
-    GetDeviceMethodsRequestRequestTypeDef,
-    InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListDevicesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnclaimDeviceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    DeviceEventTypeDef,
-    GetDeviceMethodsResponseTypeDef,
-    InvokeDeviceMethodRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/README.md` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-iot1click-devices
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,71 +295,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_devices.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickDevicesService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/literals/).
+
 ```python
-from types_aiobotocore_iot1click_devices.literals import (
-    ListDeviceEventsPaginatorName,
-    ListDevicesPaginatorName,
-    IoT1ClickDevicesServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_iot1click_devices.literals import ListDeviceEventsPaginatorName
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickDevicesService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeDeviceRequestRequestTypeDef,
-    DeviceDescriptionTypeDef,
-    DeviceTypeDef,
-    DeviceMethodTypeDef,
-    FinalizeDeviceClaimRequestRequestTypeDef,
-    GetDeviceMethodsRequestRequestTypeDef,
-    InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListDevicesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnclaimDeviceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    DeviceEventTypeDef,
-    GetDeviceMethodsResponseTypeDef,
-    InvokeDeviceMethodRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/setup.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-devices",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__main__.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService\nOther"
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

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
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
@@ -144,14 +145,15 @@
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
@@ -230,26 +232,28 @@
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

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.py` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.5.2.post2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iot1click-devices
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,71 +263,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_devices.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickDevicesService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/literals/).
+
 ```python
-from types_aiobotocore_iot1click_devices.literals import (
-    ListDeviceEventsPaginatorName,
-    ListDevicesPaginatorName,
-    IoT1ClickDevicesServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_iot1click_devices.literals import ListDeviceEventsPaginatorName
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickDevicesService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeDeviceRequestRequestTypeDef,
-    DeviceDescriptionTypeDef,
-    DeviceTypeDef,
-    DeviceMethodTypeDef,
-    FinalizeDeviceClaimRequestRequestTypeDef,
-    GetDeviceMethodsRequestRequestTypeDef,
-    InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListDevicesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnclaimDeviceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
-    DescribeDeviceResponseTypeDef,
-    ListDevicesResponseTypeDef,
-    DeviceEventTypeDef,
-    GetDeviceMethodsResponseTypeDef,
-    InvokeDeviceMethodRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-devices-2.5.2.post2/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

