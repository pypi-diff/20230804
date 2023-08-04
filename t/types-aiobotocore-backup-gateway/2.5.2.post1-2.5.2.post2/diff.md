# Comparing `tmp/types-aiobotocore-backup-gateway-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-backup-gateway-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-backup-gateway-2.5.2.post1.tar` & `types-aiobotocore-backup-gateway-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.285648 types-aiobotocore-backup-gateway-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:51:55.281648 types-aiobotocore-backup-gateway-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.285648 types-aiobotocore-backup-gateway-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.273648 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20562 2023-08-02 14:33:46.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.281648 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.363227 types-aiobotocore-backup-gateway-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-08-04 12:00:28.363227 types-aiobotocore-backup-gateway-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.363227 types-aiobotocore-backup-gateway-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.355227 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19654 2023-08-04 11:40:57.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 11:40:57.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:56.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.363227 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:28.000000 types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/LICENSE` & `types-aiobotocore-backup-gateway-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/README.md` & `types-aiobotocore-backup-gateway-2.5.2.post2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-backup-gateway
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore backup-gateway type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,111 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_backup_gateway.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `BackupGateway` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/literals/).
+
 ```python
-from types_aiobotocore_backup_gateway.literals import (
-    GatewayTypeType,
-    HypervisorStateType,
-    ListGatewaysPaginatorName,
-    ListHypervisorsPaginatorName,
-    ListVirtualMachinesPaginatorName,
-    SyncMetadataStatusType,
-    BackupGatewayServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_backup_gateway.literals import GatewayTypeType
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_backup_gateway.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `BackupGateway` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/type_defs/).
+
 ```python
-from types_aiobotocore_backup_gateway.type_defs import (
-    AssociateGatewayToServerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    BandwidthRateLimitIntervalOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
-    TagTypeDef,
-    DeleteGatewayInputRequestTypeDef,
-    DeleteHypervisorInputRequestTypeDef,
-    DisassociateGatewayFromServerInputRequestTypeDef,
-    MaintenanceStartTimeTypeDef,
-    GatewayTypeDef,
-    GetBandwidthRateLimitScheduleInputRequestTypeDef,
-    GetGatewayInputRequestTypeDef,
-    GetHypervisorInputRequestTypeDef,
-    HypervisorDetailsTypeDef,
-    GetHypervisorPropertyMappingsInputRequestTypeDef,
-    VmwareToAwsTagMappingTypeDef,
-    GetVirtualMachineInputRequestTypeDef,
-    HypervisorTypeDef,
-    PaginatorConfigTypeDef,
-    ListGatewaysInputRequestTypeDef,
-    ListHypervisorsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    ListVirtualMachinesInputRequestTypeDef,
-    VirtualMachineTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
-    VmwareTagTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
-    CreateGatewayOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteHypervisorOutputTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
-    PutBandwidthRateLimitScheduleOutputTypeDef,
-    PutHypervisorPropertyMappingsOutputTypeDef,
-    PutMaintenanceStartTimeOutputTypeDef,
-    StartVirtualMachinesMetadataSyncOutputTypeDef,
-    TagResourceOutputTypeDef,
-    UntagResourceOutputTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateHypervisorOutputTypeDef,
-    GetBandwidthRateLimitScheduleOutputTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
-    CreateGatewayInputRequestTypeDef,
-    ImportHypervisorConfigurationInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    TagResourceInputRequestTypeDef,
-    GatewayDetailsTypeDef,
-    ListGatewaysOutputTypeDef,
-    GetHypervisorOutputTypeDef,
-    GetHypervisorPropertyMappingsOutputTypeDef,
-    PutHypervisorPropertyMappingsInputRequestTypeDef,
-    ListHypervisorsOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
-    ListVirtualMachinesOutputTypeDef,
-    VirtualMachineDetailsTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
-    GetGatewayOutputTypeDef,
-    GetVirtualMachineOutputTypeDef,
-)
+from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
 
 def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/setup.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup-gateway",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__main__.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.BackupGateway 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -278,15 +278,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
 
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalUnionTypeDef,
+    BandwidthRateLimitIntervalTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -255,15 +255,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.py` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
     data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -26,15 +26,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
     "DeleteGatewayInputRequestTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
@@ -72,15 +71,15 @@
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
     "UntagResourceOutputTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateHypervisorOutputTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
@@ -88,15 +87,14 @@
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
@@ -112,44 +110,18 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "DaysOfWeek": List[int],
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-    },
-)
-_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "AverageUploadRateLimitInBitsPerSec": int,
-    },
-    total=False,
-)
-
-
-class BandwidthRateLimitIntervalOutputTypeDef(
-    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
-    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
-):
-    pass
-
-
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
@@ -609,23 +581,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -792,22 +769,14 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-        "GatewayArn": str,
-    },
-)
-
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
     data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -25,15 +25,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
     "DeleteGatewayInputRequestTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
@@ -71,15 +70,15 @@
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
     "UntagResourceOutputTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateHypervisorOutputTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "BandwidthRateLimitIntervalUnionTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
@@ -87,15 +86,14 @@
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
     "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
@@ -111,42 +109,18 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "DaysOfWeek": List[int],
-        "EndHourOfDay": int,
-        "EndMinuteOfHour": int,
-        "StartHourOfDay": int,
-        "StartMinuteOfHour": int,
-    },
-)
-_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
-    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
-    {
-        "AverageUploadRateLimitInBitsPerSec": int,
-    },
-    total=False,
-)
-
-class BandwidthRateLimitIntervalOutputTypeDef(
-    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
-    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
-):
-    pass
-
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
-        "DaysOfWeek": Sequence[int],
+        "DaysOfWeek": List[int],
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
@@ -594,23 +568,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BandwidthRateLimitIntervalUnionTypeDef = Union[
-    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
-]
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -773,22 +752,14 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
-        "GatewayArn": str,
-    },
-)
-
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt` & `types-aiobotocore-backup-gateway-2.5.2.post2/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

