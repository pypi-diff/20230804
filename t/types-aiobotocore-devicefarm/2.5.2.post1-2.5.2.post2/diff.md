# Comparing `tmp/types-aiobotocore-devicefarm-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-devicefarm-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devicefarm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-devicefarm-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-devicefarm-2.5.2.post1.tar` & `types-aiobotocore-devicefarm-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.765607 types-aiobotocore-devicefarm-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-08-02 14:52:09.761607 types-aiobotocore-devicefarm-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.765607 types-aiobotocore-devicefarm-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.753607 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61057 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60951 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-08-02 14:36:17.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-08-02 14:36:17.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74480 2023-08-02 14:36:19.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74389 2023-08-02 14:36:19.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:16.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.761607 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:09.000000 types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.763852 types-aiobotocore-devicefarm-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 12:00:44.755852 types-aiobotocore-devicefarm-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.763852 types-aiobotocore-devicefarm-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.755852 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60953 2023-08-04 11:43:37.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60847 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-08-04 11:43:37.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-08-04 11:43:37.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-08-04 11:43:37.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-08-04 11:43:37.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73144 2023-08-04 11:43:40.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73053 2023-08-04 11:43:38.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:36.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.755852 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:44.000000 types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/LICENSE` & `types-aiobotocore-devicefarm-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/setup.py` & `types-aiobotocore-devicefarm-2.5.2.post2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devicefarm",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__init__.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__init__.pyi` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/__main__.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DeviceFarm 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DeviceFarm 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/client.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
-    DeviceFilterUnionTypeDef,
+    DeviceFilterTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
     GetDeviceResultTypeDef,
@@ -115,25 +115,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
-    TestGridVpcConfigUnionTypeDef,
+    TestGridVpcConfigTypeDef,
     TimestampTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -251,19 +251,15 @@
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_network_profile)
         """
 
     async def create_project(
-        self,
-        *,
-        name: str,
-        defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...
+        self, *, name: str, defaultJobTimeoutMinutes: int = ..., vpcConfig: VpcConfigTypeDef = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_project)
         """
@@ -288,15 +284,15 @@
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_remote_access_session)
         """
 
     async def create_test_grid_project(
-        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigUnionTypeDef = ...
+        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigTypeDef = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_test_grid_project)
         """
@@ -621,19 +617,15 @@
         Gets information about device pools.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_device_pools)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_device_pools)
         """
 
     async def list_devices(
-        self,
-        *,
-        arn: str = ...,
-        nextToken: str = ...,
-        filters: Sequence[DeviceFilterUnionTypeDef] = ...
+        self, *, arn: str = ..., nextToken: str = ..., filters: Sequence[DeviceFilterTypeDef] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_devices)
         """
@@ -991,30 +983,30 @@
 
     async def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_project)
         """
 
     async def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigUnionTypeDef = ...
+        vpcConfig: TestGridVpcConfigTypeDef = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/client.pyi` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
-    DeviceFilterUnionTypeDef,
+    DeviceFilterTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
     GetDeviceResultTypeDef,
@@ -115,25 +115,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
-    TestGridVpcConfigUnionTypeDef,
+    TestGridVpcConfigTypeDef,
     TimestampTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -241,19 +241,15 @@
         """
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_network_profile)
         """
     async def create_project(
-        self,
-        *,
-        name: str,
-        defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...
+        self, *, name: str, defaultJobTimeoutMinutes: int = ..., vpcConfig: VpcConfigTypeDef = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_project)
         """
@@ -276,15 +272,15 @@
         """
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_remote_access_session)
         """
     async def create_test_grid_project(
-        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigUnionTypeDef = ...
+        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigTypeDef = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#create_test_grid_project)
         """
@@ -573,19 +569,15 @@
         """
         Gets information about device pools.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_device_pools)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_device_pools)
         """
     async def list_devices(
-        self,
-        *,
-        arn: str = ...,
-        nextToken: str = ...,
-        filters: Sequence[DeviceFilterUnionTypeDef] = ...
+        self, *, arn: str = ..., nextToken: str = ..., filters: Sequence[DeviceFilterTypeDef] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#list_devices)
         """
@@ -910,29 +902,29 @@
         """
     async def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...
+        vpcConfig: VpcConfigTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_project)
         """
     async def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigUnionTypeDef = ...
+        vpcConfig: TestGridVpcConfigTypeDef = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/literals.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/literals.pyi` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/paginator.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
-    DeviceFilterUnionTypeDef,
+    DeviceFilterTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     ListJobsResultTypeDef,
@@ -202,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[DeviceFilterUnionTypeDef] = ...,
+        filters: Sequence[DeviceFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/paginator.pyi` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
-    DeviceFilterUnionTypeDef,
+    DeviceFilterTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     ListJobsResultTypeDef,
@@ -195,15 +195,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[DeviceFilterUnionTypeDef] = ...,
+        filters: Sequence[DeviceFilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/type_defs.py` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,26 +68,24 @@
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
-    "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteNetworkProfileRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRemoteAccessSessionRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
-    "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
@@ -136,22 +134,20 @@
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "ProblemDetailTypeDef",
-    "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
-    "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
@@ -166,36 +162,39 @@
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
     "ListNetworkProfilesResultTypeDef",
     "UpdateNetworkProfileResultTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateRemoteAccessSessionRequestRequestTypeDef",
     "CreateTestGridProjectRequestRequestTypeDef",
+    "TestGridProjectTypeDef",
     "UpdateTestGridProjectRequestRequestTypeDef",
     "CreateUploadResultTypeDef",
     "GetUploadResultTypeDef",
     "InstallToRemoteAccessSessionResultTypeDef",
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
-    "DeviceSelectionResultTypeDef",
-    "DeviceFilterUnionTypeDef",
     "DeviceSelectionConfigurationTypeDef",
+    "DeviceSelectionResultTypeDef",
+    "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
     "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
@@ -213,46 +212,40 @@
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
     "RecurringChargeTypeDef",
-    "ProjectTypeDef",
-    "VpcConfigUnionTypeDef",
     "ScheduleRunConfigurationTypeDef",
-    "TestGridProjectTypeDef",
-    "TestGridVpcConfigUnionTypeDef",
     "GetAccountSettingsResultTypeDef",
     "CreateDevicePoolResultTypeDef",
     "GetDevicePoolResultTypeDef",
     "ListDevicePoolsResultTypeDef",
     "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
-    "RunTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    "ListDevicesRequestRequestTypeDef",
-    "GetSuiteResultTypeDef",
-    "ListSuitesResultTypeDef",
-    "GetTestResultTypeDef",
-    "ListTestsResultTypeDef",
-    "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
     "ListProjectsResultTypeDef",
     "UpdateProjectResultTypeDef",
-    "GetDevicePoolCompatibilityRequestRequestTypeDef",
-    "ScheduleRunRequestRequestTypeDef",
     "CreateTestGridProjectResultTypeDef",
     "GetTestGridProjectResultTypeDef",
     "ListTestGridProjectsResultTypeDef",
     "UpdateTestGridProjectResultTypeDef",
+    "RunTypeDef",
+    "GetSuiteResultTypeDef",
+    "ListSuitesResultTypeDef",
+    "GetTestResultTypeDef",
+    "ListTestsResultTypeDef",
+    "OfferingTypeDef",
+    "GetDevicePoolCompatibilityRequestRequestTypeDef",
+    "ScheduleRunRequestRequestTypeDef",
     "DevicePoolCompatibilityResultTypeDef",
     "GetDeviceResultTypeDef",
     "JobTypeDef",
     "ListDevicesResultTypeDef",
     "ProblemTypeDef",
     "RemoteAccessSessionTypeDef",
     "GetRunResultTypeDef",
@@ -540,24 +533,14 @@
         "vpceServiceName": str,
         "serviceDnsName": str,
         "vpceConfigurationDescription": str,
     },
     total=False,
 )
 
-CustomerArtifactPathsOutputTypeDef = TypedDict(
-    "CustomerArtifactPathsOutputTypeDef",
-    {
-        "iosPaths": List[str],
-        "androidPaths": List[str],
-        "deviceHostPaths": List[str],
-    },
-    total=False,
-)
-
 CustomerArtifactPathsTypeDef = TypedDict(
     "CustomerArtifactPathsTypeDef",
     {
         "iosPaths": Sequence[str],
         "androidPaths": Sequence[str],
         "deviceHostPaths": Sequence[str],
     },
@@ -623,29 +606,20 @@
 DeleteVPCEConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeviceFilterOutputTypeDef = TypedDict(
-    "DeviceFilterOutputTypeDef",
-    {
-        "attribute": DeviceFilterAttributeType,
-        "operator": RuleOperatorType,
-        "values": List[str],
-    },
-)
-
 DeviceFilterTypeDef = TypedDict(
     "DeviceFilterTypeDef",
     {
         "attribute": DeviceFilterAttributeType,
         "operator": RuleOperatorType,
-        "values": Sequence[str],
+        "values": List[str],
     },
 )
 
 DeviceMinutesTypeDef = TypedDict(
     "DeviceMinutesTypeDef",
     {
         "total": float,
@@ -1287,23 +1261,14 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "vpcId": str,
-    },
-)
-
 _RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
@@ -1358,23 +1323,14 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-TestGridVpcConfigOutputTypeDef = TypedDict(
-    "TestGridVpcConfigOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "vpcId": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1700,14 +1656,26 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "defaultJobTimeoutMinutes": int,
+        "created": datetime,
+        "vpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1778,14 +1746,26 @@
 class CreateTestGridProjectRequestRequestTypeDef(
     _RequiredCreateTestGridProjectRequestRequestTypeDef,
     _OptionalCreateTestGridProjectRequestRequestTypeDef,
 ):
     pass
 
 
+TestGridProjectTypeDef = TypedDict(
+    "TestGridProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "vpcConfig": TestGridVpcConfigTypeDef,
+        "created": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestGridProjectRequestRequestTypeDef",
     {
         "projectArn": str,
     },
 )
 _OptionalUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
@@ -1876,31 +1856,40 @@
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeviceSelectionConfigurationTypeDef = TypedDict(
+    "DeviceSelectionConfigurationTypeDef",
+    {
+        "filters": Sequence[DeviceFilterTypeDef],
+        "maxDevices": int,
+    },
+)
+
 DeviceSelectionResultTypeDef = TypedDict(
     "DeviceSelectionResultTypeDef",
     {
-        "filters": List[DeviceFilterOutputTypeDef],
+        "filters": List[DeviceFilterTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
-DeviceFilterUnionTypeDef = Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]
-DeviceSelectionConfigurationTypeDef = TypedDict(
-    "DeviceSelectionConfigurationTypeDef",
+ListDevicesRequestRequestTypeDef = TypedDict(
+    "ListDevicesRequestRequestTypeDef",
     {
+        "arn": str,
+        "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
-        "maxDevices": int,
     },
+    total=False,
 )
 
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
         "arn": str,
         "name": str,
@@ -1993,14 +1982,24 @@
 class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
     _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
 ):
     pass
 
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2346,27 +2345,14 @@
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
 )
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "defaultJobTimeoutMinutes": int,
-        "created": datetime,
-        "vpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2375,27 +2361,14 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-TestGridProjectTypeDef = TypedDict(
-    "TestGridProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "vpcConfig": TestGridVpcConfigOutputTypeDef,
-        "created": datetime,
-    },
-    total=False,
-)
-
-TestGridVpcConfigUnionTypeDef = Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef]
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2482,14 +2455,80 @@
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProjectResultTypeDef = TypedDict(
+    "GetProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsResultTypeDef = TypedDict(
+    "ListProjectsResultTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectResultTypeDef = TypedDict(
+    "UpdateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTestGridProjectResultTypeDef = TypedDict(
+    "CreateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTestGridProjectResultTypeDef = TypedDict(
+    "GetTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTestGridProjectsResultTypeDef = TypedDict(
+    "ListTestGridProjectsResultTypeDef",
+    {
+        "testGridProjects": List[TestGridProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTestGridProjectResultTypeDef = TypedDict(
+    "UpdateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "platform": DevicePlatformType,
@@ -2511,40 +2550,20 @@
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
         "radios": RadiosTypeDef,
         "location": LocationTypeDef,
-        "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
+        "customerArtifactPaths": CustomerArtifactPathsTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterUnionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDevicesRequestRequestTypeDef = TypedDict(
-    "ListDevicesRequestRequestTypeDef",
-    {
-        "arn": str,
-        "nextToken": str,
-        "filters": Sequence[DeviceFilterUnionTypeDef],
+        "vpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
@@ -2587,47 +2606,14 @@
         "type": Literal["RECURRING"],
         "platform": DevicePlatformType,
         "recurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProjectResultTypeDef = TypedDict(
-    "GetProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsResultTypeDef = TypedDict(
-    "ListProjectsResultTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProjectResultTypeDef = TypedDict(
-    "UpdateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
     },
 )
 _OptionalGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
@@ -2672,47 +2658,14 @@
 
 class ScheduleRunRequestRequestTypeDef(
     _RequiredScheduleRunRequestRequestTypeDef, _OptionalScheduleRunRequestRequestTypeDef
 ):
     pass
 
 
-CreateTestGridProjectResultTypeDef = TypedDict(
-    "CreateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTestGridProjectResultTypeDef = TypedDict(
-    "GetTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTestGridProjectsResultTypeDef = TypedDict(
-    "ListTestGridProjectsResultTypeDef",
-    {
-        "testGridProjects": List[TestGridProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTestGridProjectResultTypeDef = TypedDict(
-    "UpdateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
         "compatible": bool,
         "incompatibilityMessages": List[IncompatibilityMessageTypeDef],
     },
@@ -2792,15 +2745,15 @@
         "clientId": str,
         "billingMethod": BillingMethodType,
         "deviceMinutes": DeviceMinutesTypeDef,
         "endpoint": str,
         "deviceUdid": str,
         "interactionMode": InteractionModeType,
         "skipAppResign": bool,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm/type_defs.pyi` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,24 @@
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
-    "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteNetworkProfileRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRemoteAccessSessionRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
-    "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
@@ -135,22 +133,20 @@
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "ProblemDetailTypeDef",
-    "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
-    "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
@@ -165,36 +161,39 @@
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
     "ListNetworkProfilesResultTypeDef",
     "UpdateNetworkProfileResultTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateRemoteAccessSessionRequestRequestTypeDef",
     "CreateTestGridProjectRequestRequestTypeDef",
+    "TestGridProjectTypeDef",
     "UpdateTestGridProjectRequestRequestTypeDef",
     "CreateUploadResultTypeDef",
     "GetUploadResultTypeDef",
     "InstallToRemoteAccessSessionResultTypeDef",
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
-    "DeviceSelectionResultTypeDef",
-    "DeviceFilterUnionTypeDef",
     "DeviceSelectionConfigurationTypeDef",
+    "DeviceSelectionResultTypeDef",
+    "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
     "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
@@ -212,46 +211,40 @@
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
     "RecurringChargeTypeDef",
-    "ProjectTypeDef",
-    "VpcConfigUnionTypeDef",
     "ScheduleRunConfigurationTypeDef",
-    "TestGridProjectTypeDef",
-    "TestGridVpcConfigUnionTypeDef",
     "GetAccountSettingsResultTypeDef",
     "CreateDevicePoolResultTypeDef",
     "GetDevicePoolResultTypeDef",
     "ListDevicePoolsResultTypeDef",
     "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
-    "RunTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    "ListDevicesRequestRequestTypeDef",
-    "GetSuiteResultTypeDef",
-    "ListSuitesResultTypeDef",
-    "GetTestResultTypeDef",
-    "ListTestsResultTypeDef",
-    "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
     "ListProjectsResultTypeDef",
     "UpdateProjectResultTypeDef",
-    "GetDevicePoolCompatibilityRequestRequestTypeDef",
-    "ScheduleRunRequestRequestTypeDef",
     "CreateTestGridProjectResultTypeDef",
     "GetTestGridProjectResultTypeDef",
     "ListTestGridProjectsResultTypeDef",
     "UpdateTestGridProjectResultTypeDef",
+    "RunTypeDef",
+    "GetSuiteResultTypeDef",
+    "ListSuitesResultTypeDef",
+    "GetTestResultTypeDef",
+    "ListTestsResultTypeDef",
+    "OfferingTypeDef",
+    "GetDevicePoolCompatibilityRequestRequestTypeDef",
+    "ScheduleRunRequestRequestTypeDef",
     "DevicePoolCompatibilityResultTypeDef",
     "GetDeviceResultTypeDef",
     "JobTypeDef",
     "ListDevicesResultTypeDef",
     "ProblemTypeDef",
     "RemoteAccessSessionTypeDef",
     "GetRunResultTypeDef",
@@ -531,24 +524,14 @@
         "vpceServiceName": str,
         "serviceDnsName": str,
         "vpceConfigurationDescription": str,
     },
     total=False,
 )
 
-CustomerArtifactPathsOutputTypeDef = TypedDict(
-    "CustomerArtifactPathsOutputTypeDef",
-    {
-        "iosPaths": List[str],
-        "androidPaths": List[str],
-        "deviceHostPaths": List[str],
-    },
-    total=False,
-)
-
 CustomerArtifactPathsTypeDef = TypedDict(
     "CustomerArtifactPathsTypeDef",
     {
         "iosPaths": Sequence[str],
         "androidPaths": Sequence[str],
         "deviceHostPaths": Sequence[str],
     },
@@ -614,29 +597,20 @@
 DeleteVPCEConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeviceFilterOutputTypeDef = TypedDict(
-    "DeviceFilterOutputTypeDef",
-    {
-        "attribute": DeviceFilterAttributeType,
-        "operator": RuleOperatorType,
-        "values": List[str],
-    },
-)
-
 DeviceFilterTypeDef = TypedDict(
     "DeviceFilterTypeDef",
     {
         "attribute": DeviceFilterAttributeType,
         "operator": RuleOperatorType,
-        "values": Sequence[str],
+        "values": List[str],
     },
 )
 
 DeviceMinutesTypeDef = TypedDict(
     "DeviceMinutesTypeDef",
     {
         "total": float,
@@ -1250,23 +1224,14 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "vpcId": str,
-    },
-)
-
 _RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
@@ -1319,23 +1284,14 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-TestGridVpcConfigOutputTypeDef = TypedDict(
-    "TestGridVpcConfigOutputTypeDef",
-    {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-        "vpcId": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1645,14 +1601,26 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "defaultJobTimeoutMinutes": int,
+        "created": datetime,
+        "vpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1717,14 +1685,26 @@
 
 class CreateTestGridProjectRequestRequestTypeDef(
     _RequiredCreateTestGridProjectRequestRequestTypeDef,
     _OptionalCreateTestGridProjectRequestRequestTypeDef,
 ):
     pass
 
+TestGridProjectTypeDef = TypedDict(
+    "TestGridProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "vpcConfig": TestGridVpcConfigTypeDef,
+        "created": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestGridProjectRequestRequestTypeDef",
     {
         "projectArn": str,
     },
 )
 _OptionalUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
@@ -1813,31 +1793,40 @@
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeviceSelectionConfigurationTypeDef = TypedDict(
+    "DeviceSelectionConfigurationTypeDef",
+    {
+        "filters": Sequence[DeviceFilterTypeDef],
+        "maxDevices": int,
+    },
+)
+
 DeviceSelectionResultTypeDef = TypedDict(
     "DeviceSelectionResultTypeDef",
     {
-        "filters": List[DeviceFilterOutputTypeDef],
+        "filters": List[DeviceFilterTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
-DeviceFilterUnionTypeDef = Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]
-DeviceSelectionConfigurationTypeDef = TypedDict(
-    "DeviceSelectionConfigurationTypeDef",
+ListDevicesRequestRequestTypeDef = TypedDict(
+    "ListDevicesRequestRequestTypeDef",
     {
+        "arn": str,
+        "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
-        "maxDevices": int,
     },
+    total=False,
 )
 
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
         "arn": str,
         "name": str,
@@ -1926,14 +1915,24 @@
 
 class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
     _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
 ):
     pass
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2259,27 +2258,14 @@
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
 )
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "defaultJobTimeoutMinutes": int,
-        "created": datetime,
-        "vpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2288,27 +2274,14 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-TestGridProjectTypeDef = TypedDict(
-    "TestGridProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "vpcConfig": TestGridVpcConfigOutputTypeDef,
-        "created": datetime,
-    },
-    total=False,
-)
-
-TestGridVpcConfigUnionTypeDef = Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef]
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2395,14 +2368,80 @@
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProjectResultTypeDef = TypedDict(
+    "GetProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsResultTypeDef = TypedDict(
+    "ListProjectsResultTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectResultTypeDef = TypedDict(
+    "UpdateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTestGridProjectResultTypeDef = TypedDict(
+    "CreateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTestGridProjectResultTypeDef = TypedDict(
+    "GetTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTestGridProjectsResultTypeDef = TypedDict(
+    "ListTestGridProjectsResultTypeDef",
+    {
+        "testGridProjects": List[TestGridProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTestGridProjectResultTypeDef = TypedDict(
+    "UpdateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "platform": DevicePlatformType,
@@ -2424,40 +2463,20 @@
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
         "radios": RadiosTypeDef,
         "location": LocationTypeDef,
-        "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
+        "customerArtifactPaths": CustomerArtifactPathsTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterUnionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDevicesRequestRequestTypeDef = TypedDict(
-    "ListDevicesRequestRequestTypeDef",
-    {
-        "arn": str,
-        "nextToken": str,
-        "filters": Sequence[DeviceFilterUnionTypeDef],
+        "vpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
@@ -2500,47 +2519,14 @@
         "type": Literal["RECURRING"],
         "platform": DevicePlatformType,
         "recurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProjectResultTypeDef = TypedDict(
-    "GetProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsResultTypeDef = TypedDict(
-    "ListProjectsResultTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProjectResultTypeDef = TypedDict(
-    "UpdateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
     },
 )
 _OptionalGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
@@ -2581,47 +2567,14 @@
 )
 
 class ScheduleRunRequestRequestTypeDef(
     _RequiredScheduleRunRequestRequestTypeDef, _OptionalScheduleRunRequestRequestTypeDef
 ):
     pass
 
-CreateTestGridProjectResultTypeDef = TypedDict(
-    "CreateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTestGridProjectResultTypeDef = TypedDict(
-    "GetTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTestGridProjectsResultTypeDef = TypedDict(
-    "ListTestGridProjectsResultTypeDef",
-    {
-        "testGridProjects": List[TestGridProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTestGridProjectResultTypeDef = TypedDict(
-    "UpdateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
         "compatible": bool,
         "incompatibilityMessages": List[IncompatibilityMessageTypeDef],
     },
@@ -2701,15 +2654,15 @@
         "clientId": str,
         "billingMethod": BillingMethodType,
         "deviceMinutes": DeviceMinutesTypeDef,
         "endpoint": str,
         "deviceUdid": str,
         "interactionMode": InteractionModeType,
         "skipAppResign": bool,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post1/types_aiobotocore_devicefarm.egg-info/SOURCES.txt` & `types-aiobotocore-devicefarm-2.5.2.post2/types_aiobotocore_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

