# Comparing `tmp/types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11127 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      514 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      513 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12963 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12941 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8701 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8699 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12286 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12275 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/LICENSE` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,81 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotdeviceadvisor.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTDeviceAdvisor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/literals/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
-    ProtocolType,
-    StatusType,
-    SuiteRunStatusType,
-    TestCaseScenarioStatusType,
-    TestCaseScenarioTypeType,
-    IoTDeviceAdvisorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotdeviceadvisor.literals import AuthenticationMethodType
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDeviceAdvisor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/type_defs/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    ResponseMetadataTypeDef,
-    DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestTypeDef,
-    GetEndpointRequestRequestTypeDef,
-    GetSuiteDefinitionRequestRequestTypeDef,
-    GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunRequestRequestTypeDef,
-    ListSuiteDefinitionsRequestRequestTypeDef,
-    ListSuiteRunsRequestRequestTypeDef,
-    SuiteRunInformationTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StopSuiteRunRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestCaseScenarioTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSuiteDefinitionResponseTypeDef,
-    GetEndpointResponseTypeDef,
-    GetSuiteRunReportResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSuiteRunResponseTypeDef,
-    UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteDefinitionInformationTypeDef,
-    SuiteRunConfigurationOutputTypeDef,
-    SuiteRunConfigurationTypeDef,
-    ListSuiteRunsResponseTypeDef,
-    TestCaseRunTypeDef,
-    GetSuiteDefinitionResponseTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
-    SuiteDefinitionConfigurationUnionTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
-    StartSuiteRunRequestRequestTypeDef,
-    SuiteRunConfigurationUnionTypeDef,
-    GroupResultTypeDef,
-    TestResultTypeDef,
-    GetSuiteRunResponseTypeDef,
-)
+from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/README.md` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/README.md`

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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,81 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotdeviceadvisor.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTDeviceAdvisor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/literals/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
-    ProtocolType,
-    StatusType,
-    SuiteRunStatusType,
-    TestCaseScenarioStatusType,
-    TestCaseScenarioTypeType,
-    IoTDeviceAdvisorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotdeviceadvisor.literals import AuthenticationMethodType
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDeviceAdvisor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/type_defs/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    ResponseMetadataTypeDef,
-    DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestTypeDef,
-    GetEndpointRequestRequestTypeDef,
-    GetSuiteDefinitionRequestRequestTypeDef,
-    GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunRequestRequestTypeDef,
-    ListSuiteDefinitionsRequestRequestTypeDef,
-    ListSuiteRunsRequestRequestTypeDef,
-    SuiteRunInformationTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StopSuiteRunRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestCaseScenarioTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSuiteDefinitionResponseTypeDef,
-    GetEndpointResponseTypeDef,
-    GetSuiteRunReportResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSuiteRunResponseTypeDef,
-    UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteDefinitionInformationTypeDef,
-    SuiteRunConfigurationOutputTypeDef,
-    SuiteRunConfigurationTypeDef,
-    ListSuiteRunsResponseTypeDef,
-    TestCaseRunTypeDef,
-    GetSuiteDefinitionResponseTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
-    SuiteDefinitionConfigurationUnionTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
-    StartSuiteRunRequestRequestTypeDef,
-    SuiteRunConfigurationUnionTypeDef,
-    GroupResultTypeDef,
-    TestResultTypeDef,
-    GetSuiteRunResponseTypeDef,
-)
+from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotdeviceadvisor",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__main__.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationUnionTypeDef,
-    SuiteRunConfigurationUnionTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
+    SuiteRunConfigurationTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -86,15 +86,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
 
     async def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
@@ -203,15 +203,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_tags_for_resource)
         """
 
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
+        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -242,15 +242,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
 
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationUnionTypeDef,
-    SuiteRunConfigurationUnionTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
+    SuiteRunConfigurationTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -80,15 +80,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
     async def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
@@ -187,15 +187,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_tags_for_resource)
         """
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
+        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -222,15 +222,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
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
@@ -184,14 +185,15 @@
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
@@ -270,26 +272,28 @@
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
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
@@ -182,14 +183,15 @@
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
@@ -268,26 +270,28 @@
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -25,15 +25,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
@@ -48,28 +47,24 @@
     "UntagResourceRequestRequestTypeDef",
     "CreateSuiteDefinitionResponseTypeDef",
     "GetEndpointResponseTypeDef",
     "GetSuiteRunReportResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
-    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
-    "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "GetSuiteDefinitionResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
-    "SuiteDefinitionConfigurationUnionTypeDef",
+    "GetSuiteDefinitionResponseTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
-    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -120,22 +115,20 @@
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
-
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -283,41 +276,14 @@
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
-    {
-        "suiteDefinitionName": str,
-        "rootGroup": str,
-        "devicePermissionRoleArn": str,
-    },
-)
-_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
-    {
-        "devices": List[DeviceUnderTestTypeDef],
-        "intendedForQualification": bool,
-        "isLongDurationTest": bool,
-        "protocol": ProtocolType,
-    },
-    total=False,
-)
-
-
-class SuiteDefinitionConfigurationOutputTypeDef(
-    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
-    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
@@ -329,79 +295,53 @@
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
-
 class SuiteDefinitionConfigurationTypeDef(
     _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
 ):
     pass
 
-
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
         "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
-_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSuiteRunConfigurationOutputTypeDef",
-    {
-        "primaryDevice": DeviceUnderTestTypeDef,
-    },
-)
-_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSuiteRunConfigurationOutputTypeDef",
-    {
-        "selectedTestList": List[str],
-        "parallelRun": bool,
-    },
-    total=False,
-)
-
-
-class SuiteRunConfigurationOutputTypeDef(
-    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": Sequence[str],
+        "selectedTestList": List[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
-
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
-
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -420,54 +360,49 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-SuiteDefinitionConfigurationUnionTypeDef = Union[
-    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-]
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
@@ -493,24 +428,19 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
-
-SuiteRunConfigurationUnionTypeDef = Union[
-    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
-]
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -528,15 +458,15 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -25,14 +25,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
@@ -47,28 +48,24 @@
     "UntagResourceRequestRequestTypeDef",
     "CreateSuiteDefinitionResponseTypeDef",
     "GetEndpointResponseTypeDef",
     "GetSuiteRunReportResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
-    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
-    "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "GetSuiteDefinitionResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
-    "SuiteDefinitionConfigurationUnionTypeDef",
+    "GetSuiteDefinitionResponseTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
-    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -119,20 +116,22 @@
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
+
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -280,39 +279,14 @@
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
-    {
-        "suiteDefinitionName": str,
-        "rootGroup": str,
-        "devicePermissionRoleArn": str,
-    },
-)
-_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
-    {
-        "devices": List[DeviceUnderTestTypeDef],
-        "intendedForQualification": bool,
-        "isLongDurationTest": bool,
-        "protocol": ProtocolType,
-    },
-    total=False,
-)
-
-class SuiteDefinitionConfigurationOutputTypeDef(
-    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
-    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
@@ -324,73 +298,57 @@
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
+
 class SuiteDefinitionConfigurationTypeDef(
     _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
 ):
     pass
 
+
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
         "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
-_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSuiteRunConfigurationOutputTypeDef",
-    {
-        "primaryDevice": DeviceUnderTestTypeDef,
-    },
-)
-_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSuiteRunConfigurationOutputTypeDef",
-    {
-        "selectedTestList": List[str],
-        "parallelRun": bool,
-    },
-    total=False,
-)
-
-class SuiteRunConfigurationOutputTypeDef(
-    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": Sequence[str],
+        "selectedTestList": List[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
+
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
+
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -409,52 +367,51 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-SuiteDefinitionConfigurationUnionTypeDef = Union[
-    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-]
+
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
@@ -480,22 +437,21 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
-SuiteRunConfigurationUnionTypeDef = Union[
-    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
-]
+
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -513,15 +469,15 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,81 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotdeviceadvisor.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTDeviceAdvisor` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/literals/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.literals import (
-    AuthenticationMethodType,
-    ProtocolType,
-    StatusType,
-    SuiteRunStatusType,
-    TestCaseScenarioStatusType,
-    TestCaseScenarioTypeType,
-    IoTDeviceAdvisorServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotdeviceadvisor.literals import AuthenticationMethodType
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTDeviceAdvisor` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/type_defs/).
+
 ```python
-from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    ResponseMetadataTypeDef,
-    DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestTypeDef,
-    GetEndpointRequestRequestTypeDef,
-    GetSuiteDefinitionRequestRequestTypeDef,
-    GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunRequestRequestTypeDef,
-    ListSuiteDefinitionsRequestRequestTypeDef,
-    ListSuiteRunsRequestRequestTypeDef,
-    SuiteRunInformationTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    StopSuiteRunRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestCaseScenarioTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateSuiteDefinitionResponseTypeDef,
-    GetEndpointResponseTypeDef,
-    GetSuiteRunReportResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSuiteRunResponseTypeDef,
-    UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteDefinitionInformationTypeDef,
-    SuiteRunConfigurationOutputTypeDef,
-    SuiteRunConfigurationTypeDef,
-    ListSuiteRunsResponseTypeDef,
-    TestCaseRunTypeDef,
-    GetSuiteDefinitionResponseTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
-    SuiteDefinitionConfigurationUnionTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
-    StartSuiteRunRequestRequestTypeDef,
-    SuiteRunConfigurationUnionTypeDef,
-    GroupResultTypeDef,
-    TestResultTypeDef,
-    GetSuiteRunResponseTypeDef,
-)
+from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

