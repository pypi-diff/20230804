# Comparing `tmp/types-aiobotocore-iot-roborunner-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot-roborunner-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1.tar` & `types-aiobotocore-iot-roborunner-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.345564 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13718 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12173 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.146643 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1270 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1269 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20847 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20814 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8309 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8307 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5494 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5488 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20234 2023-08-04 13:40:48.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20195 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13718 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/LICENSE` & `types-aiobotocore-iot-roborunner-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.2.post2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-roborunner type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,93 +269,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_roborunner.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTRoboRunner` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/literals/).
+
 ```python
-from types_aiobotocore_iot_roborunner.literals import (
-    DestinationStateType,
-    ListDestinationsPaginatorName,
-    ListSitesPaginatorName,
-    ListWorkerFleetsPaginatorName,
-    ListWorkersPaginatorName,
-    IoTRoboRunnerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot_roborunner.literals import DestinationStateType
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_roborunner.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTRoboRunner` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/type_defs/).
+
 ```python
-from types_aiobotocore_iot_roborunner.type_defs import (
-    CartesianCoordinatesTypeDef,
-    CreateDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateSiteRequestRequestTypeDef,
-    CreateWorkerFleetRequestRequestTypeDef,
-    OrientationTypeDef,
-    VendorPropertiesTypeDef,
-    DeleteDestinationRequestRequestTypeDef,
-    DeleteSiteRequestRequestTypeDef,
-    DeleteWorkerFleetRequestRequestTypeDef,
-    DeleteWorkerRequestRequestTypeDef,
-    DestinationTypeDef,
-    GetDestinationRequestRequestTypeDef,
-    GetSiteRequestRequestTypeDef,
-    GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestRequestTypeDef,
-    SiteTypeDef,
-    ListWorkerFleetsRequestRequestTypeDef,
-    WorkerFleetTypeDef,
-    ListWorkersRequestRequestTypeDef,
-    UpdateDestinationRequestRequestTypeDef,
-    UpdateSiteRequestRequestTypeDef,
-    UpdateWorkerFleetRequestRequestTypeDef,
-    PositionCoordinatesTypeDef,
-    CreateDestinationResponseTypeDef,
-    CreateSiteResponseTypeDef,
-    CreateWorkerFleetResponseTypeDef,
-    CreateWorkerResponseTypeDef,
-    GetDestinationResponseTypeDef,
-    GetSiteResponseTypeDef,
-    GetWorkerFleetResponseTypeDef,
-    UpdateDestinationResponseTypeDef,
-    UpdateSiteResponseTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
-    ListDestinationsResponseTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
-    ListSitesResponseTypeDef,
-    ListWorkerFleetsResponseTypeDef,
-    CreateWorkerRequestRequestTypeDef,
-    GetWorkerResponseTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
-    UpdateWorkerResponseTypeDef,
-    WorkerTypeDef,
-    ListWorkersResponseTypeDef,
-)
+from types_aiobotocore_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
 
 def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/setup.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-roborunner",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__main__.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoTRoboRunner 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.py`

 * *Files 1% similar despite different names*

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
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.py` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,93 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_roborunner.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTRoboRunner` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/literals/).
+
 ```python
-from types_aiobotocore_iot_roborunner.literals import (
-    DestinationStateType,
-    ListDestinationsPaginatorName,
-    ListSitesPaginatorName,
-    ListWorkerFleetsPaginatorName,
-    ListWorkersPaginatorName,
-    IoTRoboRunnerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot_roborunner.literals import DestinationStateType
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_roborunner.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTRoboRunner` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/type_defs/).
+
 ```python
-from types_aiobotocore_iot_roborunner.type_defs import (
-    CartesianCoordinatesTypeDef,
-    CreateDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateSiteRequestRequestTypeDef,
-    CreateWorkerFleetRequestRequestTypeDef,
-    OrientationTypeDef,
-    VendorPropertiesTypeDef,
-    DeleteDestinationRequestRequestTypeDef,
-    DeleteSiteRequestRequestTypeDef,
-    DeleteWorkerFleetRequestRequestTypeDef,
-    DeleteWorkerRequestRequestTypeDef,
-    DestinationTypeDef,
-    GetDestinationRequestRequestTypeDef,
-    GetSiteRequestRequestTypeDef,
-    GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestRequestTypeDef,
-    SiteTypeDef,
-    ListWorkerFleetsRequestRequestTypeDef,
-    WorkerFleetTypeDef,
-    ListWorkersRequestRequestTypeDef,
-    UpdateDestinationRequestRequestTypeDef,
-    UpdateSiteRequestRequestTypeDef,
-    UpdateWorkerFleetRequestRequestTypeDef,
-    PositionCoordinatesTypeDef,
-    CreateDestinationResponseTypeDef,
-    CreateSiteResponseTypeDef,
-    CreateWorkerFleetResponseTypeDef,
-    CreateWorkerResponseTypeDef,
-    GetDestinationResponseTypeDef,
-    GetSiteResponseTypeDef,
-    GetWorkerFleetResponseTypeDef,
-    UpdateDestinationResponseTypeDef,
-    UpdateSiteResponseTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
-    ListDestinationsResponseTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
-    ListSitesResponseTypeDef,
-    ListWorkerFleetsResponseTypeDef,
-    CreateWorkerRequestRequestTypeDef,
-    GetWorkerResponseTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
-    UpdateWorkerResponseTypeDef,
-    WorkerTypeDef,
-    ListWorkersResponseTypeDef,
-)
+from types_aiobotocore_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
 
 def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt` & `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

