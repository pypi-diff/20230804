# Comparing `tmp/types-aiobotocore-snow-device-management-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-snow-device-management-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snow-device-management-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-snow-device-management-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-snow-device-management-2.5.2.post1.tar` & `types-aiobotocore-snow-device-management-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.361453 types-aiobotocore-snow-device-management-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-08-02 14:53:02.357453 types-aiobotocore-snow-device-management-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.361453 types-aiobotocore-snow-device-management-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-02 14:49:52.000000 types-aiobotocore-snow-device-management-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.353453 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:53.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.357453 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 14:53:02.000000 types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.026643 types-aiobotocore-snow-device-management-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14173 2023-08-04 13:59:27.026643 types-aiobotocore-snow-device-management-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12597 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.026643 types-aiobotocore-snow-device-management-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2167 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.026643 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1335 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1334 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      999 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14953 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14927 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8950 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8948 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5818 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5812 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14755 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14740 2023-08-04 13:53:51.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:50.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.026643 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14173 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1098 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       41 2023-08-04 13:59:26.000000 types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/LICENSE` & `types-aiobotocore-snow-device-management-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/PKG-INFO` & `types-aiobotocore-snow-device-management-2.5.2.post2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snow-device-management
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,95 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_snow_device_management.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SnowDeviceManagement` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/literals/).
+
 ```python
-from types_aiobotocore_snow_device_management.literals import (
-    AttachmentStatusType,
-    ExecutionStateType,
-    InstanceStateNameType,
-    IpAddressAssignmentType,
-    ListDeviceResourcesPaginatorName,
-    ListDevicesPaginatorName,
-    ListExecutionsPaginatorName,
-    ListTasksPaginatorName,
-    PhysicalConnectorTypeType,
-    TaskStateType,
-    UnlockStateType,
-    SnowDeviceManagementServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_snow_device_management.literals import AttachmentStatusType
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_snow_device_management.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `SnowDeviceManagement` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/type_defs/).
+
 ```python
-from types_aiobotocore_snow_device_management.type_defs import (
-    CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CapacityTypeDef,
-    CommandTypeDef,
-    CpuOptionsTypeDef,
-    DescribeDeviceEc2InputRequestTypeDef,
-    DescribeDeviceInputRequestTypeDef,
-    PhysicalNetworkInterfaceTypeDef,
-    SoftwareInformationTypeDef,
-    DescribeExecutionInputRequestTypeDef,
-    DescribeTaskInputRequestTypeDef,
-    DeviceSummaryTypeDef,
-    EbsInstanceBlockDeviceTypeDef,
-    ExecutionSummaryTypeDef,
-    InstanceStateTypeDef,
-    SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceResourcesInputRequestTypeDef,
-    ResourceSummaryTypeDef,
-    ListDevicesInputRequestTypeDef,
-    ListExecutionsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListTasksInputRequestTypeDef,
-    TaskSummaryTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateTaskInputRequestTypeDef,
-    DescribeDeviceOutputTypeDef,
-    ListDevicesOutputTypeDef,
-    InstanceBlockDeviceMappingTypeDef,
-    ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
-    ListDeviceResourcesOutputTypeDef,
-    ListTasksOutputTypeDef,
-    InstanceTypeDef,
-    InstanceSummaryTypeDef,
-    DescribeDeviceEc2OutputTypeDef,
-)
+from types_aiobotocore_snow_device_management.type_defs import CancelTaskInputRequestTypeDef
 
 
 def get_value() -> CancelTaskInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/README.md` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-snow-device-management
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore snow-device-management type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-snow-device-management"></a>
 
 # types-aiobotocore-snow-device-management
 
 [![PyPI - types-aiobotocore-snow-device-management](https://img.shields.io/pypi/v/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/)
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,95 +299,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_snow_device_management.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SnowDeviceManagement` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/literals/).
+
 ```python
-from types_aiobotocore_snow_device_management.literals import (
-    AttachmentStatusType,
-    ExecutionStateType,
-    InstanceStateNameType,
-    IpAddressAssignmentType,
-    ListDeviceResourcesPaginatorName,
-    ListDevicesPaginatorName,
-    ListExecutionsPaginatorName,
-    ListTasksPaginatorName,
-    PhysicalConnectorTypeType,
-    TaskStateType,
-    UnlockStateType,
-    SnowDeviceManagementServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_snow_device_management.literals import AttachmentStatusType
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_snow_device_management.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `SnowDeviceManagement` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/type_defs/).
+
 ```python
-from types_aiobotocore_snow_device_management.type_defs import (
-    CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CapacityTypeDef,
-    CommandTypeDef,
-    CpuOptionsTypeDef,
-    DescribeDeviceEc2InputRequestTypeDef,
-    DescribeDeviceInputRequestTypeDef,
-    PhysicalNetworkInterfaceTypeDef,
-    SoftwareInformationTypeDef,
-    DescribeExecutionInputRequestTypeDef,
-    DescribeTaskInputRequestTypeDef,
-    DeviceSummaryTypeDef,
-    EbsInstanceBlockDeviceTypeDef,
-    ExecutionSummaryTypeDef,
-    InstanceStateTypeDef,
-    SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceResourcesInputRequestTypeDef,
-    ResourceSummaryTypeDef,
-    ListDevicesInputRequestTypeDef,
-    ListExecutionsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListTasksInputRequestTypeDef,
-    TaskSummaryTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateTaskInputRequestTypeDef,
-    DescribeDeviceOutputTypeDef,
-    ListDevicesOutputTypeDef,
-    InstanceBlockDeviceMappingTypeDef,
-    ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
-    ListDeviceResourcesOutputTypeDef,
-    ListTasksOutputTypeDef,
-    InstanceTypeDef,
-    InstanceSummaryTypeDef,
-    DescribeDeviceEc2OutputTypeDef,
-)
+from types_aiobotocore_snow_device_management.type_defs import CancelTaskInputRequestTypeDef
 
 
 def get_value() -> CancelTaskInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/setup.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snow-device-management",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_snow_device_management"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SnowDeviceManagement 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__init__.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__init__.pyi` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/__main__.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SnowDeviceManagement 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement\nOther"
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

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/client.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/client.pyi` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/literals.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
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
@@ -168,14 +169,15 @@
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
@@ -254,26 +256,28 @@
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

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/literals.pyi` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,26 +254,28 @@
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

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/paginator.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/paginator.pyi` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/type_defs.py` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management/type_defs.pyi` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/PKG-INFO` & `types-aiobotocore-snow-device-management-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-snow-device-management
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SnowDeviceManagement 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore snow-device-management type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-snow-device-management"></a>
 
 # types-aiobotocore-snow-device-management
 
 [![PyPI - types-aiobotocore-snow-device-management](https://img.shields.io/pypi/v/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snow-device-management.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snow-device-management)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/)
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
 [types-aiobotocore-snow-device-management docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,95 +267,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_snow_device_management.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SnowDeviceManagement` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/literals/).
+
 ```python
-from types_aiobotocore_snow_device_management.literals import (
-    AttachmentStatusType,
-    ExecutionStateType,
-    InstanceStateNameType,
-    IpAddressAssignmentType,
-    ListDeviceResourcesPaginatorName,
-    ListDevicesPaginatorName,
-    ListExecutionsPaginatorName,
-    ListTasksPaginatorName,
-    PhysicalConnectorTypeType,
-    TaskStateType,
-    UnlockStateType,
-    SnowDeviceManagementServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_snow_device_management.literals import AttachmentStatusType
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_snow_device_management.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `SnowDeviceManagement` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snow_device_management/type_defs/).
+
 ```python
-from types_aiobotocore_snow_device_management.type_defs import (
-    CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CapacityTypeDef,
-    CommandTypeDef,
-    CpuOptionsTypeDef,
-    DescribeDeviceEc2InputRequestTypeDef,
-    DescribeDeviceInputRequestTypeDef,
-    PhysicalNetworkInterfaceTypeDef,
-    SoftwareInformationTypeDef,
-    DescribeExecutionInputRequestTypeDef,
-    DescribeTaskInputRequestTypeDef,
-    DeviceSummaryTypeDef,
-    EbsInstanceBlockDeviceTypeDef,
-    ExecutionSummaryTypeDef,
-    InstanceStateTypeDef,
-    SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeviceResourcesInputRequestTypeDef,
-    ResourceSummaryTypeDef,
-    ListDevicesInputRequestTypeDef,
-    ListExecutionsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListTasksInputRequestTypeDef,
-    TaskSummaryTypeDef,
-    TagResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateTaskInputRequestTypeDef,
-    DescribeDeviceOutputTypeDef,
-    ListDevicesOutputTypeDef,
-    InstanceBlockDeviceMappingTypeDef,
-    ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
-    ListDeviceResourcesOutputTypeDef,
-    ListTasksOutputTypeDef,
-    InstanceTypeDef,
-    InstanceSummaryTypeDef,
-    DescribeDeviceEc2OutputTypeDef,
-)
+from types_aiobotocore_snow_device_management.type_defs import CancelTaskInputRequestTypeDef
 
 
 def get_value() -> CancelTaskInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-snow-device-management-2.5.2.post1/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt` & `types-aiobotocore-snow-device-management-2.5.2.post2/types_aiobotocore_snow_device_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

