# Comparing `tmp/types-aiobotocore-emr-containers-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-emr-containers-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-containers-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-containers-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:52 2023, max compression
```

## Comparing `types-aiobotocore-emr-containers-2.5.2.post1.tar` & `types-aiobotocore-emr-containers-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.793588 types-aiobotocore-emr-containers-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-08-02 14:52:16.793588 types-aiobotocore-emr-containers-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.793588 types-aiobotocore-emr-containers-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:38:27.000000 types-aiobotocore-emr-containers-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.793588 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19931 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29048 2023-08-02 14:38:30.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:28.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.793588 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:16.000000 types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.936161 types-aiobotocore-emr-containers-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-08-04 12:00:52.936161 types-aiobotocore-emr-containers-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:52.936161 types-aiobotocore-emr-containers-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.932161 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-08-04 11:45:59.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25924 2023-08-04 11:45:57.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:56.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.936161 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:52.000000 types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/LICENSE` & `types-aiobotocore-emr-containers-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,129 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_emr_containers.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `EMRContainers` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/literals/).
+
 ```python
-from types_aiobotocore_emr_containers.literals import (
-    ContainerProviderTypeType,
-    EndpointStateType,
-    FailureReasonType,
-    JobRunStateType,
-    ListJobRunsPaginatorName,
-    ListJobTemplatesPaginatorName,
-    ListManagedEndpointsPaginatorName,
-    ListVirtualClustersPaginatorName,
-    PersistentAppUIType,
-    TemplateParameterDataTypeType,
-    VirtualClusterStateType,
-    EMRContainersServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_emr_containers.literals import ContainerProviderTypeType
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_emr_containers.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EMRContainers` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/type_defs/).
+
 ```python
-from types_aiobotocore_emr_containers.type_defs import (
-    CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CertificateTypeDef,
-    CloudWatchMonitoringConfigurationTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
-    EksInfoTypeDef,
-    ContainerLogRotationConfigurationTypeDef,
-    CredentialsTypeDef,
-    DeleteJobTemplateRequestRequestTypeDef,
-    DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteVirtualClusterRequestRequestTypeDef,
-    DescribeJobRunRequestRequestTypeDef,
-    DescribeJobTemplateRequestRequestTypeDef,
-    DescribeManagedEndpointRequestRequestTypeDef,
-    DescribeVirtualClusterRequestRequestTypeDef,
-    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
-    SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3MonitoringConfigurationTypeDef,
-    ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    ContainerInfoTypeDef,
-    GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
-    MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderTypeDef,
-    JobDriverUnionTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
-    ParametricConfigurationOverridesOutputTypeDef,
-    ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
-    VirtualClusterTypeDef,
-    EndpointTypeDef,
-    JobRunTypeDef,
-    ConfigurationOverridesUnionTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
-    StartJobRunRequestRequestTypeDef,
-    JobTemplateDataOutputTypeDef,
-    JobTemplateDataTypeDef,
-    DescribeVirtualClusterResponseTypeDef,
-    ListVirtualClustersResponseTypeDef,
-    DescribeManagedEndpointResponseTypeDef,
-    ListManagedEndpointsResponseTypeDef,
-    DescribeJobRunResponseTypeDef,
-    ListJobRunsResponseTypeDef,
-    JobTemplateTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateDataUnionTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    ListJobTemplatesResponseTypeDef,
-)
+from types_aiobotocore_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef
 
 
 def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/README.md` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-emr-containers
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore emr-containers type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-emr-containers"></a>
 
 # types-aiobotocore-emr-containers
 
 [![PyPI - types-aiobotocore-emr-containers](https://img.shields.io/pypi/v/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,129 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_emr_containers.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `EMRContainers` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/literals/).
+
 ```python
-from types_aiobotocore_emr_containers.literals import (
-    ContainerProviderTypeType,
-    EndpointStateType,
-    FailureReasonType,
-    JobRunStateType,
-    ListJobRunsPaginatorName,
-    ListJobTemplatesPaginatorName,
-    ListManagedEndpointsPaginatorName,
-    ListVirtualClustersPaginatorName,
-    PersistentAppUIType,
-    TemplateParameterDataTypeType,
-    VirtualClusterStateType,
-    EMRContainersServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_emr_containers.literals import ContainerProviderTypeType
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_emr_containers.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EMRContainers` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/type_defs/).
+
 ```python
-from types_aiobotocore_emr_containers.type_defs import (
-    CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CertificateTypeDef,
-    CloudWatchMonitoringConfigurationTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
-    EksInfoTypeDef,
-    ContainerLogRotationConfigurationTypeDef,
-    CredentialsTypeDef,
-    DeleteJobTemplateRequestRequestTypeDef,
-    DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteVirtualClusterRequestRequestTypeDef,
-    DescribeJobRunRequestRequestTypeDef,
-    DescribeJobTemplateRequestRequestTypeDef,
-    DescribeManagedEndpointRequestRequestTypeDef,
-    DescribeVirtualClusterRequestRequestTypeDef,
-    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
-    SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3MonitoringConfigurationTypeDef,
-    ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    ContainerInfoTypeDef,
-    GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
-    MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderTypeDef,
-    JobDriverUnionTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
-    ParametricConfigurationOverridesOutputTypeDef,
-    ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
-    VirtualClusterTypeDef,
-    EndpointTypeDef,
-    JobRunTypeDef,
-    ConfigurationOverridesUnionTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
-    StartJobRunRequestRequestTypeDef,
-    JobTemplateDataOutputTypeDef,
-    JobTemplateDataTypeDef,
-    DescribeVirtualClusterResponseTypeDef,
-    ListVirtualClustersResponseTypeDef,
-    DescribeManagedEndpointResponseTypeDef,
-    ListManagedEndpointsResponseTypeDef,
-    DescribeJobRunResponseTypeDef,
-    ListJobRunsResponseTypeDef,
-    JobTemplateTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateDataUnionTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    ListJobTemplatesResponseTypeDef,
-)
+from types_aiobotocore_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef
 
 
 def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/setup.py` & `types-aiobotocore-emr-containers-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-containers",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__init__.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__init__.pyi` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/__main__.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.EMRContainers 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/client.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesUnionTypeDef,
+    ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverUnionTypeDef,
-    JobTemplateDataUnionTypeDef,
+    JobDriverTypeDef,
+    JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
@@ -55,34 +55,30 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRContainersClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class EMRContainersClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
     """
 
     meta: ClientMeta
@@ -91,168 +87,153 @@
     def exceptions(self) -> Exceptions:
         """
         EMRContainersClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#can_paginate)
         """
-
     async def cancel_job_run(
         self, *, id: str, virtualClusterId: str
     ) -> CancelJobRunResponseTypeDef:
         """
         Cancels a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.cancel_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#cancel_job_run)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#close)
         """
-
     async def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: JobTemplateDataUnionTypeDef,
+        jobTemplateData: JobTemplateDataTypeDef,
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_job_template)
         """
-
     async def create_managed_endpoint(
         self,
         *,
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_managed_endpoint)
         """
-
     async def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
         tags: Mapping[str, str] = ...
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_virtual_cluster)
         """
-
     async def delete_job_template(self, *, id: str) -> DeleteJobTemplateResponseTypeDef:
         """
         Deletes a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_job_template)
         """
-
     async def delete_managed_endpoint(
         self, *, id: str, virtualClusterId: str
     ) -> DeleteManagedEndpointResponseTypeDef:
         """
         Deletes a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_managed_endpoint)
         """
-
     async def delete_virtual_cluster(self, *, id: str) -> DeleteVirtualClusterResponseTypeDef:
         """
         Deletes a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_virtual_cluster)
         """
-
     async def describe_job_run(
         self, *, id: str, virtualClusterId: str
     ) -> DescribeJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_job_run)
         """
-
     async def describe_job_template(self, *, id: str) -> DescribeJobTemplateResponseTypeDef:
         """
         Displays detailed information about a specified job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_job_template)
         """
-
     async def describe_managed_endpoint(
         self, *, id: str, virtualClusterId: str
     ) -> DescribeManagedEndpointResponseTypeDef:
         """
         Displays detailed information about a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_managed_endpoint)
         """
-
     async def describe_virtual_cluster(self, *, id: str) -> DescribeVirtualClusterResponseTypeDef:
         """
         Displays detailed information about a specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_virtual_cluster)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#generate_presigned_url)
         """
-
     async def get_managed_endpoint_session_credentials(
         self,
         *,
         endpointIdentifier: str,
         virtualClusterIdentifier: str,
         executionRoleArn: str,
         credentialType: str,
@@ -262,15 +243,14 @@
     ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
         """
         Generate a session token to connect to a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
-
     async def list_job_runs(
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
@@ -280,30 +260,28 @@
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_runs)
         """
-
     async def list_job_templates(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_templates)
         """
-
     async def list_managed_endpoints(
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
@@ -313,25 +291,23 @@
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_managed_endpoints)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_tags_for_resource)
         """
-
     async def list_virtual_clusters(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
@@ -341,91 +317,82 @@
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_virtual_clusters)
         """
-
     async def start_job_run(
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: JobDriverUnionTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        jobDriver: JobDriverTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#start_job_run)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns tags to resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#untag_resource)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_job_runs"]) -> ListJobRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_job_templates"]
     ) -> ListJobTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_managed_endpoints"]
     ) -> ListManagedEndpointsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_clusters"]
     ) -> ListVirtualClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "EMRContainersClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/client.pyi` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesUnionTypeDef,
+    ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverUnionTypeDef,
-    JobTemplateDataUnionTypeDef,
+    JobDriverTypeDef,
+    JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
@@ -55,30 +55,34 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("EMRContainersClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class EMRContainersClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
     """
 
     meta: ClientMeta
@@ -87,153 +91,168 @@
     def exceptions(self) -> Exceptions:
         """
         EMRContainersClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#can_paginate)
         """
+
     async def cancel_job_run(
         self, *, id: str, virtualClusterId: str
     ) -> CancelJobRunResponseTypeDef:
         """
         Cancels a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.cancel_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#cancel_job_run)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#close)
         """
+
     async def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: JobTemplateDataUnionTypeDef,
+        jobTemplateData: JobTemplateDataTypeDef,
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_job_template)
         """
+
     async def create_managed_endpoint(
         self,
         *,
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_managed_endpoint)
         """
+
     async def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
         tags: Mapping[str, str] = ...
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#create_virtual_cluster)
         """
+
     async def delete_job_template(self, *, id: str) -> DeleteJobTemplateResponseTypeDef:
         """
         Deletes a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_job_template)
         """
+
     async def delete_managed_endpoint(
         self, *, id: str, virtualClusterId: str
     ) -> DeleteManagedEndpointResponseTypeDef:
         """
         Deletes a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_managed_endpoint)
         """
+
     async def delete_virtual_cluster(self, *, id: str) -> DeleteVirtualClusterResponseTypeDef:
         """
         Deletes a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.delete_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#delete_virtual_cluster)
         """
+
     async def describe_job_run(
         self, *, id: str, virtualClusterId: str
     ) -> DescribeJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_job_run)
         """
+
     async def describe_job_template(self, *, id: str) -> DescribeJobTemplateResponseTypeDef:
         """
         Displays detailed information about a specified job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_job_template)
         """
+
     async def describe_managed_endpoint(
         self, *, id: str, virtualClusterId: str
     ) -> DescribeManagedEndpointResponseTypeDef:
         """
         Displays detailed information about a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_managed_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_managed_endpoint)
         """
+
     async def describe_virtual_cluster(self, *, id: str) -> DescribeVirtualClusterResponseTypeDef:
         """
         Displays detailed information about a specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_virtual_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#describe_virtual_cluster)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#generate_presigned_url)
         """
+
     async def get_managed_endpoint_session_credentials(
         self,
         *,
         endpointIdentifier: str,
         virtualClusterIdentifier: str,
         executionRoleArn: str,
         credentialType: str,
@@ -243,14 +262,15 @@
     ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
         """
         Generate a session token to connect to a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
+
     async def list_job_runs(
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         name: str = ...,
@@ -260,28 +280,30 @@
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_runs)
         """
+
     async def list_job_templates(
         self,
         *,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_job_templates)
         """
+
     async def list_managed_endpoints(
         self,
         *,
         virtualClusterId: str,
         createdBefore: TimestampTypeDef = ...,
         createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
@@ -291,23 +313,25 @@
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_managed_endpoints)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_tags_for_resource)
         """
+
     async def list_virtual_clusters(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
@@ -317,82 +341,91 @@
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#list_virtual_clusters)
         """
+
     async def start_job_run(
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: JobDriverUnionTypeDef = ...,
-        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
+        jobDriver: JobDriverTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.start_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#start_job_run)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns tags to resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#untag_resource)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_job_runs"]) -> ListJobRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_job_templates"]
     ) -> ListJobTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_managed_endpoints"]
     ) -> ListManagedEndpointsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_clusters"]
     ) -> ListVirtualClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "EMRContainersClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/client/)
         """
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/literals.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/literals.pyi` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/paginator.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/paginator.pyi` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/type_defs.py` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,35 +29,32 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
-    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -73,50 +70,43 @@
     "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
-    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
-    "JobDriverUnionTypeDef",
-    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
-    "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
+    "CreateManagedEndpointRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
-    "ConfigurationOverridesUnionTypeDef",
-    "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
-    "JobTemplateTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateDataUnionTypeDef",
+    "JobTemplateTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -155,44 +145,20 @@
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
-
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
@@ -200,19 +166,17 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
@@ -300,53 +264,29 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
 )
 
-_RequiredSparkSubmitJobDriverOutputTypeDef = TypedDict(
-    "_RequiredSparkSubmitJobDriverOutputTypeDef",
-    {
-        "entryPoint": str,
-    },
-)
-_OptionalSparkSubmitJobDriverOutputTypeDef = TypedDict(
-    "_OptionalSparkSubmitJobDriverOutputTypeDef",
-    {
-        "entryPointArguments": List[str],
-        "sparkSubmitParameters": str,
-    },
-    total=False,
-)
-
-
-class SparkSubmitJobDriverOutputTypeDef(
-    _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
-):
-    pass
-
-
 _RequiredSparkSubmitJobDriverTypeDef = TypedDict(
     "_RequiredSparkSubmitJobDriverTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitJobDriverTypeDef = TypedDict(
@@ -354,21 +294,19 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
-
 RetryPolicyConfigurationTypeDef = TypedDict(
     "RetryPolicyConfigurationTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
@@ -545,23 +483,14 @@
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobDriverOutputTypeDef = TypedDict(
-    "JobDriverOutputTypeDef",
-    {
-        "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
-        "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
@@ -581,22 +510,20 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -608,21 +535,19 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -654,22 +579,20 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -681,22 +604,20 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
@@ -752,49 +673,28 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
-
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
-
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
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-ParametricConfigurationOverridesOutputTypeDef = TypedDict(
-    "ParametricConfigurationOverridesOutputTypeDef",
-    {
-        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ParametricConfigurationOverridesTypeDef = TypedDict(
     "ParametricConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
@@ -812,50 +712,75 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
-
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
         "containerProvider": ContainerProviderTypeDef,
         "createdAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "name": str,
+        "virtualClusterId": str,
+        "type": str,
+        "releaseLabel": str,
+        "executionRoleArn": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "certificateArn": str,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateManagedEndpointRequestRequestTypeDef(
+    _RequiredCreateManagedEndpointRequestRequestTypeDef,
+    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+):
+    pass
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "type": str,
         "state": EndpointStateType,
         "releaseLabel": str,
         "executionRoleArn": str,
         "certificateArn": str,
         "certificateAuthority": CertificateTypeDef,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
         "serverUrl": str,
         "createdAt": datetime,
         "securityGroup": str,
         "subnetIds": List[str],
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
@@ -870,60 +795,28 @@
         "name": str,
         "virtualClusterId": str,
         "arn": str,
         "state": JobRunStateType,
         "clientToken": str,
         "executionRoleArn": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
-        "jobDriver": JobDriverOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "jobDriver": JobDriverTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
-ConfigurationOverridesUnionTypeDef = Union[
-    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-]
-_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
-    {
-        "name": str,
-        "virtualClusterId": str,
-        "type": str,
-        "releaseLabel": str,
-        "executionRoleArn": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
-    {
-        "certificateArn": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateManagedEndpointRequestRequestTypeDef(
-    _RequiredCreateManagedEndpointRequestRequestTypeDef,
-    _OptionalCreateManagedEndpointRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -939,46 +832,19 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredJobTemplateDataOutputTypeDef = TypedDict(
-    "_RequiredJobTemplateDataOutputTypeDef",
-    {
-        "executionRoleArn": str,
-        "releaseLabel": str,
-        "jobDriver": JobDriverOutputTypeDef,
-    },
-)
-_OptionalJobTemplateDataOutputTypeDef = TypedDict(
-    "_OptionalJobTemplateDataOutputTypeDef",
-    {
-        "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
-        "parameterConfiguration": Dict[str, TemplateParameterConfigurationTypeDef],
-        "jobTags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class JobTemplateDataOutputTypeDef(
-    _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
-):
-    pass
-
-
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -989,19 +855,17 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
-
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1045,40 +909,14 @@
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
-    {
-        "jobTemplateData": JobTemplateDataOutputTypeDef,
-    },
-)
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
-    {
-        "name": str,
-        "id": str,
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "tags": Dict[str, str],
-        "kmsKeyArn": str,
-        "decryptionError": str,
-    },
-    total=False,
-)
-
-
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
-
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "name": str,
         "clientToken": str,
         "jobTemplateData": JobTemplateDataTypeDef,
     },
@@ -1088,22 +926,43 @@
     {
         "tags": Mapping[str, str],
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+_RequiredJobTemplateTypeDef = TypedDict(
+    "_RequiredJobTemplateTypeDef",
+    {
+        "jobTemplateData": JobTemplateDataTypeDef,
+    },
+)
+_OptionalJobTemplateTypeDef = TypedDict(
+    "_OptionalJobTemplateTypeDef",
+    {
+        "name": str,
+        "id": str,
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "tags": Dict[str, str],
+        "kmsKeyArn": str,
+        "decryptionError": str,
+    },
+    total=False,
+)
+
+class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+    pass
 
-JobTemplateDataUnionTypeDef = Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef]
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers/type_defs.pyi` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,34 +29,33 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
-    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -72,50 +71,43 @@
     "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
-    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
-    "JobDriverUnionTypeDef",
-    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
-    "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
+    "CreateManagedEndpointRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
-    "ConfigurationOverridesUnionTypeDef",
-    "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
-    "JobTemplateTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateDataUnionTypeDef",
+    "JobTemplateTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -154,39 +146,21 @@
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
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
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
@@ -195,17 +169,19 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
@@ -293,49 +269,31 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
 )
 
-_RequiredSparkSubmitJobDriverOutputTypeDef = TypedDict(
-    "_RequiredSparkSubmitJobDriverOutputTypeDef",
-    {
-        "entryPoint": str,
-    },
-)
-_OptionalSparkSubmitJobDriverOutputTypeDef = TypedDict(
-    "_OptionalSparkSubmitJobDriverOutputTypeDef",
-    {
-        "entryPointArguments": List[str],
-        "sparkSubmitParameters": str,
-    },
-    total=False,
-)
-
-class SparkSubmitJobDriverOutputTypeDef(
-    _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
-):
-    pass
-
 _RequiredSparkSubmitJobDriverTypeDef = TypedDict(
     "_RequiredSparkSubmitJobDriverTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitJobDriverTypeDef = TypedDict(
@@ -343,19 +301,21 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
+
 RetryPolicyConfigurationTypeDef = TypedDict(
     "RetryPolicyConfigurationTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
@@ -532,23 +492,14 @@
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobDriverOutputTypeDef = TypedDict(
-    "JobDriverOutputTypeDef",
-    {
-        "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
-        "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
@@ -568,20 +519,22 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -593,19 +546,21 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -637,20 +592,22 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -662,20 +619,22 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
@@ -731,47 +690,30 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
+
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
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
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-ParametricConfigurationOverridesOutputTypeDef = TypedDict(
-    "ParametricConfigurationOverridesOutputTypeDef",
-    {
-        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ParametricConfigurationOverridesTypeDef = TypedDict(
     "ParametricConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
@@ -789,48 +731,79 @@
     "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVirtualClusterRequestRequestTypeDef(
     _RequiredCreateVirtualClusterRequestRequestTypeDef,
     _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
+
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
         "containerProvider": ContainerProviderTypeDef,
         "createdAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "name": str,
+        "virtualClusterId": str,
+        "type": str,
+        "releaseLabel": str,
+        "executionRoleArn": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "certificateArn": str,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateManagedEndpointRequestRequestTypeDef(
+    _RequiredCreateManagedEndpointRequestRequestTypeDef,
+    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+):
+    pass
+
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "type": str,
         "state": EndpointStateType,
         "releaseLabel": str,
         "executionRoleArn": str,
         "certificateArn": str,
         "certificateAuthority": CertificateTypeDef,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
         "serverUrl": str,
         "createdAt": datetime,
         "securityGroup": str,
         "subnetIds": List[str],
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
@@ -845,58 +818,28 @@
         "name": str,
         "virtualClusterId": str,
         "arn": str,
         "state": JobRunStateType,
         "clientToken": str,
         "executionRoleArn": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
-        "jobDriver": JobDriverOutputTypeDef,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "jobDriver": JobDriverTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
-ConfigurationOverridesUnionTypeDef = Union[
-    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-]
-_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
-    {
-        "name": str,
-        "virtualClusterId": str,
-        "type": str,
-        "releaseLabel": str,
-        "executionRoleArn": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
-    {
-        "certificateArn": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateManagedEndpointRequestRequestTypeDef(
-    _RequiredCreateManagedEndpointRequestRequestTypeDef,
-    _OptionalCreateManagedEndpointRequestRequestTypeDef,
-):
-    pass
-
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -912,41 +855,20 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-_RequiredJobTemplateDataOutputTypeDef = TypedDict(
-    "_RequiredJobTemplateDataOutputTypeDef",
-    {
-        "executionRoleArn": str,
-        "releaseLabel": str,
-        "jobDriver": JobDriverOutputTypeDef,
-    },
-)
-_OptionalJobTemplateDataOutputTypeDef = TypedDict(
-    "_OptionalJobTemplateDataOutputTypeDef",
-    {
-        "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
-        "parameterConfiguration": Dict[str, TemplateParameterConfigurationTypeDef],
-        "jobTags": Dict[str, str],
-    },
-    total=False,
-)
-
-class JobTemplateDataOutputTypeDef(
-    _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
-):
-    pass
 
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
@@ -958,17 +880,19 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
+
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1012,18 +936,42 @@
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+    {
+        "name": str,
+        "clientToken": str,
+        "jobTemplateData": JobTemplateDataTypeDef,
+    },
+)
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
-        "jobTemplateData": JobTemplateDataOutputTypeDef,
+        "jobTemplateData": JobTemplateDataTypeDef,
     },
 )
 _OptionalJobTemplateTypeDef = TypedDict(
     "_OptionalJobTemplateTypeDef",
     {
         "name": str,
         "id": str,
@@ -1033,40 +981,19 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
+
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
-    {
-        "name": str,
-        "clientToken": str,
-        "jobTemplateData": JobTemplateDataTypeDef,
-    },
-)
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-        "kmsKeyArn": str,
-    },
-    total=False,
-)
-
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
-):
-    pass
 
-JobTemplateDataUnionTypeDef = Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef]
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.2.post2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-emr-containers
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore emr-containers type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-emr-containers"></a>
 
 # types-aiobotocore-emr-containers
 
 [![PyPI - types-aiobotocore-emr-containers](https://img.shields.io/pypi/v/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
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
 [types-aiobotocore-emr-containers docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,129 +271,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_emr_containers.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `EMRContainers` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/literals/).
+
 ```python
-from types_aiobotocore_emr_containers.literals import (
-    ContainerProviderTypeType,
-    EndpointStateType,
-    FailureReasonType,
-    JobRunStateType,
-    ListJobRunsPaginatorName,
-    ListJobTemplatesPaginatorName,
-    ListManagedEndpointsPaginatorName,
-    ListVirtualClustersPaginatorName,
-    PersistentAppUIType,
-    TemplateParameterDataTypeType,
-    VirtualClusterStateType,
-    EMRContainersServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_emr_containers.literals import ContainerProviderTypeType
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_emr_containers.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EMRContainers` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/type_defs/).
+
 ```python
-from types_aiobotocore_emr_containers.type_defs import (
-    CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CertificateTypeDef,
-    CloudWatchMonitoringConfigurationTypeDef,
-    ConfigurationOutputTypeDef,
-    ConfigurationTypeDef,
-    EksInfoTypeDef,
-    ContainerLogRotationConfigurationTypeDef,
-    CredentialsTypeDef,
-    DeleteJobTemplateRequestRequestTypeDef,
-    DeleteManagedEndpointRequestRequestTypeDef,
-    DeleteVirtualClusterRequestRequestTypeDef,
-    DescribeJobRunRequestRequestTypeDef,
-    DescribeJobTemplateRequestRequestTypeDef,
-    DescribeManagedEndpointRequestRequestTypeDef,
-    DescribeVirtualClusterRequestRequestTypeDef,
-    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
-    SparkSqlJobDriverTypeDef,
-    SparkSubmitJobDriverOutputTypeDef,
-    SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
-    RetryPolicyExecutionTypeDef,
-    TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    TimestampTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    S3MonitoringConfigurationTypeDef,
-    ParametricCloudWatchMonitoringConfigurationTypeDef,
-    ParametricS3MonitoringConfigurationTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    ContainerInfoTypeDef,
-    GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
-    MonitoringConfigurationTypeDef,
-    ParametricMonitoringConfigurationTypeDef,
-    ContainerProviderTypeDef,
-    JobDriverUnionTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
-    ParametricConfigurationOverridesOutputTypeDef,
-    ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
-    VirtualClusterTypeDef,
-    EndpointTypeDef,
-    JobRunTypeDef,
-    ConfigurationOverridesUnionTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
-    StartJobRunRequestRequestTypeDef,
-    JobTemplateDataOutputTypeDef,
-    JobTemplateDataTypeDef,
-    DescribeVirtualClusterResponseTypeDef,
-    ListVirtualClustersResponseTypeDef,
-    DescribeManagedEndpointResponseTypeDef,
-    ListManagedEndpointsResponseTypeDef,
-    DescribeJobRunResponseTypeDef,
-    ListJobRunsResponseTypeDef,
-    JobTemplateTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
-    JobTemplateDataUnionTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    ListJobTemplatesResponseTypeDef,
-)
+from types_aiobotocore_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef
 
 
 def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post1/types_aiobotocore_emr_containers.egg-info/SOURCES.txt` & `types-aiobotocore-emr-containers-2.5.2.post2/types_aiobotocore_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

