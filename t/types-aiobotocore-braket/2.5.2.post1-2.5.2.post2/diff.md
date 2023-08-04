# Comparing `tmp/types-aiobotocore-braket-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-braket-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-braket-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-braket-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:30 2023, max compression
```

## Comparing `types-aiobotocore-braket-2.5.2.post1.tar` & `types-aiobotocore-braket-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:51.000000 types-aiobotocore-braket-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.505643 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-08-02 14:33:53.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:52.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:57.000000 types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.907323 types-aiobotocore-braket-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-08-04 12:00:30.899323 types-aiobotocore-braket-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:30.907323 types-aiobotocore-braket-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.895323 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-04 11:41:05.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:04.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.899323 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:30.000000 types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-braket-2.5.2.post1/LICENSE` & `types-aiobotocore-braket-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/README.md` & `types-aiobotocore-braket-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-braket
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore braket type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,98 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_braket.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Braket` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/literals/).
+
 ```python
-from types_aiobotocore_braket.literals import (
-    CancellationStatusType,
-    CompressionTypeType,
-    DeviceStatusType,
-    DeviceTypeType,
-    InstanceTypeType,
-    JobEventTypeType,
-    JobPrimaryStatusType,
-    QuantumTaskStatusType,
-    SearchDevicesPaginatorName,
-    SearchJobsFilterOperatorType,
-    SearchJobsPaginatorName,
-    SearchQuantumTasksFilterOperatorType,
-    SearchQuantumTasksPaginatorName,
-    BraketServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_braket.literals import CancellationStatusType
 
 
 def check_value(value: CancellationStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_braket.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Braket` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/type_defs/).
+
 ```python
-from types_aiobotocore_braket.type_defs import (
-    ContainerImageTypeDef,
-    ScriptModeConfigTypeDef,
-    CancelJobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CancelQuantumTaskRequestRequestTypeDef,
-    DeviceConfigTypeDef,
-    InstanceConfigTypeDef,
-    JobCheckpointConfigTypeDef,
-    JobOutputDataConfigTypeDef,
-    JobStoppingConditionTypeDef,
-    CreateQuantumTaskRequestRequestTypeDef,
-    S3DataSourceTypeDef,
-    DeviceSummaryTypeDef,
-    GetDeviceRequestRequestTypeDef,
-    GetJobRequestRequestTypeDef,
-    JobEventDetailsTypeDef,
-    GetQuantumTaskRequestRequestTypeDef,
-    JobSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QuantumTaskSummaryTypeDef,
-    SearchDevicesFilterTypeDef,
-    SearchJobsFilterTypeDef,
-    SearchQuantumTasksFilterTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AlgorithmSpecificationTypeDef,
-    CancelJobResponseTypeDef,
-    CancelQuantumTaskResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetQuantumTaskResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DataSourceTypeDef,
-    SearchDevicesResponseTypeDef,
-    SearchJobsResponseTypeDef,
-    SearchQuantumTasksResponseTypeDef,
-    SearchDevicesRequestRequestTypeDef,
-    SearchDevicesRequestSearchDevicesPaginateTypeDef,
-    SearchJobsRequestRequestTypeDef,
-    SearchJobsRequestSearchJobsPaginateTypeDef,
-    SearchQuantumTasksRequestRequestTypeDef,
-    SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
-    InputFileConfigTypeDef,
-    CreateJobRequestRequestTypeDef,
-    GetJobResponseTypeDef,
-)
+from types_aiobotocore_braket.type_defs import ContainerImageTypeDef
 
 
 def get_value() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-braket-2.5.2.post1/setup.py` & `types-aiobotocore-braket-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-braket",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__init__.pyi` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/__main__.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Braket 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Braket 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/client.pyi` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/literals.pyi` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/paginator.pyi` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.py` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket/type_defs.pyi` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post1/types_aiobotocore_braket.egg-info/SOURCES.txt` & `types-aiobotocore-braket-2.5.2.post2/types_aiobotocore_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

