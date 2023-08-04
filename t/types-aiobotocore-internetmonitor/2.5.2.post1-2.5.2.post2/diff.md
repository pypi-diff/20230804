# Comparing `tmp/types-aiobotocore-internetmonitor-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-internetmonitor-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-internetmonitor-2.5.2.post1.tar` & `types-aiobotocore-internetmonitor-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.337569 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13664 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12104 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2138 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      964 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      995 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12756 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12735 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9375 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9373 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3519 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3515 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13136 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13664 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/LICENSE` & `types-aiobotocore-internetmonitor-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,79 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_internetmonitor.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudWatchInternetMonitor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/literals/).
+
 ```python
-from types_aiobotocore_internetmonitor.literals import (
-    HealthEventImpactTypeType,
-    HealthEventStatusType,
-    ListHealthEventsPaginatorName,
-    ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
-    MonitorConfigStateType,
-    MonitorProcessingStatusCodeType,
-    TriangulationEventTypeType,
-    CloudWatchInternetMonitorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_internetmonitor.literals import HealthEventImpactTypeType
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchInternetMonitor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/type_defs/).
+
 ```python
-from types_aiobotocore_internetmonitor.type_defs import (
-    AvailabilityMeasurementTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteMonitorInputRequestTypeDef,
-    GetHealthEventInputRequestTypeDef,
-    GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListMonitorsInputRequestTypeDef,
-    MonitorTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    NetworkTypeDef,
-    RoundTripTimeTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateMonitorOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsOutputTypeDef,
-    NetworkImpairmentTypeDef,
-    PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
-    InternetHealthTypeDef,
-    ImpactedLocationTypeDef,
-    GetHealthEventOutputTypeDef,
-    HealthEventTypeDef,
-    ListHealthEventsOutputTypeDef,
-)
+from types_aiobotocore_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
 
 def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/README.md` & `types-aiobotocore-internetmonitor-2.5.2.post2/README.md`

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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,79 +263,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_internetmonitor.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudWatchInternetMonitor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/literals/).
+
 ```python
-from types_aiobotocore_internetmonitor.literals import (
-    HealthEventImpactTypeType,
-    HealthEventStatusType,
-    ListHealthEventsPaginatorName,
-    ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
-    MonitorConfigStateType,
-    MonitorProcessingStatusCodeType,
-    TriangulationEventTypeType,
-    CloudWatchInternetMonitorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_internetmonitor.literals import HealthEventImpactTypeType
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchInternetMonitor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/type_defs/).
+
 ```python
-from types_aiobotocore_internetmonitor.type_defs import (
-    AvailabilityMeasurementTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteMonitorInputRequestTypeDef,
-    GetHealthEventInputRequestTypeDef,
-    GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListMonitorsInputRequestTypeDef,
-    MonitorTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    NetworkTypeDef,
-    RoundTripTimeTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateMonitorOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsOutputTypeDef,
-    NetworkImpairmentTypeDef,
-    PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
-    InternetHealthTypeDef,
-    ImpactedLocationTypeDef,
-    GetHealthEventOutputTypeDef,
-    HealthEventTypeDef,
-    ListHealthEventsOutputTypeDef,
-)
+from types_aiobotocore_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
 
 def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/setup.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-internetmonitor",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__main__.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
+    HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
@@ -104,15 +105,16 @@
         *,
         MonitorName: str,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        TrafficPercentageToMonitor: int = ...,
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#create_monitor)
         """
@@ -217,15 +219,16 @@
         MonitorName: str,
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        TrafficPercentageToMonitor: int = ...,
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#update_monitor)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
+    HealthEventsConfigTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
@@ -97,15 +98,16 @@
         *,
         MonitorName: str,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        TrafficPercentageToMonitor: int = ...,
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#create_monitor)
         """
@@ -200,15 +202,16 @@
         MonitorName: str,
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
         MaxCityNetworksToMonitor: int = ...,
         InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        TrafficPercentageToMonitor: int = ...,
+        HealthEventsConfig: HealthEventsConfigTypeDef = ...
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#update_monitor)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,34 @@
 
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
+    "LocalHealthEventsConfigStatusType",
     "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
-HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
+HealthEventImpactTypeType = Literal[
+    "AVAILABILITY", "LOCAL_AVAILABILITY", "LOCAL_PERFORMANCE", "PERFORMANCE"
+]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
+LocalHealthEventsConfigStatusType = Literal["DISABLED", "ENABLED"]
 LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
@@ -63,14 +67,15 @@
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
@@ -166,14 +171,15 @@
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
@@ -252,26 +258,28 @@
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
@@ -417,24 +425,32 @@
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,33 @@
     from typing_extensions import Literal
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
+    "LocalHealthEventsConfigStatusType",
     "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
+HealthEventImpactTypeType = Literal[
+    "AVAILABILITY", "LOCAL_AVAILABILITY", "LOCAL_PERFORMANCE", "PERFORMANCE"
+]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
+LocalHealthEventsConfigStatusType = Literal["DISABLED", "ENABLED"]
 LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
@@ -61,14 +65,15 @@
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
@@ -164,14 +169,15 @@
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
@@ -250,26 +256,28 @@
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
@@ -415,24 +423,32 @@
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.py` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
@@ -32,27 +33,29 @@
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "LocalHealthEventsConfigTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "HealthEventsConfigTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
@@ -105,14 +108,24 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+LocalHealthEventsConfigTypeDef = TypedDict(
+    "LocalHealthEventsConfigTypeDef",
+    {
+        "Status": LocalHealthEventsConfigStatusType,
+        "HealthScoreThreshold": float,
+        "MinTrafficImpact": float,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -224,14 +237,25 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+HealthEventsConfigTypeDef = TypedDict(
+    "HealthEventsConfigTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+        "AvailabilityLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+        "PerformanceLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
@@ -335,14 +359,15 @@
     {
         "Resources": Sequence[str],
         "ClientToken": str,
         "Tags": Mapping[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
@@ -361,14 +386,15 @@
         "ModifiedAt": datetime,
         "ProcessingStatus": MonitorProcessingStatusCodeType,
         "ProcessingStatusInfo": str,
         "Tags": Dict[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
@@ -381,14 +407,15 @@
         "ResourcesToAdd": Sequence[str],
         "ResourcesToRemove": Sequence[str],
         "Status": MonitorConfigStateType,
         "ClientToken": str,
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
@@ -445,14 +472,15 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
+        "HealthScoreThreshold": float,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
@@ -467,14 +495,15 @@
 )
 _OptionalHealthEventTypeDef = TypedDict(
     "_OptionalHealthEventTypeDef",
     {
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
+        "HealthScoreThreshold": float,
     },
     total=False,
 )
 
 
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
+    LocalHealthEventsConfigStatusType,
     LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
@@ -31,27 +32,29 @@
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
+    "LocalHealthEventsConfigTypeDef",
     "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
+    "HealthEventsConfigTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
@@ -104,14 +107,24 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
+LocalHealthEventsConfigTypeDef = TypedDict(
+    "LocalHealthEventsConfigTypeDef",
+    {
+        "Status": LocalHealthEventsConfigStatusType,
+        "HealthScoreThreshold": float,
+        "MinTrafficImpact": float,
+    },
+    total=False,
+)
+
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
@@ -221,14 +234,25 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+HealthEventsConfigTypeDef = TypedDict(
+    "HealthEventsConfigTypeDef",
+    {
+        "AvailabilityScoreThreshold": float,
+        "PerformanceScoreThreshold": float,
+        "AvailabilityLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+        "PerformanceLocalHealthEventsConfig": LocalHealthEventsConfigTypeDef,
+    },
+    total=False,
+)
+
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
@@ -328,14 +352,15 @@
     {
         "Resources": Sequence[str],
         "ClientToken": str,
         "Tags": Mapping[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
@@ -352,14 +377,15 @@
         "ModifiedAt": datetime,
         "ProcessingStatus": MonitorProcessingStatusCodeType,
         "ProcessingStatusInfo": str,
         "Tags": Dict[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
@@ -372,14 +398,15 @@
         "ResourcesToAdd": Sequence[str],
         "ResourcesToRemove": Sequence[str],
         "Status": MonitorConfigStateType,
         "ClientToken": str,
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
 ):
@@ -432,14 +459,15 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
+        "HealthScoreThreshold": float,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
@@ -454,14 +482,15 @@
 )
 _OptionalHealthEventTypeDef = TypedDict(
     "_OptionalHealthEventTypeDef",
     {
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
+        "HealthScoreThreshold": float,
     },
     total=False,
 )
 
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,79 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_internetmonitor.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudWatchInternetMonitor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/literals/).
+
 ```python
-from types_aiobotocore_internetmonitor.literals import (
-    HealthEventImpactTypeType,
-    HealthEventStatusType,
-    ListHealthEventsPaginatorName,
-    ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
-    MonitorConfigStateType,
-    MonitorProcessingStatusCodeType,
-    TriangulationEventTypeType,
-    CloudWatchInternetMonitorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_internetmonitor.literals import HealthEventImpactTypeType
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudWatchInternetMonitor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/type_defs/).
+
 ```python
-from types_aiobotocore_internetmonitor.type_defs import (
-    AvailabilityMeasurementTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteMonitorInputRequestTypeDef,
-    GetHealthEventInputRequestTypeDef,
-    GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListMonitorsInputRequestTypeDef,
-    MonitorTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    NetworkTypeDef,
-    RoundTripTimeTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateMonitorOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsOutputTypeDef,
-    NetworkImpairmentTypeDef,
-    PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
-    InternetHealthTypeDef,
-    ImpactedLocationTypeDef,
-    GetHealthEventOutputTypeDef,
-    HealthEventTypeDef,
-    ListHealthEventsOutputTypeDef,
-)
+from types_aiobotocore_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
 
 def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt` & `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

