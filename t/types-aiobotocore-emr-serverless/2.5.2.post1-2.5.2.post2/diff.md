# Comparing `tmp/types-aiobotocore-emr-serverless-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-emr-serverless-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-emr-serverless-2.5.2.post1.tar` & `types-aiobotocore-emr-serverless-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.913588 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-02 14:38:31.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:30.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:16.000000 types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.992164 types-aiobotocore-emr-serverless-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-08-04 12:00:52.992164 types-aiobotocore-emr-serverless-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:52.992164 types-aiobotocore-emr-serverless-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.992164 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-04 11:46:00.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-08-04 11:46:00.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-08-04 11:46:00.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-08-04 11:46:00.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:59.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.992164 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:52.000000 types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/LICENSE` & `types-aiobotocore-emr-serverless-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/PKG-INFO` & `types-aiobotocore-emr-serverless-2.5.2.post2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,105 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_emr_serverless.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `EMRServerless` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/literals/).
+
 ```python
-from types_aiobotocore_emr_serverless.literals import (
-    ApplicationStateType,
-    ArchitectureType,
-    JobRunStateType,
-    ListApplicationsPaginatorName,
-    ListJobRunsPaginatorName,
-    EMRServerlessServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_emr_serverless.literals import ApplicationStateType
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_emr_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EMRServerless` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/type_defs/).
+
 ```python
-from types_aiobotocore_emr_serverless.type_defs import (
-    ApplicationSummaryTypeDef,
-    AutoStartConfigTypeDef,
-    AutoStopConfigTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
-    ImageConfigurationInputTypeDef,
-    NetworkConfigurationTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetDashboardForJobRunRequestRequestTypeDef,
-    GetJobRunRequestRequestTypeDef,
-    HiveTypeDef,
-    WorkerResourceConfigTypeDef,
-    SparkSubmitOutputTypeDef,
-    SparkSubmitTypeDef,
-    JobRunSummaryTypeDef,
-    ResourceUtilizationTypeDef,
-    TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    TimestampTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ManagedPersistenceMonitoringConfigurationTypeDef,
-    S3MonitoringConfigurationTypeDef,
-    StartApplicationRequestRequestTypeDef,
-    StopApplicationRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    WorkerTypeSpecificationInputTypeDef,
-    NetworkConfigurationUnionTypeDef,
-    InitialCapacityConfigTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    MonitoringConfigurationTypeDef,
-    ApplicationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    JobDriverUnionTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
-    GetApplicationResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    JobRunTypeDef,
-    ConfigurationOverridesUnionTypeDef,
-    StartJobRunRequestRequestTypeDef,
-    GetJobRunResponseTypeDef,
-)
+from types_aiobotocore_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
 
 def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/README.md` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-emr-serverless
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore emr-serverless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-emr-serverless"></a>
 
 # types-aiobotocore-emr-serverless
 
 [![PyPI - types-aiobotocore-emr-serverless](https://img.shields.io/pypi/v/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
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
 [types-aiobotocore-emr-serverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,105 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_emr_serverless.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `EMRServerless` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/literals/).
+
 ```python
-from types_aiobotocore_emr_serverless.literals import (
-    ApplicationStateType,
-    ArchitectureType,
-    JobRunStateType,
-    ListApplicationsPaginatorName,
-    ListJobRunsPaginatorName,
-    EMRServerlessServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_emr_serverless.literals import ApplicationStateType
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_emr_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EMRServerless` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/type_defs/).
+
 ```python
-from types_aiobotocore_emr_serverless.type_defs import (
-    ApplicationSummaryTypeDef,
-    AutoStartConfigTypeDef,
-    AutoStopConfigTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
-    ImageConfigurationInputTypeDef,
-    NetworkConfigurationTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetDashboardForJobRunRequestRequestTypeDef,
-    GetJobRunRequestRequestTypeDef,
-    HiveTypeDef,
-    WorkerResourceConfigTypeDef,
-    SparkSubmitOutputTypeDef,
-    SparkSubmitTypeDef,
-    JobRunSummaryTypeDef,
-    ResourceUtilizationTypeDef,
-    TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    TimestampTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ManagedPersistenceMonitoringConfigurationTypeDef,
-    S3MonitoringConfigurationTypeDef,
-    StartApplicationRequestRequestTypeDef,
-    StopApplicationRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    WorkerTypeSpecificationInputTypeDef,
-    NetworkConfigurationUnionTypeDef,
-    InitialCapacityConfigTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    MonitoringConfigurationTypeDef,
-    ApplicationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    JobDriverUnionTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
-    GetApplicationResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    JobRunTypeDef,
-    ConfigurationOverridesUnionTypeDef,
-    StartJobRunRequestRequestTypeDef,
-    GetJobRunResponseTypeDef,
-)
+from types_aiobotocore_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
 
 def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/setup.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-serverless",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__init__.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/__main__.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.EMRServerless 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesUnionTypeDef,
+    ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverUnionTypeDef,
+    JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -122,15 +122,15 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -237,16 +237,16 @@
 
     async def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverUnionTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        jobDriver: JobDriverTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -283,15 +283,15 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/client.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesUnionTypeDef,
+    ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverUnionTypeDef,
+    JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -114,15 +114,15 @@
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
@@ -219,16 +219,16 @@
         """
     async def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: JobDriverUnionTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        jobDriver: JobDriverTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
@@ -261,15 +261,15 @@
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/literals.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/paginator.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.py` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,25 @@
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationOutputTypeDef",
+    "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
-    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "TimestampTypeDef",
@@ -61,33 +58,28 @@
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
-    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
-    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "JobDriverUnionTypeDef",
-    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
-    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -173,19 +165,19 @@
 
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "subnetIds": List[str],
-        "securityGroupIds": List[str],
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -201,47 +193,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredConfigurationOutputTypeDef = TypedDict(
-    "_RequiredConfigurationOutputTypeDef",
-    {
-        "classification": str,
-    },
-)
-_OptionalConfigurationOutputTypeDef = TypedDict(
-    "_OptionalConfigurationOutputTypeDef",
-    {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
-
-class ConfigurationOutputTypeDef(
-    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Mapping[str, str],
-        "configurations": Sequence[Dict[str, Any]],
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
     },
     total=False,
 )
 
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
@@ -251,23 +221,14 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -332,46 +293,24 @@
 
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
 
-_RequiredSparkSubmitOutputTypeDef = TypedDict(
-    "_RequiredSparkSubmitOutputTypeDef",
-    {
-        "entryPoint": str,
-    },
-)
-_OptionalSparkSubmitOutputTypeDef = TypedDict(
-    "_OptionalSparkSubmitOutputTypeDef",
-    {
-        "entryPointArguments": List[str],
-        "sparkSubmitParameters": str,
-    },
-    total=False,
-)
-
-
-class SparkSubmitOutputTypeDef(
-    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
-):
-    pass
-
-
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": Sequence[str],
+        "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
 
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
@@ -569,17 +508,14 @@
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -593,23 +529,14 @@
 
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
 
-JobDriverOutputTypeDef = TypedDict(
-    "JobDriverOutputTypeDef",
-    {
-        "sparkSubmit": SparkSubmitOutputTypeDef,
-        "hive": HiveTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
     total=False,
@@ -712,15 +639,15 @@
         "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
@@ -786,28 +713,18 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
-ConfigurationOverridesOutputTypeDef = TypedDict(
-    "ConfigurationOverridesOutputTypeDef",
-    {
-        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": MonitoringConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
+        "applicationConfiguration": List["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
@@ -834,40 +751,37 @@
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverOutputTypeDef,
+        "jobDriver": JobDriverTypeDef,
     },
 )
 _OptionalJobRunTypeDef = TypedDict(
     "_OptionalJobRunTypeDef",
     {
         "name": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
 
-ConfigurationOverridesUnionTypeDef = Union[
-    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless/type_defs.pyi` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,25 @@
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationOutputTypeDef",
+    "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
-    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "TimestampTypeDef",
@@ -60,33 +57,28 @@
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
-    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
-    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "JobDriverUnionTypeDef",
-    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
-    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -166,19 +158,19 @@
 )
 
 class MaximumAllowedResourcesTypeDef(
     _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
 ):
     pass
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "subnetIds": List[str],
-        "securityGroupIds": List[str],
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
     total=False,
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -194,45 +186,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredConfigurationOutputTypeDef = TypedDict(
-    "_RequiredConfigurationOutputTypeDef",
-    {
-        "classification": str,
-    },
-)
-_OptionalConfigurationOutputTypeDef = TypedDict(
-    "_OptionalConfigurationOutputTypeDef",
-    {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
-class ConfigurationOutputTypeDef(
-    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Mapping[str, str],
-        "configurations": Sequence[Dict[str, Any]],
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
     },
     total=False,
 )
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
@@ -240,23 +212,14 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -317,44 +280,24 @@
 )
 
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
-_RequiredSparkSubmitOutputTypeDef = TypedDict(
-    "_RequiredSparkSubmitOutputTypeDef",
-    {
-        "entryPoint": str,
-    },
-)
-_OptionalSparkSubmitOutputTypeDef = TypedDict(
-    "_OptionalSparkSubmitOutputTypeDef",
-    {
-        "entryPointArguments": List[str],
-        "sparkSubmitParameters": str,
-    },
-    total=False,
-)
-
-class SparkSubmitOutputTypeDef(
-    _RequiredSparkSubmitOutputTypeDef, _OptionalSparkSubmitOutputTypeDef
-):
-    pass
-
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": Sequence[str],
+        "entryPointArguments": List[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
@@ -548,17 +491,14 @@
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -570,23 +510,14 @@
 )
 
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
-JobDriverOutputTypeDef = TypedDict(
-    "JobDriverOutputTypeDef",
-    {
-        "sparkSubmit": SparkSubmitOutputTypeDef,
-        "hive": HiveTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
     total=False,
@@ -685,15 +616,15 @@
         "name": str,
         "stateDetails": str,
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
@@ -753,28 +684,18 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
-ConfigurationOverridesOutputTypeDef = TypedDict(
-    "ConfigurationOverridesOutputTypeDef",
-    {
-        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": MonitoringConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
+        "applicationConfiguration": List["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
@@ -801,38 +722,35 @@
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverOutputTypeDef,
+        "jobDriver": JobDriverTypeDef,
     },
 )
 _OptionalJobRunTypeDef = TypedDict(
     "_OptionalJobRunTypeDef",
     {
         "name": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
-ConfigurationOverridesUnionTypeDef = Union[
-    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post1/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-emr-serverless-2.5.2.post2/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

