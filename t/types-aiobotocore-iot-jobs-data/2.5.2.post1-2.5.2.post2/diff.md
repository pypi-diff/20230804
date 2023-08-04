# Comparing `tmp/types-aiobotocore-iot-jobs-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot-jobs-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-jobs-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-jobs-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1.tar` & `types-aiobotocore-iot-jobs-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.121564 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:36.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.125564 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:25.000000 types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.166643 types-aiobotocore-iot-jobs-data-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12581 2023-08-04 13:59:12.166643 types-aiobotocore-iot-jobs-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11036 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.166643 types-aiobotocore-iot-jobs-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2117 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      505 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      504 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7414 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7402 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8208 2023-08-04 13:40:46.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8206 2023-08-04 13:40:46.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5353 2023-08-04 13:40:46.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5346 2023-08-04 13:40:46.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:45.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12581 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      836 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:12.000000 types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/LICENSE` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iot-jobs-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-jobs-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-jobs-data"></a>
 
 # types-aiobotocore-iot-jobs-data
 
 [![PyPI - types-aiobotocore-iot-jobs-data](https://img.shields.io/pypi/v/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/)
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,50 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_jobs_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTJobsDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/literals/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.literals import (
-    JobExecutionStatusType,
-    IoTJobsDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iot_jobs_data.literals import JobExecutionStatusType
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTJobsDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.type_defs import (
-    DescribeJobExecutionRequestRequestTypeDef,
-    JobExecutionTypeDef,
-    ResponseMetadataTypeDef,
-    GetPendingJobExecutionsRequestRequestTypeDef,
-    JobExecutionSummaryTypeDef,
-    JobExecutionStateTypeDef,
-    StartNextPendingJobExecutionRequestRequestTypeDef,
-    UpdateJobExecutionRequestRequestTypeDef,
-    DescribeJobExecutionResponseTypeDef,
-    StartNextPendingJobExecutionResponseTypeDef,
-    GetPendingJobExecutionsResponseTypeDef,
-    UpdateJobExecutionResponseTypeDef,
-)
+from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestRequestTypeDef
 
 
 def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/README.md` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-iot-jobs-data
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore iot-jobs-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-jobs-data"></a>
 
 # types-aiobotocore-iot-jobs-data
 
 [![PyPI - types-aiobotocore-iot-jobs-data](https://img.shields.io/pypi/v/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-jobs-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/)
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,50 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_jobs_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTJobsDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/literals/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.literals import (
-    JobExecutionStatusType,
-    IoTJobsDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iot_jobs_data.literals import JobExecutionStatusType
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTJobsDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.type_defs import (
-    DescribeJobExecutionRequestRequestTypeDef,
-    JobExecutionTypeDef,
-    ResponseMetadataTypeDef,
-    GetPendingJobExecutionsRequestRequestTypeDef,
-    JobExecutionSummaryTypeDef,
-    JobExecutionStateTypeDef,
-    StartNextPendingJobExecutionRequestRequestTypeDef,
-    UpdateJobExecutionRequestRequestTypeDef,
-    DescribeJobExecutionResponseTypeDef,
-    StartNextPendingJobExecutionResponseTypeDef,
-    GetPendingJobExecutionsResponseTypeDef,
-    UpdateJobExecutionResponseTypeDef,
-)
+from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestRequestTypeDef
 
 
 def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/setup.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-jobs-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot_jobs_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/__main__.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane\nOther"
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

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/client.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "JobExecutionStatusType",
     "IoTJobsDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 JobExecutionStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "REMOVED", "SUCCEEDED", "TIMED_OUT"
 ]
 IoTJobsDataPlaneServiceName = Literal["iot-jobs-data"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -43,14 +41,15 @@
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
@@ -146,14 +145,15 @@
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
@@ -232,26 +232,28 @@
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

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/literals.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "JobExecutionStatusType",
     "IoTJobsDataPlaneServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 JobExecutionStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "REMOVED", "SUCCEEDED", "TIMED_OUT"
 ]
 IoTJobsDataPlaneServiceName = Literal["iot-jobs-data"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -41,14 +43,15 @@
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
@@ -144,14 +147,15 @@
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
@@ -230,26 +234,28 @@
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

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.py` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data/type_defs.pyi` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-jobs-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTJobsDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/
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
 [types-aiobotocore-iot-jobs-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,50 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot_jobs_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IoTJobsDataPlane` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/literals/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.literals import (
-    JobExecutionStatusType,
-    IoTJobsDataPlaneServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iot_jobs_data.literals import JobExecutionStatusType
 
 
 def check_value(value: JobExecutionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot_jobs_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTJobsDataPlane` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_jobs_data/type_defs/).
+
 ```python
-from types_aiobotocore_iot_jobs_data.type_defs import (
-    DescribeJobExecutionRequestRequestTypeDef,
-    JobExecutionTypeDef,
-    ResponseMetadataTypeDef,
-    GetPendingJobExecutionsRequestRequestTypeDef,
-    JobExecutionSummaryTypeDef,
-    JobExecutionStateTypeDef,
-    StartNextPendingJobExecutionRequestRequestTypeDef,
-    UpdateJobExecutionRequestRequestTypeDef,
-    DescribeJobExecutionResponseTypeDef,
-    StartNextPendingJobExecutionResponseTypeDef,
-    GetPendingJobExecutionsResponseTypeDef,
-    UpdateJobExecutionResponseTypeDef,
-)
+from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestRequestTypeDef
 
 
 def get_value() -> DescribeJobExecutionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iot-jobs-data-2.5.2.post1/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt` & `types-aiobotocore-iot-jobs-data-2.5.2.post2/types_aiobotocore_iot_jobs_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

