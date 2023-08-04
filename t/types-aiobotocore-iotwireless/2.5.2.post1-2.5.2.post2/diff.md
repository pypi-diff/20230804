# Comparing `tmp/types-aiobotocore-iotwireless-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotwireless-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotwireless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotwireless-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-iotwireless-2.5.2.post1.tar` & `types-aiobotocore-iotwireless-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75886 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    75768 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102175 2023-08-02 14:41:09.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102082 2023-08-02 14:41:08.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.186643 types-aiobotocore-iotwireless-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12422 2023-08-04 13:59:13.186643 types-aiobotocore-iotwireless-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10888 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.186643 types-aiobotocore-iotwireless-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:41:25.000000 types-aiobotocore-iotwireless-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.186643 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      474 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      473 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    75826 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    75708 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12334 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12332 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97141 2023-08-04 13:41:29.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97052 2023-08-04 13:41:28.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:26.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.186643 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12422 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:13.000000 types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/LICENSE` & `types-aiobotocore-iotwireless-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/setup.py` & `types-aiobotocore-iotwireless-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotwireless",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__main__.py` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTWireless 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTWireless 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.py` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,19 +96,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceProfileUnionTypeDef,
-    LoRaWANDeviceUnionTypeDef,
+    LoRaWANDeviceProfileTypeDef,
+    LoRaWANDeviceTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayUnionTypeDef,
-    LoRaWANMulticastSessionUnionTypeDef,
+    LoRaWANGatewayTypeDef,
+    LoRaWANMulticastSessionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -127,16 +127,16 @@
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
     TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionUnionTypeDef,
-    WirelessGatewayLogOptionUnionTypeDef,
+    WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -297,15 +297,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
 
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -388,30 +388,30 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
 
     async def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayUnionTypeDef,
+        LoRaWAN: LoRaWANGatewayTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -1199,15 +1199,15 @@
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_fuota_task)
         """
 
     async def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_multicast_group_session)
         """
@@ -1320,16 +1320,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
 
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
```

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.pyi` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,19 +96,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceProfileUnionTypeDef,
-    LoRaWANDeviceUnionTypeDef,
+    LoRaWANDeviceProfileTypeDef,
+    LoRaWANDeviceTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayUnionTypeDef,
-    LoRaWANMulticastSessionUnionTypeDef,
+    LoRaWANGatewayTypeDef,
+    LoRaWANMulticastSessionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -127,16 +127,16 @@
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
     TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionUnionTypeDef,
-    WirelessGatewayLogOptionUnionTypeDef,
+    WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -281,15 +281,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -367,29 +367,29 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
     async def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayUnionTypeDef,
+        LoRaWAN: LoRaWANGatewayTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -1101,15 +1101,15 @@
         """
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_fuota_task)
         """
     async def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_multicast_group_session)
         """
@@ -1213,16 +1213,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
```

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.py` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationConfigTypeType",
     "BatteryLevelType",
     "ConnectionStatusType",
     "DeviceProfileTypeType",
     "DeviceStateType",
     "DlClassType",
@@ -62,15 +61,14 @@
     "WirelessGatewayTypeType",
     "IoTWirelessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ApplicationConfigTypeType = Literal["SemtechGeolocation"]
 BatteryLevelType = Literal["critical", "low", "normal"]
 ConnectionStatusType = Literal["Connected", "Disconnected"]
 DeviceProfileTypeType = Literal["LoRaWAN", "Sidewalk"]
 DeviceStateType = Literal[
     "Provisioned", "RegisteredNotSeen", "RegisteredReachable", "RegisteredUnreachable"
 ]
@@ -162,14 +160,15 @@
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
@@ -265,14 +264,15 @@
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
@@ -351,26 +351,28 @@
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

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.pyi` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApplicationConfigTypeType",
     "BatteryLevelType",
     "ConnectionStatusType",
     "DeviceProfileTypeType",
     "DeviceStateType",
     "DlClassType",
@@ -61,14 +62,15 @@
     "WirelessGatewayTypeType",
     "IoTWirelessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ApplicationConfigTypeType = Literal["SemtechGeolocation"]
 BatteryLevelType = Literal["critical", "low", "normal"]
 ConnectionStatusType = Literal["Connected", "Disconnected"]
 DeviceProfileTypeType = Literal["LoRaWAN", "Sidewalk"]
 DeviceStateType = Literal[
     "Provisioned", "RegisteredNotSeen", "RegisteredReachable", "RegisteredUnreachable"
 ]
@@ -160,14 +162,15 @@
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
@@ -263,14 +266,15 @@
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
@@ -349,26 +353,28 @@
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

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.py` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,30 +58,28 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SessionKeysAbpV10XTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
-    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
@@ -119,21 +117,20 @@
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
-    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionOutputTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "TimestampTypeDef",
@@ -242,15 +239,14 @@
     "GetWirelessGatewayTaskResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SendDataToMulticastGroupResponseTypeDef",
     "SendDataToWirelessDeviceResponseTypeDef",
     "StartSingleWirelessDeviceImportTaskResponseTypeDef",
     "StartWirelessDeviceImportTaskResponseTypeDef",
     "TestWirelessDeviceResponseTypeDef",
-    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
@@ -268,27 +264,24 @@
     "ListDeviceProfilesResponseTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
-    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
-    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
-    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
@@ -307,31 +300,24 @@
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
-    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
-    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
-    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
-    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
-    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
-    "LoRaWANMulticastSessionUnionTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
@@ -341,32 +327,29 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
-    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "WirelessGatewayLogOptionUnionTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
-    "LoRaWANDeviceUnionTypeDef",
+    "GetWirelessDeviceResponseTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -480,23 +463,14 @@
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
-BeaconingOutputTypeDef = TypedDict(
-    "BeaconingOutputTypeDef",
-    {
-        "DataRate": int,
-        "Frequencies": List[int],
-    },
-    total=False,
-)
-
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
@@ -530,19 +504,17 @@
     {
         "PilotPower": int,
         "BaseStationId": int,
     },
     total=False,
 )
 
-
 class CdmaNmrObjTypeDef(_RequiredCdmaNmrObjTypeDef, _OptionalCdmaNmrObjTypeDef):
     pass
 
-
 CertificateListTypeDef = TypedDict(
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
@@ -657,21 +629,19 @@
         "FactorySupport": bool,
         "ApId": str,
         "DeviceTypeId": str,
     },
     total=False,
 )
 
-
 class DakCertificateMetadataTypeDef(
     _RequiredDakCertificateMetadataTypeDef, _OptionalDakCertificateMetadataTypeDef
 ):
     pass
 
-
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -714,22 +684,20 @@
     "_OptionalDeleteQueuedMessagesRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class DeleteQueuedMessagesRequestRequestTypeDef(
     _RequiredDeleteQueuedMessagesRequestRequestTypeDef,
     _OptionalDeleteQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteServiceProfileRequestRequestTypeDef = TypedDict(
     "DeleteServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -778,22 +746,20 @@
     "_OptionalDeregisterWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class DeregisterWirelessDeviceRequestRequestTypeDef(
     _RequiredDeregisterWirelessDeviceRequestRequestTypeDef,
     _OptionalDeregisterWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 DestinationsTypeDef = TypedDict(
     "DestinationsTypeDef",
     {
         "Arn": str,
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
@@ -920,40 +886,14 @@
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANDeviceProfileOutputTypeDef = TypedDict(
-    "LoRaWANDeviceProfileOutputTypeDef",
-    {
-        "SupportsClassB": bool,
-        "ClassBTimeout": int,
-        "PingSlotPeriod": int,
-        "PingSlotDr": int,
-        "PingSlotFreq": int,
-        "SupportsClassC": bool,
-        "ClassCTimeout": int,
-        "MacVersion": str,
-        "RegParamsRevision": str,
-        "RxDelay1": int,
-        "RxDrOffset1": int,
-        "RxDataRate2": int,
-        "RxFreq2": int,
-        "FactoryPresetFreqsList": List[int],
-        "MaxEirp": int,
-        "MaxDutyCycle": int,
-        "RfRegion": str,
-        "SupportsJoin": bool,
-        "Supports32BitFCnt": bool,
-    },
-    total=False,
-)
-
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -987,16 +927,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionOutputTypeDef = TypedDict(
-    "LoRaWANMulticastSessionOutputTypeDef",
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1050,19 +990,17 @@
         "AssistPosition": Sequence[float],
         "AssistAltitude": float,
         "Use2DSolver": bool,
     },
     total=False,
 )
 
-
 class GnssTypeDef(_RequiredGnssTypeDef, _OptionalGnssTypeDef):
     pass
 
-
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
@@ -1094,22 +1032,20 @@
     "_OptionalGetResourceEventConfigurationRequestRequestTypeDef",
     {
         "PartnerType": Literal["Sidewalk"],
     },
     total=False,
 )
 
-
 class GetResourceEventConfigurationRequestRequestTypeDef(
     _RequiredGetResourceEventConfigurationRequestRequestTypeDef,
     _OptionalGetResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceLogLevelRequestRequestTypeDef = TypedDict(
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
@@ -1322,22 +1258,20 @@
         "MaxResults": int,
         "NextToken": str,
         "Status": OnboardStatusType,
     },
     total=False,
 )
 
-
 class ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListEventConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventConfigurationsRequestRequestTypeDef",
     {
         "ResourceType": EventNotificationResourceTypeType,
     },
 )
 _OptionalListEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1345,22 +1279,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEventConfigurationsRequestRequestTypeDef(
     _RequiredListEventConfigurationsRequestRequestTypeDef,
     _OptionalListEventConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListFuotaTasksRequestRequestTypeDef = TypedDict(
     "ListFuotaTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1377,22 +1309,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMulticastGroupsByFuotaTaskRequestRequestTypeDef(
     _RequiredListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
     _OptionalListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
 ):
     pass
 
-
 MulticastGroupByFuotaTaskTypeDef = TypedDict(
     "MulticastGroupByFuotaTaskTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -1465,22 +1395,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
-
 class ListQueuedMessagesRequestRequestTypeDef(
     _RequiredListQueuedMessagesRequestRequestTypeDef,
     _OptionalListQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
-
 ListServiceProfilesRequestRequestTypeDef = TypedDict(
     "ListServiceProfilesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1639,19 +1567,17 @@
     {
         "Rsrp": int,
         "Rsrq": float,
     },
     total=False,
 )
 
-
 class LteNmrObjTypeDef(_RequiredLteNmrObjTypeDef, _OptionalLteNmrObjTypeDef):
     pass
 
-
 SemtechGnssConfigurationTypeDef = TypedDict(
     "SemtechGnssConfigurationTypeDef",
     {
         "Status": PositionConfigurationStatusType,
         "Fec": PositionConfigurationFecType,
     },
 )
@@ -1748,19 +1674,17 @@
         "UtranCid": int,
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
-
 class TdscdmaNmrObjTypeDef(_RequiredTdscdmaNmrObjTypeDef, _OptionalTdscdmaNmrObjTypeDef):
     pass
 
-
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1785,21 +1709,19 @@
         "Expression": str,
         "Description": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
-
 UpdatePositionRequestRequestTypeDef = TypedDict(
     "UpdatePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
@@ -1819,22 +1741,20 @@
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "MaxEirp": float,
     },
     total=False,
 )
 
-
 class UpdateWirelessGatewayRequestRequestTypeDef(
     _RequiredUpdateWirelessGatewayRequestRequestTypeDef,
     _OptionalUpdateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
-
 WcdmaLocalIdTypeDef = TypedDict(
     "WcdmaLocalIdTypeDef",
     {
         "Uarfcndl": int,
         "Psc": int,
     },
 )
@@ -1852,19 +1772,17 @@
     {
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
-
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
-
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
@@ -1908,22 +1826,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef(
     _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
         "RoleArn": str,
@@ -1935,21 +1851,19 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -1957,22 +1871,20 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -1980,22 +1892,20 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2244,28 +2154,14 @@
     "TestWirelessDeviceResponseTypeDef",
     {
         "Result": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANGatewayOutputTypeDef = TypedDict(
-    "LoRaWANGatewayOutputTypeDef",
-    {
-        "GatewayEui": str,
-        "RfRegion": str,
-        "JoinEuiFilters": List[List[str]],
-        "NetIdFilters": List[str],
-        "SubBands": List[int],
-        "Beaconing": BeaconingOutputTypeDef,
-        "MaxEirp": float,
-    },
-    total=False,
-)
-
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
@@ -2287,22 +2183,20 @@
     "_OptionalUpdateResourcePositionRequestRequestTypeDef",
     {
         "GeoJsonPayload": BlobTypeDef,
     },
     total=False,
 )
 
-
 class UpdateResourcePositionRequestRequestTypeDef(
     _RequiredUpdateResourcePositionRequestRequestTypeDef,
     _OptionalUpdateResourcePositionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2316,19 +2210,17 @@
         "BaseLat": float,
         "BaseLng": float,
         "CdmaNmr": Sequence[CdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class CdmaObjTypeDef(_RequiredCdmaObjTypeDef, _OptionalCdmaObjTypeDef):
     pass
 
-
 SidewalkDeviceTypeDef = TypedDict(
     "SidewalkDeviceTypeDef",
     {
         "AmazonId": str,
         "SidewalkId": str,
         "SidewalkManufacturingSn": str,
         "DeviceCertificates": List[CertificateListTypeDef],
@@ -2400,21 +2292,19 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
-
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
@@ -2428,21 +2318,19 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
-
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMulticastGroupRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
 )
 _OptionalCreateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2452,22 +2340,20 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMulticastGroupRequestRequestTypeDef(
     _RequiredCreateMulticastGroupRequestRequestTypeDef,
     _OptionalCreateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2476,22 +2362,20 @@
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMulticastGroupRequestRequestTypeDef(
     _RequiredUpdateMulticastGroupRequestRequestTypeDef,
     _OptionalUpdateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2504,22 +2388,20 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "MulticastGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationResponseTypeDef",
     {
         "TraceContent": TraceContentTypeDef,
         "WirelessDevices": List[str],
         "WirelessGateways": List[str],
         "Description": str,
@@ -2547,22 +2429,20 @@
         "Description": str,
         "MulticastGroupsToAdd": Sequence[str],
         "MulticastGroupsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateServiceProfileRequestRequestTypeDef = TypedDict(
     "CreateServiceProfileRequestRequestTypeDef",
     {
         "Name": str,
         "LoRaWAN": LoRaWANServiceProfileTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
@@ -2645,26 +2525,14 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
-FPortsOutputTypeDef = TypedDict(
-    "FPortsOutputTypeDef",
-    {
-        "Fuota": int,
-        "Multicast": int,
-        "ClockSync": int,
-        "Positioning": PositioningTypeDef,
-        "Applications": List[ApplicationConfigTypeDef],
-    },
-    total=False,
-)
-
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2687,35 +2555,23 @@
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ParticipatingGatewaysOutputTypeDef = TypedDict(
-    "ParticipatingGatewaysOutputTypeDef",
-    {
-        "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
-        "TransmissionInterval": int,
-    },
-)
-
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": Sequence[GatewayListItemTypeDef],
+        "GatewayList": List[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
-LoRaWANDeviceProfileUnionTypeDef = Union[
-    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
-]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2744,19 +2600,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2767,26 +2631,14 @@
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
-    {
-        "DlDr": int,
-        "DlFreq": int,
-        "SessionStartTime": TimestampTypeDef,
-        "SessionTimeout": int,
-        "PingSlotPeriod": int,
-    },
-    total=False,
-)
-
 LoRaWANStartFuotaTaskTypeDef = TypedDict(
     "LoRaWANStartFuotaTaskTypeDef",
     {
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
@@ -2850,19 +2702,17 @@
     {
         "RxLevel": int,
         "GlobalIdentity": GlobalIdentityTypeDef,
     },
     total=False,
 )
 
-
 class GsmNmrObjTypeDef(_RequiredGsmNmrObjTypeDef, _OptionalGsmNmrObjTypeDef):
     pass
 
-
 ImportedWirelessDeviceTypeDef = TypedDict(
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
@@ -2987,19 +2837,17 @@
         "Rsrq": float,
         "NrCapable": bool,
         "LteNmr": Sequence[LteNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class LteObjTypeDef(_RequiredLteObjTypeDef, _OptionalLteObjTypeDef):
     pass
 
-
 PositionSolverConfigurationsTypeDef = TypedDict(
     "PositionSolverConfigurationsTypeDef",
     {
         "SemtechGnss": SemtechGnssConfigurationTypeDef,
     },
     total=False,
 )
@@ -3025,22 +2873,20 @@
         "ClientRequestToken": str,
         "DeviceName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartSingleWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef",
     {
         "DestinationName": str,
         "Sidewalk": SidewalkStartImportInfoTypeDef,
     },
 )
@@ -3049,22 +2895,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
-
 UpdatePartnerAccountRequestRequestTypeDef = TypedDict(
     "UpdatePartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkUpdateAccountTypeDef,
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
@@ -3095,19 +2939,17 @@
         "Rscp": int,
         "PathLoss": int,
         "TdscdmaNmr": Sequence[TdscdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class TdscdmaObjTypeDef(_RequiredTdscdmaObjTypeDef, _OptionalTdscdmaObjTypeDef):
     pass
 
-
 _RequiredWcdmaObjTypeDef = TypedDict(
     "_RequiredWcdmaObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "UtranCid": int,
     },
@@ -3120,160 +2962,107 @@
         "Rscp": int,
         "PathLoss": int,
         "WcdmaNmr": Sequence[WcdmaNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
-
-_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
-    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "LogLevel": LogLevelType,
-    },
-)
-_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
-    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
-    {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
-    },
-    total=False,
-)
-
-
-class WirelessDeviceLogOptionOutputTypeDef(
-    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
-):
-    pass
-
-
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
-
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
-
-_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
         "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-
-class WirelessGatewayLogOptionOutputTypeDef(
-    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
-
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
     {
-        "Type": Literal["LoRaWAN"],
-        "LogLevel": LogLevelType,
+        "LoRaWAN": LoRaWANGatewayTypeDef,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
     {
-        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
     },
     total=False,
 )
 
-
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
-
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
+        "LoRaWAN": LoRaWANGatewayTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
-        "LastUplinkReceivedAt": str,
-    },
-    total=False,
-)
-
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
-    {
         "LoRaWAN": LoRaWANGatewayTypeDef,
-    },
-)
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
-
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
-):
-    pass
-
-
-LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3290,35 +3079,20 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANDeviceOutputTypeDef = TypedDict(
-    "LoRaWANDeviceOutputTypeDef",
-    {
-        "DevEui": str,
-        "DeviceProfileId": str,
-        "ServiceProfileId": str,
-        "OtaaV1_1": OtaaV11TypeDef,
-        "OtaaV1_0_x": OtaaV10XTypeDef,
-        "AbpV1_1": AbpV11TypeDef,
-        "AbpV1_0_x": AbpV10XTypeDef,
-        "FPorts": FPortsOutputTypeDef,
-    },
-    total=False,
-)
-
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3338,64 +3112,42 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
-LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
-    "LoRaWANSendDataToDeviceOutputTypeDef",
-    {
-        "FPort": int,
-        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
-    },
-    total=False,
-)
-
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
-LoRaWANMulticastSessionUnionTypeDef = Union[
-    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
-]
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-    },
-)
-
 _RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartFuotaTaskRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
     },
     total=False,
 )
 
-
 class StartFuotaTaskRequestRequestTypeDef(
     _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
 ):
     pass
 
-
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3417,19 +3169,17 @@
         "GsmTimingAdvance": int,
         "RxLevel": int,
         "GsmNmr": Sequence[GsmNmrObjTypeDef],
     },
     total=False,
 )
 
-
 class GsmObjTypeDef(_RequiredGsmObjTypeDef, _OptionalGsmObjTypeDef):
     pass
 
-
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3476,22 +3226,20 @@
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateResourceEventConfigurationRequestRequestTypeDef(
     _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef,
     _OptionalUpdateResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
         "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
         "Join": JoinResourceTypeEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
@@ -3572,22 +3320,20 @@
     {
         "Solvers": PositionSolverConfigurationsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
-
 class PutPositionConfigurationRequestRequestTypeDef(
     _RequiredPutPositionConfigurationRequestRequestTypeDef,
     _OptionalPutPositionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3600,30 +3346,34 @@
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
-WirelessDeviceLogOptionUnionTypeDef = Union[
-    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
-]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WirelessGatewayLogOptionUnionTypeDef = Union[
-    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
-]
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
+    },
+    total=False,
+)
+
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3634,32 +3384,14 @@
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "DestinationName": str,
     },
 )
@@ -3673,23 +3405,38 @@
         "Tags": Sequence[TagTypeDef],
         "Positioning": PositioningConfigStatusType,
         "Sidewalk": SidewalkCreateWirelessDeviceTypeDef,
     },
     total=False,
 )
 
-
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3700,29 +3447,27 @@
         "Description": str,
         "LoRaWAN": LoRaWANUpdateDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
     },
     total=False,
 )
 
-
 class UpdateWirelessDeviceRequestRequestTypeDef(
     _RequiredUpdateWirelessDeviceRequestRequestTypeDef,
     _OptionalUpdateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3768,22 +3513,20 @@
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     {
         "AutoCreateTasks": bool,
         "Name": str,
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "Arn": str,
@@ -3805,24 +3548,14 @@
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
-    },
-    total=False,
-)
-
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3840,22 +3573,20 @@
     "_OptionalSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessMetadata": WirelessMetadataTypeDef,
     },
     total=False,
 )
 
-
 class SendDataToWirelessDeviceRequestRequestTypeDef(
     _RequiredSendDataToWirelessDeviceRequestRequestTypeDef,
     _OptionalSendDataToWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
```

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.pyi` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "SessionKeysAbpV10XTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
-    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
     "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
@@ -118,21 +118,20 @@
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
-    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionOutputTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
     "TimestampTypeDef",
@@ -241,15 +240,14 @@
     "GetWirelessGatewayTaskResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SendDataToMulticastGroupResponseTypeDef",
     "SendDataToWirelessDeviceResponseTypeDef",
     "StartSingleWirelessDeviceImportTaskResponseTypeDef",
     "StartWirelessDeviceImportTaskResponseTypeDef",
     "TestWirelessDeviceResponseTypeDef",
-    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
     "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
@@ -267,27 +265,24 @@
     "ListDeviceProfilesResponseTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
-    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
-    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
-    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
     "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
@@ -306,31 +301,24 @@
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
-    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
-    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
-    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
-    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
-    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
-    "LoRaWANMulticastSessionUnionTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
     "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
@@ -340,32 +328,29 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
-    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "WirelessGatewayLogOptionUnionTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "GetWirelessDeviceResponseTypeDef",
     "CreateWirelessDeviceRequestRequestTypeDef",
-    "LoRaWANDeviceUnionTypeDef",
+    "GetWirelessDeviceResponseTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -479,23 +464,14 @@
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
-BeaconingOutputTypeDef = TypedDict(
-    "BeaconingOutputTypeDef",
-    {
-        "DataRate": int,
-        "Frequencies": List[int],
-    },
-    total=False,
-)
-
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
@@ -529,17 +505,19 @@
     {
         "PilotPower": int,
         "BaseStationId": int,
     },
     total=False,
 )
 
+
 class CdmaNmrObjTypeDef(_RequiredCdmaNmrObjTypeDef, _OptionalCdmaNmrObjTypeDef):
     pass
 
+
 CertificateListTypeDef = TypedDict(
     "CertificateListTypeDef",
     {
         "SigningAlg": SigningAlgType,
         "Value": str,
     },
 )
@@ -654,19 +632,21 @@
         "FactorySupport": bool,
         "ApId": str,
         "DeviceTypeId": str,
     },
     total=False,
 )
 
+
 class DakCertificateMetadataTypeDef(
     _RequiredDakCertificateMetadataTypeDef, _OptionalDakCertificateMetadataTypeDef
 ):
     pass
 
+
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -709,20 +689,22 @@
     "_OptionalDeleteQueuedMessagesRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class DeleteQueuedMessagesRequestRequestTypeDef(
     _RequiredDeleteQueuedMessagesRequestRequestTypeDef,
     _OptionalDeleteQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteServiceProfileRequestRequestTypeDef = TypedDict(
     "DeleteServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -771,20 +753,22 @@
     "_OptionalDeregisterWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class DeregisterWirelessDeviceRequestRequestTypeDef(
     _RequiredDeregisterWirelessDeviceRequestRequestTypeDef,
     _OptionalDeregisterWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 DestinationsTypeDef = TypedDict(
     "DestinationsTypeDef",
     {
         "Arn": str,
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
@@ -911,40 +895,14 @@
 GetDeviceProfileRequestRequestTypeDef = TypedDict(
     "GetDeviceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANDeviceProfileOutputTypeDef = TypedDict(
-    "LoRaWANDeviceProfileOutputTypeDef",
-    {
-        "SupportsClassB": bool,
-        "ClassBTimeout": int,
-        "PingSlotPeriod": int,
-        "PingSlotDr": int,
-        "PingSlotFreq": int,
-        "SupportsClassC": bool,
-        "ClassCTimeout": int,
-        "MacVersion": str,
-        "RegParamsRevision": str,
-        "RxDelay1": int,
-        "RxDrOffset1": int,
-        "RxDataRate2": int,
-        "RxFreq2": int,
-        "FactoryPresetFreqsList": List[int],
-        "MaxEirp": int,
-        "MaxDutyCycle": int,
-        "RfRegion": str,
-        "SupportsJoin": bool,
-        "Supports32BitFCnt": bool,
-    },
-    total=False,
-)
-
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -978,16 +936,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionOutputTypeDef = TypedDict(
-    "LoRaWANMulticastSessionOutputTypeDef",
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1041,17 +999,19 @@
         "AssistPosition": Sequence[float],
         "AssistAltitude": float,
         "Use2DSolver": bool,
     },
     total=False,
 )
 
+
 class GnssTypeDef(_RequiredGnssTypeDef, _OptionalGnssTypeDef):
     pass
 
+
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
@@ -1083,20 +1043,22 @@
     "_OptionalGetResourceEventConfigurationRequestRequestTypeDef",
     {
         "PartnerType": Literal["Sidewalk"],
     },
     total=False,
 )
 
+
 class GetResourceEventConfigurationRequestRequestTypeDef(
     _RequiredGetResourceEventConfigurationRequestRequestTypeDef,
     _OptionalGetResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceLogLevelRequestRequestTypeDef = TypedDict(
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
@@ -1309,20 +1271,22 @@
         "MaxResults": int,
         "NextToken": str,
         "Status": OnboardStatusType,
     },
     total=False,
 )
 
+
 class ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListEventConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventConfigurationsRequestRequestTypeDef",
     {
         "ResourceType": EventNotificationResourceTypeType,
     },
 )
 _OptionalListEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -1330,20 +1294,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEventConfigurationsRequestRequestTypeDef(
     _RequiredListEventConfigurationsRequestRequestTypeDef,
     _OptionalListEventConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListFuotaTasksRequestRequestTypeDef = TypedDict(
     "ListFuotaTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1360,20 +1326,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMulticastGroupsByFuotaTaskRequestRequestTypeDef(
     _RequiredListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
     _OptionalListMulticastGroupsByFuotaTaskRequestRequestTypeDef,
 ):
     pass
 
+
 MulticastGroupByFuotaTaskTypeDef = TypedDict(
     "MulticastGroupByFuotaTaskTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
@@ -1446,20 +1414,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WirelessDeviceType": WirelessDeviceTypeType,
     },
     total=False,
 )
 
+
 class ListQueuedMessagesRequestRequestTypeDef(
     _RequiredListQueuedMessagesRequestRequestTypeDef,
     _OptionalListQueuedMessagesRequestRequestTypeDef,
 ):
     pass
 
+
 ListServiceProfilesRequestRequestTypeDef = TypedDict(
     "ListServiceProfilesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1618,17 +1588,19 @@
     {
         "Rsrp": int,
         "Rsrq": float,
     },
     total=False,
 )
 
+
 class LteNmrObjTypeDef(_RequiredLteNmrObjTypeDef, _OptionalLteNmrObjTypeDef):
     pass
 
+
 SemtechGnssConfigurationTypeDef = TypedDict(
     "SemtechGnssConfigurationTypeDef",
     {
         "Status": PositionConfigurationStatusType,
         "Fec": PositionConfigurationFecType,
     },
 )
@@ -1725,17 +1697,19 @@
         "UtranCid": int,
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
+
 class TdscdmaNmrObjTypeDef(_RequiredTdscdmaNmrObjTypeDef, _OptionalTdscdmaNmrObjTypeDef):
     pass
 
+
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1760,19 +1734,21 @@
         "Expression": str,
         "Description": str,
         "RoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
+
 UpdatePositionRequestRequestTypeDef = TypedDict(
     "UpdatePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
@@ -1792,20 +1768,22 @@
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "MaxEirp": float,
     },
     total=False,
 )
 
+
 class UpdateWirelessGatewayRequestRequestTypeDef(
     _RequiredUpdateWirelessGatewayRequestRequestTypeDef,
     _OptionalUpdateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
+
 WcdmaLocalIdTypeDef = TypedDict(
     "WcdmaLocalIdTypeDef",
     {
         "Uarfcndl": int,
         "Psc": int,
     },
 )
@@ -1823,17 +1801,19 @@
     {
         "Rscp": int,
         "PathLoss": int,
     },
     total=False,
 )
 
+
 class WcdmaNmrObjTypeDef(_RequiredWcdmaNmrObjTypeDef, _OptionalWcdmaNmrObjTypeDef):
     pass
 
+
 WirelessDeviceEventLogOptionTypeDef = TypedDict(
     "WirelessDeviceEventLogOptionTypeDef",
     {
         "Event": WirelessDeviceEventType,
         "LogLevel": LogLevelType,
     },
 )
@@ -1877,20 +1857,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef(
     _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "Name": str,
         "ExpressionType": ExpressionTypeType,
         "Expression": str,
         "RoleArn": str,
@@ -1902,19 +1884,21 @@
         "Description": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -1922,20 +1906,22 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -1943,20 +1929,22 @@
     {
         "QueryString": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(
     _RequiredStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     _OptionalStartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2205,28 +2193,14 @@
     "TestWirelessDeviceResponseTypeDef",
     {
         "Result": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANGatewayOutputTypeDef = TypedDict(
-    "LoRaWANGatewayOutputTypeDef",
-    {
-        "GatewayEui": str,
-        "RfRegion": str,
-        "JoinEuiFilters": List[List[str]],
-        "NetIdFilters": List[str],
-        "SubBands": List[int],
-        "Beaconing": BeaconingOutputTypeDef,
-        "MaxEirp": float,
-    },
-    total=False,
-)
-
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
@@ -2248,20 +2222,22 @@
     "_OptionalUpdateResourcePositionRequestRequestTypeDef",
     {
         "GeoJsonPayload": BlobTypeDef,
     },
     total=False,
 )
 
+
 class UpdateResourcePositionRequestRequestTypeDef(
     _RequiredUpdateResourcePositionRequestRequestTypeDef,
     _OptionalUpdateResourcePositionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2275,17 +2251,19 @@
         "BaseLat": float,
         "BaseLng": float,
         "CdmaNmr": Sequence[CdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class CdmaObjTypeDef(_RequiredCdmaObjTypeDef, _OptionalCdmaObjTypeDef):
     pass
 
+
 SidewalkDeviceTypeDef = TypedDict(
     "SidewalkDeviceTypeDef",
     {
         "AmazonId": str,
         "SidewalkId": str,
         "SidewalkManufacturingSn": str,
         "DeviceCertificates": List[CertificateListTypeDef],
@@ -2357,19 +2335,21 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
+
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateFuotaTaskRequestRequestTypeDef = TypedDict(
@@ -2383,19 +2363,21 @@
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
     },
     total=False,
 )
 
+
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMulticastGroupRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
 )
 _OptionalCreateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2405,20 +2387,22 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMulticastGroupRequestRequestTypeDef(
     _RequiredCreateMulticastGroupRequestRequestTypeDef,
     _OptionalCreateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2427,20 +2411,22 @@
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANMulticastTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMulticastGroupRequestRequestTypeDef(
     _RequiredUpdateMulticastGroupRequestRequestTypeDef,
     _OptionalUpdateMulticastGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
@@ -2453,20 +2439,22 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "MulticastGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalCreateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
     "GetNetworkAnalyzerConfigurationResponseTypeDef",
     {
         "TraceContent": TraceContentTypeDef,
         "WirelessDevices": List[str],
         "WirelessGateways": List[str],
         "Description": str,
@@ -2494,20 +2482,22 @@
         "Description": str,
         "MulticastGroupsToAdd": Sequence[str],
         "MulticastGroupsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef(
     _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
     _OptionalUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateServiceProfileRequestRequestTypeDef = TypedDict(
     "CreateServiceProfileRequestRequestTypeDef",
     {
         "Name": str,
         "LoRaWAN": LoRaWANServiceProfileTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
@@ -2590,26 +2580,14 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
-FPortsOutputTypeDef = TypedDict(
-    "FPortsOutputTypeDef",
-    {
-        "Fuota": int,
-        "Multicast": int,
-        "ClockSync": int,
-        "Positioning": PositioningTypeDef,
-        "Applications": List[ApplicationConfigTypeDef],
-    },
-    total=False,
-)
-
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2632,35 +2610,23 @@
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ParticipatingGatewaysOutputTypeDef = TypedDict(
-    "ParticipatingGatewaysOutputTypeDef",
-    {
-        "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
-        "TransmissionInterval": int,
-    },
-)
-
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": Sequence[GatewayListItemTypeDef],
+        "GatewayList": List[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
-LoRaWANDeviceProfileUnionTypeDef = Union[
-    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
-]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2689,19 +2655,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2712,26 +2686,14 @@
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
-    {
-        "DlDr": int,
-        "DlFreq": int,
-        "SessionStartTime": TimestampTypeDef,
-        "SessionTimeout": int,
-        "PingSlotPeriod": int,
-    },
-    total=False,
-)
-
 LoRaWANStartFuotaTaskTypeDef = TypedDict(
     "LoRaWANStartFuotaTaskTypeDef",
     {
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
@@ -2795,17 +2757,19 @@
     {
         "RxLevel": int,
         "GlobalIdentity": GlobalIdentityTypeDef,
     },
     total=False,
 )
 
+
 class GsmNmrObjTypeDef(_RequiredGsmNmrObjTypeDef, _OptionalGsmNmrObjTypeDef):
     pass
 
+
 ImportedWirelessDeviceTypeDef = TypedDict(
     "ImportedWirelessDeviceTypeDef",
     {
         "Sidewalk": ImportedSidewalkDeviceTypeDef,
     },
     total=False,
 )
@@ -2930,17 +2894,19 @@
         "Rsrq": float,
         "NrCapable": bool,
         "LteNmr": Sequence[LteNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class LteObjTypeDef(_RequiredLteObjTypeDef, _OptionalLteObjTypeDef):
     pass
 
+
 PositionSolverConfigurationsTypeDef = TypedDict(
     "PositionSolverConfigurationsTypeDef",
     {
         "SemtechGnss": SemtechGnssConfigurationTypeDef,
     },
     total=False,
 )
@@ -2966,20 +2932,22 @@
         "ClientRequestToken": str,
         "DeviceName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartSingleWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef",
     {
         "DestinationName": str,
         "Sidewalk": SidewalkStartImportInfoTypeDef,
     },
 )
@@ -2988,20 +2956,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartWirelessDeviceImportTaskRequestRequestTypeDef(
     _RequiredStartWirelessDeviceImportTaskRequestRequestTypeDef,
     _OptionalStartWirelessDeviceImportTaskRequestRequestTypeDef,
 ):
     pass
 
+
 UpdatePartnerAccountRequestRequestTypeDef = TypedDict(
     "UpdatePartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkUpdateAccountTypeDef,
         "PartnerAccountId": str,
         "PartnerType": Literal["Sidewalk"],
     },
@@ -3032,17 +3002,19 @@
         "Rscp": int,
         "PathLoss": int,
         "TdscdmaNmr": Sequence[TdscdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class TdscdmaObjTypeDef(_RequiredTdscdmaObjTypeDef, _OptionalTdscdmaObjTypeDef):
     pass
 
+
 _RequiredWcdmaObjTypeDef = TypedDict(
     "_RequiredWcdmaObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "UtranCid": int,
     },
@@ -3055,148 +3027,115 @@
         "Rscp": int,
         "PathLoss": int,
         "WcdmaNmr": Sequence[WcdmaNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
-_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
-    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "LogLevel": LogLevelType,
-    },
-)
-_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
-    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
-    {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
-    },
-    total=False,
-)
-
-class WirelessDeviceLogOptionOutputTypeDef(
-    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
-):
-    pass
 
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
+
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
-_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
+
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
         "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-class WirelessGatewayLogOptionOutputTypeDef(
-    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
+
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
     {
-        "Type": Literal["LoRaWAN"],
-        "LogLevel": LogLevelType,
+        "LoRaWAN": LoRaWANGatewayTypeDef,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
     {
-        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
     },
     total=False,
 )
 
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
 ):
     pass
 
+
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
+        "LoRaWAN": LoRaWANGatewayTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
-        "LastUplinkReceivedAt": str,
-    },
-    total=False,
-)
-
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
-    {
         "LoRaWAN": LoRaWANGatewayTypeDef,
-    },
-)
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
-):
-    pass
-
-LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3213,35 +3152,20 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoRaWANDeviceOutputTypeDef = TypedDict(
-    "LoRaWANDeviceOutputTypeDef",
-    {
-        "DevEui": str,
-        "DeviceProfileId": str,
-        "ServiceProfileId": str,
-        "OtaaV1_1": OtaaV11TypeDef,
-        "OtaaV1_0_x": OtaaV10XTypeDef,
-        "AbpV1_1": AbpV11TypeDef,
-        "AbpV1_0_x": AbpV10XTypeDef,
-        "FPorts": FPortsOutputTypeDef,
-    },
-    total=False,
-)
-
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3261,62 +3185,44 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
-LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
-    "LoRaWANSendDataToDeviceOutputTypeDef",
-    {
-        "FPort": int,
-        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
-    },
-    total=False,
-)
-
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
-LoRaWANMulticastSessionUnionTypeDef = Union[
-    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
-]
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-    },
-)
-
 _RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartFuotaTaskRequestRequestTypeDef",
     {
         "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
     },
     total=False,
 )
 
+
 class StartFuotaTaskRequestRequestTypeDef(
     _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
 ):
     pass
 
+
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3338,17 +3244,19 @@
         "GsmTimingAdvance": int,
         "RxLevel": int,
         "GsmNmr": Sequence[GsmNmrObjTypeDef],
     },
     total=False,
 )
 
+
 class GsmObjTypeDef(_RequiredGsmObjTypeDef, _OptionalGsmObjTypeDef):
     pass
 
+
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3395,20 +3303,22 @@
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateResourceEventConfigurationRequestRequestTypeDef(
     _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef,
     _OptionalUpdateResourceEventConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetEventConfigurationByResourceTypesResponseTypeDef = TypedDict(
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
         "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
         "Join": JoinResourceTypeEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
@@ -3489,20 +3399,22 @@
     {
         "Solvers": PositionSolverConfigurationsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+
 class PutPositionConfigurationRequestRequestTypeDef(
     _RequiredPutPositionConfigurationRequestRequestTypeDef,
     _OptionalPutPositionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3515,30 +3427,34 @@
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
-WirelessDeviceLogOptionUnionTypeDef = Union[
-    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
-]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WirelessGatewayLogOptionUnionTypeDef = Union[
-    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
-]
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
+    },
+    total=False,
+)
+
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3549,32 +3465,14 @@
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "DestinationName": str,
     },
 )
@@ -3588,21 +3486,40 @@
         "Tags": Sequence[TagTypeDef],
         "Positioning": PositioningConfigStatusType,
         "Sidewalk": SidewalkCreateWirelessDeviceTypeDef,
     },
     total=False,
 )
 
+
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
+
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3613,27 +3530,29 @@
         "Description": str,
         "LoRaWAN": LoRaWANUpdateDeviceTypeDef,
         "Positioning": PositioningConfigStatusType,
     },
     total=False,
 )
 
+
 class UpdateWirelessDeviceRequestRequestTypeDef(
     _RequiredUpdateWirelessDeviceRequestRequestTypeDef,
     _OptionalUpdateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3679,20 +3598,22 @@
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(
     _RequiredCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     _OptionalCreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     {
         "AutoCreateTasks": bool,
         "Name": str,
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "Arn": str,
@@ -3714,24 +3635,14 @@
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
-    },
-    total=False,
-)
-
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3749,20 +3660,22 @@
     "_OptionalSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "WirelessMetadata": WirelessMetadataTypeDef,
     },
     total=False,
 )
 
+
 class SendDataToWirelessDeviceRequestRequestTypeDef(
     _RequiredSendDataToWirelessDeviceRequestRequestTypeDef,
     _OptionalSendDataToWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
```

### Comparing `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt` & `types-aiobotocore-iotwireless-2.5.2.post2/types_aiobotocore_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

